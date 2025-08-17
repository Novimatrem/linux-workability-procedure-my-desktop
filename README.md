# linux-workability-procedure-my-desktop

1. Install Xubuntu 25.04 as normal, ensuring that your install medium is of a reasonable speed, such as a USB memory stick. Do NOT use something as slow as a DVD.

2. You will reach a fatal error mid-install, "Something went wrong", clicking on "Show log" shows tons of grub-related errors.

3. Click Close, shut down the PC, remove the install medium (USB). Turn the machine back on, and boot from your Linux drive via BIOS/UEFI.

4. In grub, quickly select "Advanced options for Ubuntu", and then the (recovery mode) one.

5. Choose root - Drop to root shell prompt, then press Enter again.

6. ``sudo adduser zoey``

7. ``sudo adduser zoey sudo``

8. ``sudo reboot now``

9. Boot into the Linux drive normally, using the default Ubuntu selection in grub. Log in graphically to the account you just made.

10. You will have now reached a graphical Xubuntu 25.04 desktop, but BEWARE that the system is nowhere near completely ready, but this is a lot more comfortable and gives me a lot more to work with.

11. In case you haven't already, go into your BIOS/UEFI and set the Linux disk to be the first one, the highest priority, to boot automatically.

12. ``sudo dpkg --add-architecture i386``

13. ``wget https://cdn.akamai.steamstatic.com/client/installer/steam.deb``

14. ``sudo apt install -y gdebi``

15. ``sudo gdebi -n steam.deb``

16. Install Cyberpunk 2077 and see how well it works. (wait, follow the rest of this first)

17. Install Shadow Warrior 2013 and see how well it works. (wait, follow the rest of this first)

18. Run ``sudo nano /etc/apt/sources.list`` - comment out the cdrom line, and save the file.

19. ``sudo add-apt-repository ppa:obsproject/obs-studio``

20. ``sudo apt update``

21. ``sudo apt install -y obs-studio``

gpu best chances:

22. ``sudo add-apt-repository ppa:kisak/kisak-mesa``

23. ``sudo apt update -y``

24. ```sudo dpkg --configure -a && sudo apt-get -f install && sudo apt update -y && sudo apt upgrade -y && sudo apt full-upgrade -y && sudo apt autoremove -y && sudo apt autoclean -y && sudo apt clean -y && sudo dpkg --configure -a && sudo apt-get -f install && sudo snap refresh && sudo journalctl --flush && sudo journalctl --rotate && sudo journalctl --vacuum-time=1s && sudo journalctl --vacuum-size=200M && sudo journalctl --flush```

25. Reboot.

