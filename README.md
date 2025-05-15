# System Hacking – Gaining and Maintaining Access 

**We need these:**  
Attacker Machine (example Kali Linux)  
Target Machine (example Metasploitable 2)  
Tools: Metasploit Framework, Nmap, Netcat, Hydra (for optional password cracking)  

In this repository, we will do some scanning operations, exploiting a vulnerable service, post-exploitation enumeration, privilage exploitation, creating a persistent backdoor and at the end, will clean up everything.  

## Basic system hacking  

**Step 1: Host Discovery & Scanning**
We firstly find the target ip.  
![ifconfig](configuration.png)  
We check the open ports and service versions.  
![sv](sv-scan.png)  
**Step 2: Exploiting**
We cause to start Metasploit in Kali Linux.  
![metasploit](metasploit.png)  
We find weak service.  
![weak](vsftpd.png)  
![weak](options.png)  
![exploiting](exploit.png)  
We get shell.  
![shell](shell.png)  
**Step 3: Post-exploitation**  
We look at to users.  
![users](users.png)  
Configuration the network:  
![configure](configuration.png)  
We look through some files.  
![look](find.png)  
**Step 4: Privilege Escalation**  
Avtomatic checking  
![avtomatic](avtomatik_yoxlama.png)  
Suid files
![suid](suid-files.png)  
We use exploit  
![exploit](dirty_cow.png)  
**Step 5: Persistence**
Adding user  
![user](new-user.png)  
Entrancing with ssh  
![ssh](ssh.png)  
**Step 6: Cover Tracks**  
Deleting bash history  
![deleting](deleting.png)  
Deleting the log files  
![logs](deleting_logs.png)  
Changing the date  
![date](date.png)


