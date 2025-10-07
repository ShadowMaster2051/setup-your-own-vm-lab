# Create a VM lab

## Your first VM lab
VM is running Ubuntu.
VM was determined to be non-functional likley due to corrupt driver. Boot failures and hangs occured along with slow-running apps when booted successfully. Attempted to install guest OS utilizing ISO image to no avail. Adjusted RAM allocations to same results. 
4 GB of RAM and a virtual hard disk value of 32GB was chosen for optimal performance according to specification.
Too much RAM could induce active swapping, wherein the VM moves data between its disk space and RAM, due to strain.
RAM was reduced to minimum of 2GB; boot issues persisted. 
Repairing and/or replacing the corrupted driver would enable it to work effectively. 

## Your second VM
VM is running Ubuntu. 
No issues seemingly upon installation; all was set up seemingly smoothly on Mac OS per instructions.
4 GB of RAM was added, as well as 32 GB to the hard disk for optimal performance. 
Increased RAM could lead to degradation in performance, active swapping (when the VM moves data between its disk space and RAM out of strain), and the VM possibly crashing. 
Encountered 'Temporary failure resolving 'ports.ubuntu.com'. Determined this is likely due to a DNS forwarding to proper DNS server. Added known DNS server using the prompt, 'echo "nameserver 8.8.8.8" | sudo tee /etc/resolv.conf > /dev/null' followed by, 'sudo apt-get update' resulting in a successful connection. 
OS failed to boot after entering 'reboot' command. Powered off VM, restarted pressing F2 to check BIOS settings. Attempted to reboot from UEFI Shell by first finding the hard disk file utilizing the 'map -r' command. No hard disk file was found. Due to this finding and the red bar across the turtle icon, it is likely the hard disk or driver is corrupt, much like the first virtual machine, disabling me from proceeding further.
