git-vagrant-box
===============

Vagrant Box for the Global Git Repository Boilerplate

INSTRUCTIONS
------------

1. Choose your base box folder (e.g. centos-6.5).
2. Download the base OS ISO from the link in base_image.url.
3. Create a new machine in VirtualBox
4. Name the machine 'unit9-{box-name}', e.g. 'unit9-centos-6.5'.
5. Leave all settings to default except the max disk size. Set it to 20 GB.
6. Mount the downloaded ISO and install it on the machine.
7. Set the root password to 'vagrant'.
8. Log in to the virtual machine with a superuser.
9. Mount Guest Additions in VirtualBox
10. Manually type / execute the setup_network script.
11. run:
cd /tmp
curl -L https://raw.githubusercontent.com/unit9/git-vagrant-box/develop/centos-6.5/bootstrap > bootstrap
chmod +x bootstrap
./bootstrap
12. Power off the machine.
13. Build the Vagrant box for that machine by running `./build`.