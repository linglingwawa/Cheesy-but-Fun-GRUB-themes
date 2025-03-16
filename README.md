To use these themes on your GRand Unified Bootloader (more commonly known as GRUB), the tutorial is right here.
1. Download the themes you would like to apply (Wuthering Weilinai, Grand Theft Auto etc.)
2. Open the terminal and CD to the directory where the downloads are.
3. Unzip the files with the unzip tool (if you dont have it installed install it with your package manager: sudo apt install unzip)
4. Copy the theme files to /usr/share/grub/themes with root privileges like this: sudo cp -r your-theme/ /usr/share/grub/themes
5. Edit your grub config with a text editor (either NANO or gedit) with root privileges too, the config is located in /etc/default/grub (sudo nano/gedit /etc/default/grub)
6. Scroll all the way down till you see "GRUB_THEME=/path/to/theme".
7. Change "/path/to/theme" with "/usr/share/grub/themes/your-theme/theme.txt"
8. Press CTRL+O, Y and then CTRL+X
9. Update GRUB with sudo update-grub or sudo grub-mkconfig -o /boot/grub/grub.cfg
10. Reboot and you will see your theme!
