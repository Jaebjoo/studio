---
title: Studio 6 
layout: default
description: Automation of VM creation
---

## Studio 6 : 
# Automation of VM creation

#### 

##### The following is the script used for the VM creation.
It takes a csv file and a cloud.init file
cloud init runs the first time the VM boots.

$List = Import-CSV C:\Users\jooj2\Desktop\vms.csv -Header 'Name'
ForEach($Student in $List)
{

$VMName = $Student.Name + "IN616-test5"
$ComputerName = $Student.Name + ".IN616"
$VMSize = "Standard_B1ls"
$ResourceGroupName ="IN616Dev"
$LocationName = "australiasoutheast"
$VMLocalAdminUser = "student"
$VMLocalAdminSecurePassword = ConvertTo-SecureString jae!Rohill1234 -AsPlainText -Force
$NetworkName = "IN616_network"
$ImageName = "Ubuntu Server 18.04 LTS - Gen1"
$OpenPorts = "22"




$NetworkName = "IN616_network"
$NICName = $VMName
$SubnetName = "IN616"
$SubnetAddressPrefix = "10.2.2.0/24"
$VnetAddressPrefix = "10.2.2.0/24"

$publicIp = New-AzPublicIpAddress -Name $VMName -ResourceGroupName $ResourceGroupName -AllocationMethod Static -DomainNameLabel $dnsPrefix -Location $LocationName

$SingleSubnet = New-AzVirtualNetworkSubnetConfig -Name $SubnetName -AddressPrefix $SubnetAddressPrefix
$Vnet = New-AzVirtualNetwork -Name $NetworkName -ResourceGroupName $ResourceGroupName -Location $LocationName -AddressPrefix $VnetAddressPrefix -Subnet $SingleSubnet
$NIC = New-AzNetworkInterface -Name $NICName -ResourceGroupName $ResourceGroupName -Location $LocationName -SubnetId $Vnet.Subnets[0].Id -PublicIPAddressID $publicIp.Id

$Credential = New-Object System.Management.Automation.PSCredential ($VMLocalAdminUser, $VMLocalAdminSecurePassword);

$VirtualMachine = New-AzVMConfig -VMName $VMName -VMSize $VMSize

$VirtualMachine = Add-AzVMNetworkInterface -VM $VirtualMachine -Id $NIC.Id
$VirtualMachine = Set-AzVMSourceImage -VM $VirtualMachine -PublisherName 'Canonical' -Offer 'UbuntuServer' -Skus '18.04-LTS' -Version latest
$VirtualMachine = Set-AzVMOperatingSystem -VM $VirtualMachine -Linux -ComputerName $ComputerName -Credential $Credential -CustomData (Get-Content -Path C:\Users\jooj2\Desktop\cloud_init.txt -Raw)


New-AzVM -ResourceGroupName $ResourceGroupName -Location $LocationName -VM $VirtualMachine -Verbose
}

$CloudinitFile = Import-CSV C:\Users\jooj2\Desktop\cloud_init.txt
$EncodedText=(Get-Content -raw C:\Users\jooj2\Desktop\cloud_init.txt)

##### The following is the cloud.init file

#cloud-config
users:
  - default
  - name: student
    groups: sudo
    sudo: ['ALL=(ALL) NOPASSWD:ALL']
    shell: /bin/bash
	
chpasswd:
    list: |
         student: password
    expire: False

It will create the user and then change the password to "password"


