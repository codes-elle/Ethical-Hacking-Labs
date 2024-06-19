# Ethical-Hacking-Labs

## Question 1: Online Password Cracking (15 points):
I have demonstrated how to use Hydra to do online password guessing attack to obtain Metasploitable Linux VM’s user account password by using FTP login cracking.
(1). Run your Metasploitable 2 Linux VM, add a new user account of ‘newuser’ with the password of ‘computer’. Your answer should have screenshot image to show how you create such an account on this Linux VM.
 
(2). On your Kali Linux VM, run Hydra to do online password attack to the FTP service running on the Metasploitable 2 Linux VM, against the new account of ‘newuser’.  Please use the password list file (/usr/share/john/password.lst) for this attack after removing the comment lines in the beginning of this password list file.
       Please show the screenshot image of this hydra attack, which should find the correct password ‘computer’ within a dozen of tries  



## Question 2: (Metasploit attack to vulnerable Linux, 15 points)
I have demonstrated how to use Metasploit on Kali Linux to compromise the Metasploitable 2 Linux VM against the ‘vsftpd’ vulnerability. Please conduct a similar compromising attack to Metasploitable Linux VM against the ‘UnrealIRCd’ vulnerability.  You need to conduct this attack with the following requirements: (a). When compromising is successful, use the ‘reverse’ shell for the remote access;  (b). For the reverse connection of the shell, let the shell connect back to the Kali Linux VM on local port of ‘6666’;  (c). When the shell is successful generated, run the command ‘uname -a’ in the shell to confirm that you are running this command on the remote Metasploitable Linux VM machine.
   Please provide screenshot images to show all your operation commands, and the result of the successful attack with the result of the ‘uname -a’ command.

    
 
## Question 3: (Metasploit attack to WinXP, 15 points)
Set up your Kali Linux VM and your vulnerable WinXP VM ready. Make sure they can see each other. Then on Kali Linux VM, run Metasploit to attack the vulnerable WinXP by using the MS10-018 ‘drive-by download’ vulnerability with the following two requirements: First, payload uses the reverse-tcp meterpreter remote shell; Second, the malicious webserver running on local Kali Linux should work on the port 8888.
 (1). Use screenshot images to show how you use metasploit to successfully compromise your WinXP VM.
  
(2). Under the newly created meterpreter shell, display the compromised WinXP IP configuration, and then display its system information by use the ‘sysinfo’ command.
Please use screenshot images to show your operation commands and the attack results.
  


## Question 4: (Metasploit attack to WinXP, 20 points)
This time, you are required to run Metasploit to attack the vulnerable WinXP on the MS10-046 ‘drive-by download’ vulnerability. This attack has the following requirements: First, the attack payload used in the metasploit attack should give attacker the remote desktop control of the WinXP (i.e., vncinject payload); Second, you can use this remote desktop to remotely operate on the vulnerable WinXP (not just viewing); Third, this remote desktop control is using reverse-tcp mode.
(1). Use screenshot images to show how you use Metasploit to successfully compromise your WinXP VM.   

(2). Show the screenshot of the remote desktop window created on the Kali Linux derived from this metasploit attack.
  

## Question 5: (Offline Password Cracking, 15 points)
  I have created two accounts in Kali Linux, ‘final1’ and ‘final2’, and copied the /etc/shadow password file (only keeping the two accounts’ lines), which can be downloaded here ( shadow.txt Download shadow.txt).
  Please download this file to your Kali Linux VM, and use the John the Ripper offline password cracking tool to find out the passwords for these two accounts. Please use screenshot to show how you do it.
 


## Question 6: (Armitage Exploitation, 20 points)
Please run your Kali Linux VM, your vulnerable WinXP VM, and your metasploitable Linux VM at the same time. Make sure they can see each other and are in the same Virtual LAN.  If you have run Armitage on your Kali Linux VM before, please open Armitage, remove all hosts in the Armitage target window (menu "hosts"--> "clear database"), then restart your Armitage to do this assignment. Use screenshot images to demonstrate your testing.
(1). What are the IP addresses of your Kail Linux VM, the WinXP VM, and the Metasploitable 2 Linux VM?

(2). Run Armitage on your Kali Linux, then conduct nmap scan (OS detect) inside Armitage. Use screenshot image to show the Armitage interface where the target window section will only show the Metasploitable 2 Linux and the WinXP icons (after removing all other unrelated network devices). 
 
(3). After completing the above scanning process, you can either use ‘Hail Mary’ flooding attack to let Armitage conduct all possible attacks to the Metasploitable2 Linux and WinXP, and/or you can use individual attack module shown up on the host 'attack' menu to do attack. Make sure in the end, using whatever way, you can compromise both of these two vulnerable machines.  Use screenshot image to show the result showing that both VMs are compromised.
 
