
# Source

https://wiki.archlinux.org/index.php/Sudo#Configuration

# Add a username to sudoer's group 

usermod -aG sudo username

# Run  to print out the current sudo configuration, or sudo -lU user for a specific user.

sudo -ll 

sudo -lU 
Add <username> to a group: sudo usermod -aG sudo esa
