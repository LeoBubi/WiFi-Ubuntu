# WiFi-Ubuntu

All the packages needed to enable WiFi on Ubuntu, after having it installed on an Intel Mac.

1. sudo apt-get purge bcmwl-kernel-source

2. Download 'http://archive.ubuntu.com/ubuntu/pool/main/b/b43-fwcutter/b43-fwcutter_019-11build1_amd64.deb'

3. Download 'http://lwfinger.com/b43-firmware/broadcom-wl-5.100.138.tar.bz2'

4. Run in terminal:
	
	- sudo dpkg -i b43-fwcutter_019-11build1_amd64.deb
	- tar xfvj broadcom-wl-5.100.138.tar.bz2 
	- sudo b43-fwcutter -w /lib/firmware broadcom-wl-5.100.138/linux/wl-apsta.o

5. Run 'sudo modprobe b43'

6. Reboot

7. Move into the folder with all the deb packages

8. Run 'sudo dpkg -i *.deb'

9. Reboot and that's it!

