# First CSE15L lab report

## Setting up the CSE 15L account
First we had to go on UCSD's Educational Technology Servies webpage and reset our password
![image](https://user-images.githubusercontent.com/62564887/212569042-6d531119-4747-4119-a7bb-83b4f6973234.png)
* We had to find our CSE15L specific username
* We then had to use that username to do the account lookup
* Then we made a new password and waited 15 min

## Installing VS Code
I had already used VS Code in another class so I had that installed
![image](https://user-images.githubusercontent.com/62564887/212569236-e0da4127-9c64-46e5-9841-cfa116867f33.png)
* This is what you see when you open VS code for the first time
* Since I used it for CSE 12 I had my code from that class open first so I had to make a new window

## Setting up git
Git was something new so I had to go through the steps to get that set up in the terminal
![image](https://user-images.githubusercontent.com/62564887/212569290-24e2c6db-50f3-489a-9068-bcc89debcc20.png)
* In the .exe file I had to use all the defualt settings and it installed multiple applications on my computer
* One of my lab mates help me get familiar with git bash and link it up with this repo

## Remotely connecting
At this point I ran my first SSH command and after putting in my password I got this result
![image](https://user-images.githubusercontent.com/62564887/212569364-0d9e8f96-563f-4881-ab8d-b4a7d5f92e3b.png)
* The command I used to to this was as follows
* ```ssh cse15lwiadj@ieng6.ucsd.edu```
* It was interesting how the password doesn't show up when you type it

## Running some commands
To see if everything was running fine a ran some commands and luckily everything was working fine
Some of these commands were:
```
cd ..
ls
ls -l
ls -a
```
![image](https://user-images.githubusercontent.com/62564887/212569423-72f6a03c-d695-4f19-a9a8-f79330bcaca9.png)
* In the beginning, when I was only in my account I could only see the one visible file that is there by default in everyone's account which was per15
* I then ran the command ```ls -l``` to see a more detailed list of the files. I found that the default size of our accounts is 4096 bytes. 
* I also ran the ```ls -a``` command to see all the hidden files in my folder
* Finally, I used the ```cd ..``` command to go one step out of the current directory so I could see some information on all the other account that were using the same remote desktop
* I saw that there were 1448 such accounts and they were from different classes and were even created a couple years ago. 
* The oldest one I could see was from 2019


