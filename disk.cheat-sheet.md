
# Misc 

   Show disk usage 
      du . -h 
  Show file system disk usage
     df -h:w

  Check details of usb stick
     sudo fdisk -l

  Copy a file to USB stick
     sudo dd bs=4M if=/path/to/myimage.iso of=/dev/sd[drive letter] status=progress oflag=sync
