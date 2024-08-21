---
ms.date: 08/04/2020
title: Using ISOs
description: How to use ISOs
author: bleblanc
manager: jhow
ms.tgt_pltfrm: na

ms.author: jhow
ms.localizationpriority: medium
ms.topic: article
ms.service: windows-insider
---

# Using ISOs

If your device is hard to use because of an issue, or if you want to switch out of the Dev Channel or stop receiving preview builds, you might need to use an ISO for a clean installation or in-place upgrade. ISOs are available for both Windows 10 Insider Preview Builds and for Windows 11 Insider Preview Builds.

> [!div class="nextstepaction"]
> [Download Windows Insider ISOs](https://aka.ms/WIPISO)

## In-place upgrade with a Windows Insider Preview ISO 

1. [Download your chosen ISO from the Windows Insider ISO page](https://aka.ms/WIPISO) by saving it to a location on your device or creating a bootable USB.

2. Open File Explorer and go to where you saved the ISO. Select the ISO file to open it, which lets Windows mount the image so you can access it.

3. Select the setup.exe file to launch the install process.

4. During setup, select the **Keep Windows settings, personal files, and apps** option.

5. Once it's finished installing, go to [**Settings** > **Windows Update** > **Windows Insider Program**](https://aka.ms/WIPSettings) to make sure your Windows Insider settings are correct.

## Clean installation with a Windows Insider Preview ISO

1. Back up all your files and applications. A clean install with a Windows Insider Preview ISO will erase all of your files, settings, and applications.

2. [Download your chosen ISO from the Windows Insider ISO page](https://aka.ms/WIPISO) by saving it to a location on your device or creating a bootable USB.

3. Open File Explorer and go to where you saved the ISO. Select the ISO file to open it, which lets Windows mount the image so you can access it.

4. Select the setup.exe file to launch the install process.

5. During setup, select the **Change what to keep** option, and then choose **Nothing** on the next screen to complete a clean install.

6. Once it's finished installing, make sure your Windows Insider settings are correct.

- In Windows 10, go to [**Settings** > **Update & Security** > **Windows Insider Program**](https://aka.ms/WIPSettings)

- In Windows 11, go to [**Settings** > **Windows Update** > **Windows Insider Program**](https://aka.ms/WIPSettings)

## Creating a bootable USB for Windows Insider ISOs

If you're having certain issues that prevent you from downloading an ISO to your device, or you need to quickly set up a new device in the Windows Insider Program, a bootable USB made from a Windows Insider ISO file can help.


1. [Download your chosen ISO from the Windows Insider ISO page](https://aka.ms/WIPISO) by saving it to a location on your device you can easily remember.

2. Connect a USB drive that's at least 8 GB. **Back up any data on the drive you want to save, because any data on it will be erased.**

3. Open Start menu. Search for and launch the Recovery Drive application.

4. When the application opens, uncheck the "Back up system files to the recovery drive." box and click Next.

5. Select your drive from the list and click Next.

6.  You'll see a confirmation prompt. Click Create. When this completes your USB drive will now be in a bootable configuration. Next we'll add the contents of the ISO file to it.

7.  Locate the ISO file you downloaded in step 1 above.  Right-click the ISO file and select Mount.

8.  The ISO file will be mounted as a new drive letter on your computer and open in a new File Explorer window.

9.  Copy all the contents of the mounted ISO folder onto the bootable USB you just created.

10. Once the copy process is finished, you're all set. Now you can use it on a device.

11.  To un-mount the ISO file, navigate to that drive letter in File Explorer.  In the toolbar, click eject.


- If you use this drive to upgrade a device that already has Windows on it, connect it to the device, open File Explorer, locate the drive, and launch setup.exe to get started.

- If you use this drive to do a clean Windows install, connect it to the target device and reboot. You may also need to adjust your BIOS or UEFI settings to allow it to boot from a USB-based drive.

## Clean installation with a Windows 11 ISO (Not an Insider Preview Build)

1. Back up all your files and applications. A clean install with a Windows 11 ISO will erase all of your files, settings, and applications.

2. [Download the latest Windows 11 ISO](https://www.microsoft.com/software-download/windows11) by saving it to a location on your PC or creating a bootable USB.

3. Open File Explorer and go to where you saved the ISO. Select the ISO file to open it, which lets Windows mount the image so you can access it.

4. Select the setup.exe file to launch the install process.

5. During setup, select the **Change what to keep** option, and then choose **Nothing** on the next screen to complete a clean install.

6. Once it's finished installing, go to [**Settings** > **Windows Update** > **Windows Insider Program**](https://aka.ms/WIPSettings) if you'd like to set up Insider Preview builds again. [Get more help setting up Insider Preview builds.](./get-started.md)

## Clean installation with a Windows 10 ISO (Not an Insider Preview build)

1. Back up all your files and applications. A clean install with a Windows 10 ISO will erase all of your files, settings, and applications.

2. [Download the latest Windows 10 ISO](https://www.microsoft.com/software-download/windows10) by saving it to a location on your PC or creating a bootable USB.

3. Open File Explorer and go to where you saved the ISO. Select the ISO file to open it, which lets Windows mount the image so you can access it.

4. Select the setup.exe file to launch the install process.

5. During setup, select the **Change what to keep** option, and then choose **Nothing** on the next screen to complete a clean install.

6. Once it's finished installing, go to [**Settings** > **Update & Security** > **Windows Insider Program**](https://aka.ms/WIPSettings) if you'd like to set up Insider Preview builds again. [Get more help setting up Insider Preview builds.](./get-started.md)

