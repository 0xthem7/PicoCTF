Python Wrangling

Description:
	Python scripts are invoked kind of like programs in the Terminal... 
	Can you run this Python script `ende.py` using this password `pw.txt` to get the flag?

	``` Solution ```

Step 1 :
	$ cat ende.py
	- To know what is the code doing
	- we see its encoding and decoding
Step 2 : 
	$ cat pw.txt
	- To know what is in the pw it a password file
	- Hmm, looks like we have to decode the flag now...
	- Lets, decode the file using the python script
	- As in the code 
	- usage_msg = "Usage: "+ sys.argv[0] +" (-e/-d) [file]"
	- we see it requires a file to encode and decode and we have and encoded file;
Step 3 :
	$ python3 ende.py -d flag.txt.en
	Please enter the password:aa821c16aa821c16aa821c16aa821c16
	Boom we got the flag!!!

┌──(selenophilem7㉿selenophilem7)-[~/…/Hacking/PicoCTF/General skills/Python Wraling]
└─$ python3 ende.py -d flag.txt.en 
Please enter the password:aa821c16aa821c16aa821c16aa821c16
picoCTF{4p0110_1n_7h3_h0us3_aa821c16}

