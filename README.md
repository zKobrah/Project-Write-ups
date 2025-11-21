<p align="center">
  <img src="https://freepngimg.com/convert-png/32023-lenovo-logo-transparent" width="300">
</p>
<p align="center">
  <strong> Lenovo Ideapad S145 - Slow start-up + Faulty Keyboard </strong>
</p>


# Synopsis
User submits a device that is experiencing slow start-ups and a faulty keyboard. User states that when attempting to log-in after initial boot, they are unable to input password due to the password box blinking rapidly.

--------

# Tools
- iFixit PC repair toolkit
- USB Keyboard

--------

# Process

Upon first inspection, I noticed that it seems as though the "Enter" key is being rapidly input; as if a ghost key is being held down. I reboot the device to check if this anomoly is able to be reproduced.
I perform a hard shut down of the device and hold the power button for 30 seconds to discharge any residual power.
Upon booting the device, the issue is replicated.

--------

Next, I shut the device down and reboot into BIOS/UEFI knowing if this issue is replicated here, it points to faulty hardware. Upon entering BIOS, the anomoly begins to happen again; its as though the "Enter" key is being held down and begins entering system settings immediately. With this knowledge, I power the device down.
From here I am certain that this is a hardware issue. After powering down the device, I gather my repair tools and begin to disassemble the laptop looking for the keyboard ribbon. I physically inspect the ribbon and am able to determine that it is correcly connected to the keyboard slot. I decide to disconnect the ribbon and reassemble the device. 
Once assembled, I boot the device. Once booted, the device is no longer inputting the "Enter" key. I decide to use a USB keyboard in order to run some diagnostics on the device while I wait for a replacement keyboard.

--------

Upon logging onto the device, I note that the startup is extremely sluggish. The user stated that they do not use this device very often and only use it when they store photos or use their Criquet. I begin to notice a large number of applications being loaded at start-up. I ask the user if the applications are necessary to have open during start-up and they advise that they aren't.
I open the Task Manager and navigate to Startup Apps, disabling all unnecessary applications.
Next I open the system settings and check for any Windows updates. The device immediately prompted that it was severly outdated and missing important security updates.
After checking for updates, 7 updates and one firmware update were available. I backed up the device and began downloading and installing the updates.
(It is important to note that this user is using Windows 10 and it is passed the support end date)
The updates installed are as follows:
- Windows Malicious Software Removal Tool (x64)
- 2025-10 Cumulative Update for .NET Framework 3.5, 4.8, and 4.81 for Windows 10 Version 22H2
- 2025-10 Update for Windows 10 Version 22H2
- Lenovo - System - 1.2.0.11
- 2023-10 Update for Windows 10 Version 22H2
- Microsoft .NET Framework 4.8.1 for Windows 10 Verion 22H2
- Realtek Superconductor Corp - USB - 10.0.18362.31260
- Lenovo Ltd - Firmware - 1.26.0.0

--------
