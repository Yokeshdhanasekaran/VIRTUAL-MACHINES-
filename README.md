# VIRTUAL-MACHINES-
EX 6: MOVING FILES BETWEEN VIRTUAL MACHINES

Aim:
To move the files between virtual machine.
 You can move files between virtual machines in several ways:
•	You can copy files using network utilities as you would between physical computers on your network. To do this between two virtual machine:
•	Both virtual machines must be configured to allow access to your network.
•	Any of the networking methods (host-only, bridged and NAT) are appropriate. 
•	With host-only networking, you copy files from the virtual machines to the host and vice-versa, since host-only networking only allows the virtual machines see your host computer.
•	With bridged networking or NAT enabled, you can copy files across your network between the virtual machines.
•	You can create a shared drive, either a virtual disk or a raw partition, and mount the drive in each of the virtual machines.
Procedure:
		How to Enable File sharing in VirtualBox. 
Step 1. Install Guest Additions on the Guest machine. 
Step 2. Configure File Sharing on VirtualBox. 
 
Step 1. Install Guest Additions on the Guest machine. 
1. Start the Virtuabox Guest Machine (OS). 
2. From Oracle's VM VirtualBox main menu, select Devices > Install Guest Additions *

a. Open Windows Explorer
b. Double click at the "CD Drive (X:) VirtualBox Guest additions" to explore its contents.
		  
![image](https://github.com/user-attachments/assets/bce6709b-c2e0-4d7c-849b-611ebd3a5998)


C.Right click at "VBoxWindowsAdditions" application and from the pop-up menu, choose "Run as administrator".
 
![image](https://github.com/user-attachments/assets/9f7b04f5-22c9-42d1-8f22-bcebb4d4ec99)


3.Press Next and then follow the on screen instructions to complete the Guest Additions installation.
	 
![image](https://github.com/user-attachments/assets/4d688418-553a-41a0-8498-2c58e3df9a67)


4. When the setup is completed, choose Finish and restart the Virtuabox guest machine.
Step 2. Setup File Sharing on VirtualBox Guest Machine.
1. From VirtualBox menu click Devices and choose Shared Folders -> Shared Folder Settings.

![image](https://github.com/user-attachments/assets/85c28a14-32c5-4f7a-ac5c-9c3541bf7c5c)

2. Click the Add new shared folder icon.
 
![image](https://github.com/user-attachments/assets/1e45ad19-dcc6-459b-9744-ff88d6c3003e)


3. Click the drop-down arrow and select Other.
 
![image](https://github.com/user-attachments/assets/c68ec7b3-9b9c-4c6f-8d02-b9442b78b69e)

3. Locate and highlight (from the Host OS) the folder that you want to share between the VirtualBox Guest machine and the Host and click Select Folder. *
* Note: To make your life easier, create a new folder for the file sharing, on the Host OS and give it with a recognizable name. (e.g. "Public")
 
![image](https://github.com/user-attachments/assets/751b7a3f-732e-49f4-b39f-cdfbebe9cc55)


4. Now, in the 'Add Share' options, type a name (if you want) at the 'Folder Name box, click the Auto Mount and the Make Permanent checkboxes and click OK twice to close the Shared Folder Settings.
 
![image](https://github.com/user-attachments/assets/bab11beb-b819-45a4-b04f-4bd91e3309c6)


5. You 're done! To access the shared folder from the Guest OS, open Windows Explorer and under the 'Network locations' you should see a new network drive that corresponds to the shared folder on the Host OS.

Result:

Thus the virtual machine files are moved to another VM
