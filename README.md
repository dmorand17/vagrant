# vagrant
Vagrant configuration files

# Prerequisites

VM is needed to run windows

[Virtual Box](https://www.virtualbox.org/wiki/Downloads) 
```bash
brew install --cask virtualbox
```

[Vagrant](https://www.vagrantup.com/downloads)
```bash
brew install --cask vagrant
```

# Starting the VM

We must first [tell VirtualBox it's fine to use the ports we assigned](https://www.virtualbox.org/manual/ch06.html#network_hostonly):

```bash
sudo mkdir /etc/vbox
sudo touch /etc/vbox/networks.conf
# add `* 33.33.33.0/24` to that file
```

The default windows user and password are both `vagrant`.

## VirtualBox settings
* Change Display to 200% to fix resolution issues
