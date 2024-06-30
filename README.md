<img align="right" width=20% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Big%20Hedge/Assets.xcassets/AppIcon.appiconset/512.png?raw=true">

# Big Hedge Patcher
Big Hedge is an easy-to-use tool that allows anyone to install macOS 11 Big Sur on unsupported Macs.

<br><img width="480" src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/mainwindow.png?raw=true"><br>

## Background
Big Hedge, originally known as [MicropatcherAutomator](https://github.com/moosethegoose2213/automator-for-barrykn-micropatcher), is a project that I co-created with 
[AsentientHedgehog](https://github.com/moosethegoose2213) to provide a user-friendly UI for his automation script back in late 2020.

We later renamed the tool to Big Hedge and introduced numerous new features, including the ability to create ISO/DMG images
of the patched macOS 11 Installer and upgrade to macOS 11 directly without a bootable USB. However, it never reached a formal release,
so I decided to publish the unreleased source code of Big Hedge to my GitHub for archival purpose.

Also, I would recommend using [OpenCore Legacy Patcher](https://github.com/dortania/OpenCore-Legacy-Patcher) for installing
macOS 11 or later on unsupported Macs, as both Big Hedge and MicropatcherAutomator are no longer maintained.

## Supported Models

To check your hardware model, open System Information and look for the `Model Identifier` key.

<details>
  <summary>2012 and Early 2013 MacBook Pro</summary>
  <ul>
    <li>MacBookPro9,x</li>
    <li>MacBookPro10,x</li>
  </ul>
</details>

<details>
  <summary>2012 MacBook Air</summary>
  <ul>
    <li>MacBookAir5,x</li>
  </ul>
</details>

<details>
  <summary>2012 and 2013 iMac</summary>
  <ul>
    <li>iMac13,x</li>
    <li>iMac14,x</li>
  </ul>
</details>

<details>
  <summary>2012 Mac mini</summary>
  <ul>
    <li>Macmini6,x</li>
  </ul>
</details>

> [!WARNING]  
> If your Mac is not listed here, it is either unsupported by Big Hedge or lacks graphics acceleration on macOS Big Sur.
> 
> Running macOS Big Sur without graphics acceleration will result in extremely poor performance.

## Instructions

> [!IMPORTANT]  
> Remember to **backup your Mac** before upgrading.
> 
> Also, you must **turn FireVault OFF** before using Big Hedge. Detailed instructions can be found [here](https://support.apple.com/en-vn/guide/mac-help/mchlp2560/10.15/mac/10.15).

To begin, download the latest version of Big Hedge from the following link:
[Big_Hedge.zip](https://github.com/minh-ton/Big-Hedge-Patcher/releases/latest/download/Big_Hedge.zip).

Once the download is complete, open the application.

<br>
<div align="center">
  <img width="480" src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/mainwindow.png?raw=true">
</div>
<br>

Continue to proceed to the `macOS Big Sur Installer App` page.

<br>
<div align="center">
  <img width="480" src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/installer_app_0.png?raw=true">
</div>
<br>

On this page, you can choose to either browse for an existing installer or download a new copy of the macOS Big Sur Installer.

<br>
<div align="center">
  <table width="100%">
    <tr>
      <th width="50%">Browse for the Installer App</th>
      <th width="50%">Download Installer App</th>
    </tr>
    <tr>
      <td align="center" width="50%">
        <br><p>To use a pre-downloaded macOS Big Sur Installer, select the installer app and click <b>Open</b>.</p>
        <br><img src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/browse_installer_finder.png?raw=true">
        <br><br><p>After selecting the installer, click <b>Continue</b> to proceed to the next step.</p>
        <img src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/browse_installer_ok.png?raw=true">
      </td>
      <td align="center" width="50%">
        <br><p>Click <b>Continue</b> and enter your user password to start the download.</p>
        <br><img src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/download_installer_1.png?raw=true">
        <br><br><p>The download may take some time to complete. Once done, click <b>Yes</b> to use the downloaded installer.</p>
        <img src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/download_installer_3.png?raw=true">
      </td>
    </tr>
  </table>
</div>
<br>

On the next page, you will see three different methods to install macOS Big Sur on your unsupported Mac.

<br>
<div align=center>
  <img width="480" src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/installation_method_0.png?raw=true">
</div>
<br>

---

### A. Create a Bootable Installer (Recommended)

> [!NOTE]
> This option is only available if you're running Big Hedge on macOS 10.13 High Sierra or later.

#### 1. Create the USB Installer

Obtain a USB drive with **at least 16GB of storage**. Use Disk Utility to format the USB drive as `Mac OS Extended (Journaled)` with the `GUID Partition Map` scheme using the instructions found [here](https://support.apple.com/en-vn/guide/disk-utility/dskutl14079/22..6/mac/14.0).

> [!CAUTION]
> The entire USB drive will be formatted. Remember to back up your files.

Choose your USB drive from the dropdown menu in Big Hedge. If your USB drive is not listed,  the Refresh icon.
<br>
<div align=center width=100%>
<img width=45% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/create_bootable_0.png?raw=true"> <img width=45% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/create_bootable_1.png?raw=true">
</div>
<br>

Continue to proceed to the `Create Bootable Installer` page.

<br>
<div align=center width=100%>
<img width=45% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/create_bootable_2.png?raw=true"> <img width=45% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/create_bootable_3.png?raw=true">
</div>
<br>

Continue with the process and enter your user password when prompted.

<br>
<div align=center width=100%>
<img width=45% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/create_bootable_5.png?raw=true"> <img width=45% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/create_bootable_6.png?raw=true">
</div>
<br>

This process will take several minutes to complete. If successful, you should see the following screen:

<br>
<div align=center>
  <img width="480" src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/create_bootable_success.png?raw=true">
</div>
<br>

#### 2. Install macOS Big Sur

You will need to restart your Mac and boot while holding the Option key. You should see the startup screen:

<br>
<div align=center>
  <img width="600" src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/boot_picker_0.png?raw=true">
</div>
<br>

First, select `EFI Boot`. Once you do this, your Mac will immediately power off.
If you skip this step, you will see a forbidden sign at boot.

Hold the Option key while powering on your Mac again. This time, select `Install macOS Big Sur` to boot from the USB Installer.

<br>
<div align=center>
  <img width="600" src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/boot_picker_1.png?raw=true">
</div>
<br>

Once booted into the Installer, select `Install macOS Big Sur` and follow the on-screen instructions to install macOS Big Sur.
You may want to reformat your internal drive using Disk Utility beforehand, or continue with the installation if you just want to upgrade macOS.

<br>
<div align=center width=100%>
<img width=45% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/recovery_view_0.png?raw=true"> <img width=45% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/install_macos_view.png?raw=true">
</div>
<br>

After the installation is completed, follow the on-screen instructions to set up macOS Big Sur.

#### 3. Apply Post-Install Patches

You will need to restart your Mac and boot while holding the Option key. Then select `Install macOS Big Sur` to boot from the USB Drive.

<br>
<div align=center>
  <img width="600" src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/recovery_view_1.png?raw=true">
</div>
<br>

In the Recovery menu, select `Post-Install Automator` and click **Continue**.

<br>
<div align=center>
  <img width="600" src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/postautomator_view.png?raw=true">
</div>
<br>

Select the drive where you installed macOS Big Sur from the dropdown menu.
Then click **Continue** to install patches to the macOS Big Sur installation.

When complete, restart your Mac to finalize the installation.

---

### B. Install to Machine

#### 1. Bypass Compatibility Checks

Big Hedge will first check your machine for issues.

<br>
<div align=center width=100%>
<img width=45% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/install_to_machine_0.png?raw=true"> <img width=45% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/install_to_machine_ok.png?raw=true">
</div>
<br>

> [!NOTE]  
> The instructions for disabling SIP and FireVault can be found [here](https://developer.apple.com/documentation/security/disabling_and_enabling_system_integrity_protection) and [here](https://support.apple.com/en-vn/guide/mac-help/mchlp2560/10.15/mac/10.15).

Continue with the process and enter your user password when prompted.

<br>
<div align=center width=100%>
<img width=45% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/install_to_machine_starting.png?raw=true"> <img width=45% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/install_to_machine_2.png?raw=true">
</div>
<br>

Once done, click **Launch Installer** to open the macOS Big Sur Installer.
Follow the on-screen instructions to install macOS Big Sur.

<br>
<div align=center>
  <img width="480" src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/install_to_machine_success.png?raw=true">
</div>
<br>

#### 2. Apply Post-Install Patches

After the installation is completed, reopen Big Hedge. On the menubar, select `Post Installation > Apply Post-Install Patches` to launch the PostAutomator app.

<br>
<div align=center>
  <img width="480" src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/install_to_machine_menu.png?raw=true">
</div>
<div align=center>
  <img width="480" src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/post_install.png?raw=true">
</div>
<br>

Select the drive where you installed macOS Big Sur from the dropdown menu.
Then click **Continue** to install patches to the macOS Big Sur installation.

When complete, restart your Mac to complete the installation.

---

### C. Create a Disk Image

> [!NOTE]
> This option is only available if you're running Big Hedge on macOS 10.13 High Sierra or later.

You will need to choose the format of the disk image, either ISO or DMG.

<br>
<div align=center width=100%>
<img width=45% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/create_image_0.png?raw=true"> <img width=45% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/create_image_1.png?raw=true">
</div>
<br>

Click **Continue** and browse for the location to save the output disk image.

<br>
<div align=center>
  <img width="480" src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/create_image_2.png?raw=true">
</div>
<br>

Continue with the process and enter your user password when prompted.

<br>
<div align=center width=100%>
<img width=45% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/create_image_4.png?raw=true"> <img width=45% src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/create_image_5.png?raw=true">
</div>
<br>

Once done, you can use the disk image to restore to a USB/CD/DVD drive using [Disk Utility](https://support.apple.com/en-vn/guide/disk-utility/dskutl14062/mac) (macOS), [TransMac](https://www.acutesystems.com/scrtm.htm) (Windows), or [BackToMac](https://git.datcuandrei.com/datcuandrei/BackToMac) (Linux).

<br>
<div align=center>
  <img width="480" src="https://github.com/minh-ton/Big-Hedge-Patcher/blob/main/Screenshots/create_image_success.png?raw=true">
</div>
<br>

## Credits
Big Hedge is based on the [big-sur-micropatcher](https://github.com/barrykn/big-sur-micropatcher), so none of this would be possible without [BarryKN](https://github.com/barrykn) and his amazing work.

Also, special thanks to [ASentientHedgehog](https://github.com/moosethegoose2213) for inviting me to this great project, as well as [BenSova](https://github.com/Ben216k), [ASentientBot](https://asentientbot.github.io), [jackluke](https://forums.macrumors.com/members/jackluke.1133911), and many others for their help in developing this tool.

## License
This project is licensed under the GPL-3.0 License.
