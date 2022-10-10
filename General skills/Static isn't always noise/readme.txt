	``` Static isn't always noise ```

Description :
	Can you look at the data in this binary: static? This BASH script might help!

Solution

step 1:
	Give executable permision to the bash file.
	$ chmod +x ltdis.sh
step 2 :
	Tried to read the static but lots of garbage
step 3:
	Now run the following command

┌──(selenophilem7㉿selenophilem7)-[~/…/Hacking/PicoCTF/General skills/Static isn't always noise]
└─$ ./ltdis.sh static 
Attempting disassembly of static ...
Disassembly successful! Available at: static.ltdis.x86_64.txt
Ripping strings from binary with file offsets...
Any strings found in static have been written to static.ltdis.strings.txt with file offset


step 4:
	cat the static.ltdis.strings.txt
 and we got the flag

flag : picoCTF{d15a5m_t34s3r_1e6a7731}
