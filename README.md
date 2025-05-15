# System Hacking – Gaining and Maintaining Access 

**We need these:**  
Attacker Machine (example Kali Linux)  
Target Machine (example Metasploitable 2)  
Tools: Metasploit Framework, Nmap, Netcat, Hydra (for optional password cracking)  

In this repository, we will do some scanning operations, exploiting a vulnerable service, post-exploitation enumeration, privilage exploitation, creating a persistent backdoor and at the end, will clean up everything.  

## Basic system hacking  

**Step 1: Host Discovery & Scanning**  
We firstly find the target ip.  
![ifconfig](images/configuration.png)  
We check the open ports and service versions.  
![sv](images/sv-scan.png)  
**Step 2: Exploiting**  
We cause to start Metasploit in Kali Linux.  
![metasploit](images/metasploit.png)  
We find weak service.  
![weak](images/vsftpd.png)  
![weak](images/options.png)  
![exploiting](images/exploit.png)  
We get shell.  
![shell](images/shell.png)  
**Step 3: Post-exploitation**  
We look at to users.  
![users](images/users.png)  
Configuration the network:  
![configure](images/configuration.png)  
We look through some files.  
![look](images/find.png)  
**Step 4: Privilege Escalation**  
Avtomatic checking  
![avtomatic](images/avtomatik_yoxlama.png)  
Suid files  
![suid](images/suid-files.png)  
We use exploit  
![exploit](images/dirty_cow.png)  
**Step 5: Persistence**  
Adding user  
![user](images/new-user.png)  
Entrancing with ssh  
![ssh](images/ssh.png)  
**Step 6: Cover Tracks**  
Deleting bash history  
![deleting](images/deleting.png)  
Deleting the log files  
![logs](images/deleting_logs.png)  
Changing the date  
![date](images/date.png)  


