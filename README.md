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

