#                                  Preview
OldBIOS
![Image](https://github.com/user-attachments/assets/6d926d8a-0149-4faa-a52e-d95e51893af7)
CrossGRUB
![Image](https://github.com/user-attachments/assets/abf33b9e-1afc-459d-939c-33fe917935a8)
Navi
![Image](https://github.com/user-attachments/assets/116fcfa8-9433-4418-843b-578341c37152)
Wuthering Weilinai
![Image](https://github.com/user-attachments/assets/f6a9d41a-eafe-4eff-a344-678ea8ece33e)
Cybervero
![Image](https://github.com/user-attachments/assets/99af57f8-05fe-40fd-9724-01160c303a9c)
#                                  Tutorial
To use these themes on your GRand Unified Bootloader (more commonly known as GRUB), the tutorial is right here.
1. Download the themes you would like to apply (Wuthering Weilinai, OldBIOS etc.)
2. Open the terminal and CD to the directory where the downloads are.
3. Unzip the files with the unzip tool (if you dont have it installed install it with your package manager: sudo apt install unzip)
4. Copy the theme files to /usr/share/grub/themes with root privileges like this: sudo cp -r your-theme/ /usr/share/grub/themes
5. Edit your grub config with a text editor (either NANO or gedit) with root privileges too, the config is located in /etc/default/grub (sudo nano/gedit /etc/default/grub)
6. Scroll all the way down till you see "GRUB_THEME=/path/to/theme".
7. Change "/path/to/theme" with "/usr/share/grub/themes/your-theme/theme.txt"
8. Press CTRL+O, Y and then CTRL+X (with NANO, on gedit you just press CTRL+S)
9. Update GRUB with sudo update-grub or sudo grub-mkconfig -o /boot/grub/grub.cfg
10. Reboot and you will see your theme!
