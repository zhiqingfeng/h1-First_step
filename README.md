# H1-First Step
This is the homework for the course Information Security by Tero Karvinen.
Using Hauwei Laptop and Macbook Air for this course. 

## Bandit oh-five (LEVEL 0-4) 
### LEVLE 0 
The command I used for this level
```
ssh
```
- In this level, I need to use ```ssh``` command to connect the ```bandit.labs.overthewire.org```
<img width="629" alt="image" src="https://user-images.githubusercontent.com/95883827/214844049-3f3b6600-8f1f-4827-b7f3-c200eb3b6b9f.png">

### LEVEL 0 -> LEVEL 1
The command I used for this level
```
ls
less
exit
```

- Use ```less``` command to check the password from the home directory. 
<img width="390" alt="image" src="https://user-images.githubusercontent.com/95883827/214844542-3bde48bf-0e74-4719-ba62-2c75dced7f5a.png">

- Use ```exit``` from the bandit0 server.
- Logged in to bandit1 successfully with the password which copied from bandit0.
<img width="587" alt="image" src="https://user-images.githubusercontent.com/95883827/214845358-c14ba0b8-3de2-42da-98cc-fa330907e6cd.png">


### LEVEL 1 -> LEVEL 2
The command I used for this level
```
ls
less
exit
```
- The home directory only have dash file. 
  <img width="168" alt="image" src="https://user-images.githubusercontent.com/95883827/214847411-d1a2ab51-fc2a-44d1-ae31-f330539dd7ea.png">
  Use this link could hlep you understand [WebServerTalk](https://www.webservertalk.com/dashed-filename).
- 
## Bullseye
### Error before working on Debain.
Here have a problem that I couldn't choose to Live when i installed the Debian GNU/Linux Live.
Now I am installing the Debian installer. Evrything on the process. Not so sure can I install this? 

Update:
Now I could log in after installed the Debian Installer.
 ![Add file: Upload](Screenshot 2023-01-24 200746.png)

I couldn't use sudo command. 
 ![Add file: Upload](Screenshot 2023-01-24 201132.png)

I think this casued by i installed the Debian installer but not Debian GNU/Linux live.

### START OVER
Step 1: 
- Installed the VirtualBox on Macbook, and created a new Virtual Machine. 
Setp 2:
- Started the app, choosed Debian GNU/Linux Live (kernel 5.10.0-20amd64)
- It didnt work again, so I installed the Debian Installer again on Macbook.

### START OVER AGAIN
Step 1:
Go back to Windows laptop and log in the application.
Step 2:
I typed sudo apt-get update.But there displayed my username is not in the sudoers file. This incident will be reported. 
Now looking for the root reason of this issue. :( 


### UPDATE -- FINAL VERSION
1. installed the UPM and logged in Debian successfully. :) (So I am doing everything in DebainLinuxBullsEye) 

## WebGoat
1. Installed and Ran WebGoat. But I couldn't run the java command --> (bash:java:command not found) 
2. Looking for the solution about java command. 
3. Installed Java and Javac, and now it's available to use java command and registered on WebGoat successfully. :) 
## Hacker warmup

   1) General: HTTP Basics
     - Entered my name and press GO!. 
     - Magic number is 71. Found it from the HTML by searched the keyword.
   3) General: Developer tools
     - PhoneHome response is 807131848
     - networkNum: 14.930557891802575
## Sources

Tasks: [Tero-Karvinen_h1_first-steps](https://terokarvinen.com/2023/information-security-2023/?f=moodle#h1-first-steps)

Lectures:

[Hutchins et al 2011: Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains](https://lockheedmartin.com/content/dam/lockheed-martin/rms/documents/cyber/LM-White-Paper-Intel-Driven-Defense.pdf)

[Karvinen 2020: Command Line Basics Revisited](https://terokarvinen.com/2020/command-line-basics-revisited/)

[OverTheWire: Bandit](https://overthewire.org/wargames/bandit/)

[SelfTaughtDev: OverTheWire Bandit Walkthrough | How To Pass Level 0 & 1, a YouTube video](https://youtu.be/2wozdVl3psY)

[Hitesh J 2020: Dashed Filename – Learn How to Create, Remove, List, Read & Copy!](https://www.webservertalk.com/dashed-filename)

[MayADevBe blog 2021: OverTheWire Bandit Level 4 -> 5 - Walkthrough (SPOILER ALERT)](https://mayadevbe.me/posts/overthewire/bandit/level5/)

[Karvinen 2006: Raportin kirjoittaminen (in Finnish)](https://terokarvinen.com/2006/raportin-kirjoittaminen-4/)

[VirtualBox Download page](https://www.virtualbox.org/wiki/Downloads)

[Karvinen 2021: Install Debian on VirtualBox](https://terokarvinen.com/2021/install-debian-on-virtualbox/)

[Meurya 2021: Install Debian 11 Bullseye on VirtualBox](https://www.how2shout.com/linux/install-debian-11-bullseye-on-virtualbox/)

[User tomboi 2021: E: Package 'ufw' has no installation candidate on Debian Linux](https://www.nixcraft.com/t/e-package-ufw-has-no-installation-candidate-on-debian-linux/3726)

[User Omar 2020: Package ufw is not available, but is referred to by another package](https://unix.stackexchange.com/questions/596035/package-ufw-is-not-available-but-is-referred-to-by-another-package)
