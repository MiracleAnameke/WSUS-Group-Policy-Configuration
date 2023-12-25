# WSUS Group Policy Configuration

## Description
This repository provides a detailed guide on setting up a Windows domain with WSUS for managing Windows Updates. It covers creating user accounts on Windows Server 2008, joining Windows 7 and Windows 10 VMs to the domain, configuring Group Policy Objects for WSUS, and confirming GPO application.

## Setup Environment

- **Windows Server 2008 R2**: Configured as a domain controller.
- **Windows 7 and Windows 10 VMs**: Configured to join the newly created domain.

## Configuration Steps

### Step 1: Create Accounts on Server 2008
Create administrator and user accounts within Active Directory Users and Computers.

<p align="center">
  <img src="https://i.imgur.com/eyYFFbF.png" height="80%" width="80%" alt="Create Accounts on Server 2008"/>
</p>

### Step 2 and 3: Join W7 VM and Win 10 to the Domain
Modify network settings to point to the domain controller and join both VMs to the domain.

<p align="center">
  <img src="https://i.imgur.com/LQo5jMl.png" height="80%" width="80%" alt="Join W7 VM to the Domain"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/yMvHz3i.png" height="80%" width="80%" alt="Join Win 10 to the Domain"/>
</p>

### Step 4: Creating a Group Policy Object for WSUS on S2008R2
Configure a new GPO for managing WSUS updates in the domain using the Group Policy Management console.

<p align="center">
  <img src="https://i.imgur.com/DmHL0Iw.png" height="80%" width="80%" alt="Creating GPO for WSUS"/>
</p>

### Step 5: Confirm Application of GPO with RSOP.msc
Verify the GPO application on client machines using the `rsop.msc` utility.

<p align="center">
  <img src="https://i.imgur.com/fxNr8iC.png" height="80%" width="80%" alt="Confirm GPO Application"/>
</p>

## How to Use
Follow the steps provided to set up your environment for WSUS updates. Administrative privileges are required to perform these operations.

## Contributing
Contributions are welcome. Please fork the repository, make your changes, and submit a pull request with your enhancements.
