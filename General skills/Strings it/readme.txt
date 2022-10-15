	```Strings it```

Description

Can you find the flag in file without running it?

Step 1:
	First of all copy the link of the file.
	Then use wget command to download the file to the local directory;
	$ wget https://jupiter.challenges.picoctf.org/static/5bd86036f013ac3b9c958499adf3e2e2/strings
	Once file is downloaded lets move to the next step

Step 2:
	If you don't know about strings command it is used to print the charactes of the strings types which are printable in the file.
	
	$ strings [File name]
	which will be 
	$ strings strings 
	remember the second strings is file name and second one is the command
	
	Uff!! lots of garbage lets use grep because we know the flag type
	
	$ strings strings | grep pico
	picoCTF{5tRIng5_1T_827aee91}
	Boom we solved this one tooo....
