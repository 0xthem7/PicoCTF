		``` Magikarp Ground Mission```

Description
Do you know how to move between directories and read files in the shell? 
Start the container, `ssh` to it, and then `ls` once connected to begin.
Login via `ssh` as `ctf-player` with the password, `6d448c9c`

Solution :

Step 1:
	Click the blue button ```Lunch Instance```
It will provide a ssh command ; copy it.
ssh ctf-player@venus.picoctf.net -p 59157

Step 2:
	Past the command in terminal 
	
	$ ssh ctf-player@venus.picoctf.net -p 59157
	Password is given in Description
	``` 6d448c9c ```
```After this we got logged in to secured shell {ssh} ```
Now type the following command

Use ls command to see whats inside the folder

ctf-player@pico-chall$ ls
1of3.flag.txt  instructions-to-2of3.txt

Boom we got some instruction and first part of flag

lets use cat command

ctf-player@pico-chall$ cat 1of3.flag.txt 
picoCTF{xxsh_

ctf-player@pico-chall$ cat instructions-to-2of3.txt 
Next, go to the root of all things, more succinctly `/`


Now lets go to the root folder 

ctf-player@pico-chall$ cd /
ctf-player@pico-chall$ ls
2of3.flag.txt  dev   instructions-to-3of3.txt  media  proc  sbin  tmp
bin	       etc   lib		       mnt    root  srv   usr
boot	       home  lib64		       opt    run   sys   var
ctf-player@pico-chall$ 

Boom we got the second part of the flag

ctf-player@pico-chall$ cat 2of3.flag.txt 
0ut_0f_\/\/4t3r_

Amd we also get some instructions

ctf-player@pico-chall$ cat instructions-to-3of3.txt 
Lastly, ctf-player, go home... more succinctly `~`

Lets move on to the home directory

ctf-player@pico-chall$ cd ~
ctf-player@pico-chall$ ls
3of3.flag.txt  drop-in
ctf-player@pico-chall$ 

Boom we got the final part of the flag

ctf-player@pico-chall$ cat 3of3.flag.txt 
5190b070}


Altogether

Flag : 
picoCTF{xxsh_0ut_0f_\/\/4t3r_5190b070}

And Done !!
Happy hacking ; It was little bit awesome...

