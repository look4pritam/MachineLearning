# VirtualBox

- Install virtualbox.

```sh
sudo apt-get update
sudo apt-get install virtualbox
```

- Install VirtualBox extension pack.

```sh
wget https://download.virtualbox.org/virtualbox/6.1.32/Oracle_VM_VirtualBox_Extension_Pack-6.1.32.vbox-extpack
sudo VBoxManage extpack install Oracle_VM_VirtualBox_Extension_Pack-6.1.32.vbox-extpack
```

# [VirtualBox - Shared Folders](https://gist.github.com/estorgio/0c76e29c0439e683caca694f338d4003)

- Create a shared folder 'installers'.
- Devices -> Insert Guest Additions CD image.
- Mount a CD drive.

```sh
sudo mkdir /media/cdrom
sudo mount -t iso9660 /dev/cdrom /media/cdrom
```

- Install dependencies for VirtualBox guest additions.

```sh
sudo apt-get update
sudo apt-get install -y build-essential linux-headers-`uname -r`
```

- Run the installation script for the guest additions.

```sh
sudo /media/cdrom/./VBoxLinuxAdditions.run
```

- Add current user to 'vboxsf' group.

```sh
sudo usermod -aG vboxsf $(whoami)
```
