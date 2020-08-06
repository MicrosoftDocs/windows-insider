---
title: Using ISOs
description: How to use ISOs
author: bleblanc
manager: dougkim
ms.tgt_pltfrm: na
ms.devlang: na
ms.author: v-allsh
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
---

# Using ISOs

If your device is hard to use because of an issue, or if you want to switch out of the Dev Channel or stop receiving preview builds, you might need to use an ISO for a clean installation or in-place upgrade. ISOs are available for both Windows 10 Insider Preview Builds and for Windows.

> [!div class="nextstepaction"]
> [Download Windows Insider ISOs](https://aka.ms/WIPISO)

## In-place upgrade with a Windows Insider Preview ISO 

1. [Download your chosen ISO from the Windows Insider ISO page](https://aka.ms/WIPISO) by saving it to a location on your device or creating a bootable USB.

2. Open File Explorer and go to where you saved the ISO. Select the ISO file to open it, which lets Windows mount the image so you can access it.

3. Select the setup.exe file to launch the install process.

4. During setup, select the **Keep Windows settings, personal files, and apps** option.

5. Once it's finished installing, go to **[Settings > Update & Security > Windows Insider Program](https://aka.ms/WIPSettings)** to make sure your Windows Insider settings are correct.

## Clean installation with a Windows Insider Preview ISO 

1. Back up all your files and applications. A clean install with a Windows Insider ISO will erase all of your files, settings, and applications.

2. [Download your chosen ISO from the Windows Insider ISO page](https://aka.ms/WIPISO) by saving it to a location on your device or creating a bootable USB.

3. Open File Explorer and go to where you saved the ISO. Select the ISO file to open it, which lets Windows mount the image so you can access it.

4. Select the setup.exe file to launch the install process.

5. During setup, select the **Change what to keep** option, and then choose **Nothing** on the next screen to complete a clean intall.

6. Once it's finished installing, go to **[Settings > Update & Security > Windows Insider Program](https://aka.ms/WIPSettings)** to make sure your Windows Insider settings are correct.

## Creating a bootable USB for Windows Insider ISOs

If you're having certain issues that prevent you from downloading an ISO to your device, or you need to quickly set up a new device in the Windows Insider Program, a bootable USB made from a Windows Insider ISO file can help.

> [!NOTE] 
> There are many third-party software applications that are capable of converting a USB drive into a bootable format. We're using [Rufus](https://rufus.akeo.ie/) in this example since it's free and lightweight on system resources. You can use any software that can format the USB into a bootable format and convert the ISO into the decompiled installation files.

1. [Download your chosen ISO from the Windows Insider ISO page](https://aka.ms/WIPISO) by saving it to a location on your device you can easily remember.

2. Connect a USB drive that's at least 8GB. **Back up any data on the drive you want to save, because any data on it will erased.**

3. Launch [Rufus](https://rufus.akeo.ie/) or your preferred software.

4. Configure the Rufus menu options:

![Rufus menu options](images/Rufus-ISO-options.png)

- If you have multiple drives connected via USB (external hard drive, thumb drive, etc.), make sure you select the right device from the dropdown.

- **Partition scheme and target system type** should be set to **MBR partition scheme for BIOS or UEFI**. 

- **File system** should be set to **NTFS**. If for some reason this doesn't work on your device, you can re-create it using FAT32.

- **Cluster size** can stay on **4096 bytes (Default)**

- For **New volume label**, enter a name of your choosing.

- Under **Format Options**, **1 Pass** should be selected from the first dropdown. Select the checkboxes beside **Quick format**, **Create a bootable disk using**, and **Create extended label and icon files**. Beside **Create a bootable disk using**, choose **ISO Image** from the dropdown, then select the disk icon next to the dropdown and navigate to the ISO file you downloaded.

5. Select **Start**, and Rufus will format your USB and decompile the ISO.

6. Once it's finished, you're all set. Now you can use it on a device.

- If you use this drive to upgrade a device that already has Windows on it, connect it to the device, open File Explorer, locate the drive, and launch setup.exe to get started.

- If you use this drive to do a clean Windows install, connect it to the device and reboot. You may also need to adjust your BIOS or UEFI settings to allow it to boot from a USB-based drive.

## Clean installation of Windows

> [!NOTE] 
> A clean installation is an advanced option to help you start fresh on your device. This will remove all your personal files, apps, and drivers, apps and customizations from your device manufacturer, and changes you made in Settings. We recommend you read through these steps and make sure you're confident how to do them before you get started.

### Create installation media

1. Back up all your files and applications. A clean install will erase all of your files, settings, and applications.

2. [Download this tool](https://www.microsoft.com/software-download/windows10) and select **Run**. You need to be an administrator to run this tool.

3. If you agree to the license terms, select **Accept**.

4. On the **What do you want to do?** page, select **Create installation media for another PC**, and then select **Next**.

5. Select the language, edition, and architecture (64-bit or 32-bit) for Windows 10. 

6. Select which media you want to use:

- **ISO file.** Save an ISO file to your device, which can also be used to create a DVD. After the file is downloaded, you can go to where the file was saved, or select Open DVD burner, and follow the instructions to burn the file to a DVD.

- **USB flash drive.** Attach a blank USB flash drive with at least 8GB of space. Any content on the flash drive will be deleted.

### Using the ISO file you created

1. Open File Explorer and go to where you saved the ISO. Select the ISO file to open it, which lets Windows mount the image so you can access it.

2. Select the setup.exe file to launch the install process.

3. During setup, select the **Change what to keep** option, and then choose **Nothing** on the next screen to complete a clean intall.

4. Once it's finished installing, you can check for updates now by going to **[Settings > Update & Security > Windows Update](https://aka.ms/WIPWindowsUpdate)** and selecting **Check for updates**.

### Using the USB or DVD you created

1. Attach the USB flash drive or insert the DVD in the device where you want to install Windows 10.

2. Restart your device.

3. If your device does not automatically boot to the USB or DVD media, you might have to open a boot menu or change the boot order in your BIOS or UEFI settings. 

4. On the **Install Windows** page, select your language, time, and keyboard preferences, and then select **Next**.

5. Select Install Windows.

6. Once it's finished installing, you can check for updates now by going to **[Settings > Update & Security > Windows Update](https://aka.ms/WIPWindowsUpdate)** and selecting **Check for updates**.
