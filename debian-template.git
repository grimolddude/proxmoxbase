#!/bin/bash


# Install sudo
apt-get update
apt-get install -y sudo

# Add a user to the sudo group and add to sudoers file (replace 'dc' with the desired username)
useradd -m -s /bin/bash grim
usermod -aG sudo grim

# Disable su by changing the root shell
usermod -s /sbin/nologin root

# Disable root from SSH login
echo "PermitRootLogin no" >> /etc/ssh/sshd_config

# Restart SSH service to apply changes
service ssh restart

# Add user 'grim' to sudoers file
echo "dc ALL=(ALL:ALL) ALL" >> /etc/sudoers

echo "Setup complete. Make sure to test the SSH login with the user account before logging out as root."


# screen
apt install screen -y



