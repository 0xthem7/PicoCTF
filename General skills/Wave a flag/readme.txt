	``` Wave a Flag ```
Description
Can you invoke help flags for a tool or binary? 
This program has extraordinarily helpful information...

Solution

Step 1:
	$ chmod +x warm 
	- Give executable permission

Step 2:
	$ ./warm
	Hello user! Pass me a -h to learn what I can do!
	- ./ is used to run the file ;
	- Lets pass -h as mentioned in the text
Step 3:
	$ ./warm -h
	Oh, help? I actually don't do much, but I do have this flag here:
	picoCTF{b1scu1ts_4nd_gr4vy_755f3544}
	- Boom we got the flag

┌──(selenophilem7㉿selenophilem7)-[~/…/Hacking/PicoCTF/General skills/Wave a flag]
└─$ ./warm
Hello user! Pass me a -h to learn what I can do!
                                                                                     
┌──(selenophilem7㉿selenophilem7)-[~/…/Hacking/PicoCTF/General skills/Wave a flag]
└─$ ./warm -h
Oh, help? I actually don't do much, but I do have this flag here: picoCTF{b1scu1ts_4nd_gr4vy_755f3544}
