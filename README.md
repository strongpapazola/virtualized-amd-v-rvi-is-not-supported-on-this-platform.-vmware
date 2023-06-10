https://communities.vmware.com/t5/VMware-Workstation-Pro/SOLVED-VM-not-working-on-Workstation-Pro-16-Intel-VT-x-Issue/td-p/2855709

I found the solution. Its a Windows 10 Home edition workaround.
Run the following command in CMD (open as "Run as Administrator") --- bcdedit /set hypervisorlaunchtype off
Once the command is executed, reboot the system.
This way VMware is able to set Virtualize Intel VT-X/EPT in VM settings.
You can follow the video on YouTube - https://www.youtube.com/watch?v=BTSYfjAgbZc 
