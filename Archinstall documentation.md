#### Installation:

> The installation process could fail due to the variety of computer hardware. If there is any problem, please contact me as soon as possible to solve it.

After the ISO has been booted up, the terminal will launch automatically. Some features cannot work in a live environment, such as the status bar(waybar), but it will after the OS is installed.

First you need to connect to a network. If you want to use Wi-Fi, use the command
`nmtui` 
and connect.

> The password for the hyprland user: kietvo17112003

1. Inside the terminal, type in 
	`sudo archinstall --config faisal.json`
	This will launch the installation script. 
2. **Archinstall language**: Choose the language you prefer.
3. **Mirrors** -> Mirror region: Choose your region, this will affect the package download process in pacman.
	-> Back
4. **Locale**: Skip
5. **Disk configuration** -> Use a best-effort default partition layout
	-> Choose your disk: Choose nvme0n1
	-> Select which file system your main partition should be: Ext4
	-> Would you like to create separate partition for home?: No
6. **Disk encryption**: Skip
7. **Bootloader**: Skip (already configured)
8. **Unified kernel images**: Skip (already configured)
9. **Swap**: Skip (already configured)
10. **Host name**: Your computer name (Default is Faisal, you can change it if you want)
11. **Root password**: You have to set the password for your root.
12. **User account** -> Add a user
	-> Username
	-> Password
	-> Re-enter the password
	-> Should you be a superuser?: Yes
	-> Confirm and exit
13. **Profile**: Skip
14. **Audio** -> Pulseaudio
15. **Kernel**: Skip
16. **Additional packages**: *Must be skipped, don't touch it*
17. **Network configuration** -> Use Network Manager
18. **Timezone**: Choose your time zone
19. **Automatic time sync**: Skip
20. **Optional Repositories**: Skip

-> **Install**. After the script launches, there will be a prompt that says press enter to proceed. Wait for the installation process completed.

In the end, there will be a prompt that asks if you want to get into the chroot environment, choose no, unplug the USB, and restart the machine into the fresh Archlinux with Hyprland environment.

#### Post-installation:
>If there is any issue with the status bar, the terminal, ... Please contact me as soon as possible to resolve it.

**Network configuration**: There will be a network icon on the left side of status bar, you can use it to interact with network manager.

**Screen sharing**: Install pipewire and wireplumber, everything else has been configured
`sudo pacman -S pipewire wireplumber`
#### Key binding:

*Meta*: The Windows key

**Application launcher**: Meta + d
**Terminal**: Meta + Enter
**Power menu**: Meta + x
**Screen shot**: Meta + s

**Kill window**: Meta + Shift + q
**Toggle full screen**: Meta + F
**Toggle floating**: Meta + Space
**Move between workspaces**: Meta + 1, 2, 3, 4, 5, 6 or using 3 fingers swipe gesture on the touchpad.
**Send window to workspace**: Meta + Shift + 1, 2, 3, 4, 5, 6
**Move window**: Hold Meta key and use left mouse button
**Resize window**: Hold Meta key and use right mouse button