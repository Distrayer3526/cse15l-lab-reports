### Step 1
First I made sure to delete my fork of the repository. Do that I had to type the repository location in my github account and press enter. 

![image](https://user-images.githubusercontent.com/62564887/221060171-d79c8d3a-1595-4bf4-97cf-22770c63bc7f.png)
### Step 2 
Next I fork the original repository again by pressing the fork button
![image](https://user-images.githubusercontent.com/62564887/221060336-e8d83544-e4d3-4c49-95ae-828a06844cb4.png)
### Step 4 
Once I am in my local terminal I can press <up> and the ssh command for my account appears. Since we set up the ssh key I don't have to type my password anymore to log in
  
![image](https://user-images.githubusercontent.com/62564887/221060885-387181bb-7727-43ed-bc8f-39bcfffa947e.png)
### Step 5 
To clone my repository I first get the ssh link from my fork. 
![image](https://user-images.githubusercontent.com/62564887/221061113-47a3f0f0-11ea-4ca5-872d-ee86a3c7a6b9.png)
Then I go in my remote terminal and type the command `git clone git@github.com:Distrayer3526/lab7.git<enter>`
  
![image](https://user-images.githubusercontent.com/62564887/221061295-c28ae89a-2d12-4685-a275-5d7ba44ed09d.png)
### Step 6 
To get the JUnit test commands I run `history | grep java<enter>` and then copy the specific command that I need. Then I run `cd l<tab><enter>` and run the respective commands
  
![image](https://user-images.githubusercontent.com/62564887/221061923-ff2844c2-a78d-4be9-b2bd-0bb1a2b0d4e5.png)
### Step 7
To fix the file I run `vim L<tab><enter>`, press `i`, go to the last while loop and change `index1` to `index2`, and then press `esc` and put `:wq<enter>` to save my changes
  
![image](https://user-images.githubusercontent.com/62564887/221062450-b2556b0b-2231-4d26-bad6-7352ea242db6.png)
### Step 8
Now since I recently ran the JUnit commands I press the up arrow 3 times to run javac and then 3 times again to run the java command
  
![image](https://user-images.githubusercontent.com/62564887/221062714-e49f8abe-36e5-45bc-8517-791bc254be69.png)
### Step 9
Then I run `git add L<tab>java<enter>`, `git commit -m "Update"<enter>`, and then `git push<enter>`
![image](https://user-images.githubusercontent.com/62564887/221063062-e4925420-96a5-4edf-9e4f-01a41fec4d4e.png)
