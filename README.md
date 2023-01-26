# H1-First Step
This is the homework for the course Information Security by Tero Karvinen.
Using Hauwei Laptop and Macbook Air for this course. 
```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```

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
ssh
ls
cat
exit
```
- The home directory only have dash file. 

- <img width="168" alt="image" src="https://user-images.githubusercontent.com/95883827/214847411-d1a2ab51-fc2a-44d1-ae31-f330539dd7ea.png">

- Use this link could hlep you understand [WebServerTalk](https://www.webservertalk.com/dashed-filename).
- Used ```cat``` to read the dashfile(-), now I can see the password for next level. :) 
- <img width="255" alt="image" src="https://user-images.githubusercontent.com/95883827/214848007-2249309c-b051-4d3a-8cfb-9584c19fd159.png">
- Now use ```exit``` command to exit from banit1. 


### LEVEL 2 -> LEVEL 3
The command I used for this level
```
ssh
ls
cat
exit
```
- Connected bandit2 with command ```ssh```to ```bandit2@bandit.labs.overthewire.org```
- <img width="592" alt="image" src="https://user-images.githubusercontent.com/95883827/214849535-1cee0475-40e3-4511-8eb0-e840c9ed8925.png">
- Use command ```ls``` to find the password file. 
- Use ```cat``` command, and the terminal automatically help me to filled up the command with  ```->``` from keyboard.
- <img width="357" alt="image" src="https://user-images.githubusercontent.com/95883827/214849856-dec99db5-3d36-4800-9df3-cfec72389fd9.png">
- Exit from the bandit2 server. And going to the next level.


### LEVEL 3 -> LEVEL4
The command I used for this level
```
ssh
ls
cd
find
cat
exit
```
- Used ```ssh``` to connect to bandit3 
- <img width="559" alt="image" src="https://user-images.githubusercontent.com/95883827/214850661-c8134ed3-25c0-4a9d-952d-2357e2bb25b0.png">
- Used ```ls``` to find the inhere directory, and ```cd``` go to ```inhere```, and then used ```ls```, there is empty. Then I used ```find``` to search for files in a directory hierarchy   ,so that I can see what kind of the file inside this directory. 
- <img width="231" alt="image" src="https://user-images.githubusercontent.com/95883827/214851510-cf84d6df-1404-4d62-a392-3015e75c9230.png">

- NOTE: if I used ```cd``` then it will look like this, that's why i used ```find``` to know what is the hidden file. 
  ```
  bandit3@bandit:~$ cat inhere/
  cat: inhere/: Is a directory
  ```
- So I google the solution to read the hidden file. Use this link could hlep you understand [Medium.com](https://medium.com/@theGirlWhoEncrypts/overthewire-bandit-level-3-level-4-ab55bcdcff36).
- Used ```ls -a``` to list all hidden dot files  the and then used ```cat``` to read the hidden file.
- <img width="287" alt="image" src="https://user-images.githubusercontent.com/95883827/214853386-c386bb15-5663-4bc8-a46e-d110a1d17e4c.png">
- Exit from the bandit3 server. 


### LEVEL 4 -> LEVEL 5
The command I used for this level
```
ssh
ls
ls -larth
cd
find
file
cat
exit
```
- Used ```ssh``` to connect bandit4.
- <img width="579" alt="image" src="https://user-images.githubusercontent.com/95883827/214854675-1d7ed8c8-ec89-400b-91cc-26d4ad0639d9.png">
- In this game, I used the command as follow to know the details.
- <img width="638" alt="image" src="https://user-images.githubusercontent.com/95883827/214855094-20188131-572b-4c8b-af38-1b67549f9c7e.png">
- Used command ```file```  ```file ./inhere/*````to determine the file type.
- <img width="263" alt="image" src="https://user-images.githubusercontent.com/95883827/214855415-f22ea17b-460c-4ab7-a79b-3b2a25457d57.png">
- Then use ```cat``` to read this human-readble file which is ```-file07```
- <img width="289" alt="image" src="https://user-images.githubusercontent.com/95883827/214855562-69c2cb12-c3d0-4015-955d-98de6953c7ae.png">
- Exit from the bandit4 server. 

> This is very interesting game and it's very partical to know which command to search what you want to know. I will play more later. :) 


## Bullseye
### Error before working on Debain.
When I was following the instruction by Tero, I couldn't install any Debain in my laptop. The problem is that I couldn't choose to Live when i installed the Debian GNU/Linux Live.
Now I am installing the Debian installer. Evrything on the process. Not so sure can I install this? 

Update:
Now I could log in after installed the Debian Installer.
 ![Add file: Upload](https://github.com/zhiqingff/h1-First_step/blob/main/Screenshot%202023-01-24%20201132.png)

I couldn't use sudo command. 
 ![Add file: Upload](https://github.com/zhiqingff/h1-First_step/blob/main/Screenshot%202023-01-24%20200746.png)

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
