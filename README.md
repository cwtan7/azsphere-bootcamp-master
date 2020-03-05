# Azure-Sphere-Bootcamp

This repo is built for Azure Sphere Bootcamp Hands-on day. It provides all required information for trainee to follow and finish all hands-on labs. 

# Pre-Lab prerequisites

Follow [Get started with a development kit](https://docs.microsoft.com/en-us/azure-sphere/install/overview) to complete all neccessary steps before start.

> All hands-on and setup are based on Windows and Visual Studio. Linux and VS Code are not used for this bootcamp

Quick check list:
- [FTDI driver](https://www.ftdichip.com/Drivers/VCP.htm) is alreadyinstalled and three COMx ports are present in Device Manager
![](/img/readme/devicedriver.png)
- Up to date Visual Studio and [Azure Sphere SDK for **Visual Studio**](https://docs.microsoft.com/en-us/azure-sphere/install/install-sdk#azure-sphere-sdk-for-visual-studio) are installed
- Already has a Microsoft account
- Has a Azure account and a free subscription or pay-as-you-go subscription for Lab-3 and Lab-4
- Logged in using Azure Sphere command line utility: For first time / unregistered user, please use `azsphere login --newuser <MS account>` and subsequently `azsphere login`.
- Device is recovered by `azsphere device recover`
- Create a Azure Sphere tenant by `azsphere tenant create -n <tenant name>` if there is no tenant in your orgnization.
- Has selected Azure Sphere tenant by `azsphere tenant select -i <tenant id>`
- (New device ONLY) Device is claimed to user's tenant by `azsphere device claim`
- Device is recovered by `azsphere device recover` command to have a knowning good Azure Sphere OS.
- [Git](https://git-scm.com/download/win) is installed and added to PATH.

# Hardware

The hands-on can be used with both MT3620_RDB and AVNET_MT3620_SK. 

## MT3620_RDB

Detailed information about this hardware can be found on [azure-sphere-hardware-designs](https://github.com/Azure/azure-sphere-hardware-designs)

![](/img/readme/RDB.png)

## AVNET_MT3620_SK

Detailed information about this hardware can be found in this [community](https://www.element14.com/community/community/designcenter/azure-sphere-starter-kits)

![](/img/readme/AzureSphereKit_front.png)

> **NOTE:** AVNET_MT3620_SK comes with on-board sensor such as accelemeter, gyrometer, temperature and pressure sensors. 

# Labs

- [Lab-1 Blinking LED](lab_tutorial/lab-1.md)
- [Lab-2 Application Over-the-Air deployment](lab_tutorial/lab-2.md)
- [Lab-3 Connect to Azure IoT Hub](lab_tutorial/lab-3.md)
- [Lab-4 Visualize real world data on Azure IoT Central](lab_tutorial/lab-4.md)

# Sample Code Disclaimer

**Sample code – No Warranties**
THE SAMPLE CODE SOFTWARE IS PROVIDED “AS IS” AND WITHOUT WARRANTY. TO THE MAXIMUM EXTENT PERMITTED BY LAW, MICROSOFT DISCLAIMS ANY AND ALL OTHER WARRANTIES, WHETHER EXPRESS OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, ANY IMPLIED WARRANTIES OF MERCHANTABILITY, NON-INFRINGEMENT, OR FITNESS FOR A PARTICULAR PURPOSE, WHETHER ARISING BY A COURSE OF DEALING, USAGE OR TRADE PRACTICE OR COURSE OF PERFORMANCE. In no event shall Microsoft, its licensors, the authors or copyright holders be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the software or the use thereof. 
 
This code may contain errors and/or may not operate correctly. Microsoft undertakes no duty to correct any errors or update the software. Your use of this code is optional and subject to any license provided therewith or referenced therein, if any. Microsoft does not provide you with any license or other rights to any Microsoft product or service through the code provided to you.
