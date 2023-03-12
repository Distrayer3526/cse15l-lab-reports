# Writing a `bash` script for lab report 4
While doing the competition in class, it never occured to me that being able to edit the `ListExamples.java` file in the terminal (without having to open `vim` or `nano`) would make our time that much faster. The team who ended up winning the competition in our lab did exactly that and were able to get a time under 10 sec. So to do lab report 4 in a different way I first researched how to edit files directly from the terminal. 

## `SED`
One way I found to do this was the `SED` command. It is mostly used for searching, find and replace, or insertion and deletion. For this lab, I needed to replace a certain line so this was perfect for me. I needed to edit the line 43 and rewrite it directly to the file so after reading the documentation I was able to make the command that I needed: `sed -i '43 s/index1 += 1/index2 += 1/' ListExamples.java`. The `-i` parameter tells `SED` to replace in place and the `43` specifies which line it is editing. The `s` stands for substitution, the `/` is a delimiter, `index1 += 1` is the stuff to be replaced, and `index2 += 1` is the string that should replace the old one. 

## Putting it in a `bash` file
The rest of the commands needed for this assignment could simply be put directly into the bash file. I did, however, make the CPATH variable to make it a bit easier if I had to switch between operating systems. The final `bash` script was:
![image](https://user-images.githubusercontent.com/62564887/224517510-f048b3c4-ea24-4f99-a179-e8494c56384e.png)
