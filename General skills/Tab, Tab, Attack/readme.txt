		``` Tab, Tab, Attack ```
Description :
	Using tabcomplete in the Terminal will add years to your life, esp.
	when dealing with long rambling directory structures and filenames: Addadshashanammu.zip

Solution 

Step1 :
	Download the file , copy link of zip , use wget to download using terminal
	
	$ wget https://mercury.picoctf.net/static/659efd595171e4c40378be6a2e9b7298/Addadshashanammu.zip

	Let's talk; {Tab attack}
	So in linux when we have a folder or anything that we can see using the ls command we can use [TAB] key of your keyboard to autofill
	Just go and type like;
	
	$ cd  [TAB KEY]
	And it will be something like ;
	                                                                                                            
┌──(selenophilem7㉿selenophilem7)-[~]
└─$ cd ~
Completing local directory
Desktop/    Documents/  Downloads/  hs/         Music/      Pictures/   Public/     Templates/  Videos/   

if you are in home directory
	
Step 2:
	Lets continue ;
	unzip the file that we downloaded using wget command

	$ unzip Addadshashanammu.zip

Step 3:
	Lets to tab attack that which we learn on step 1
	$ cd [TAB KEY] 
	it will be 
	$ cd Addadshashanammu 
	Continue the tab attack on cd you know !!
	Then after some time it will show not work as it does previously;
	Now its time to ls 
	
	$ ls 
	fang-of-haynekhtnamet
	
	Run the file
	$ ./fang-of-haynekhtnamet
	Boom we got the flag
Flag : picoCTF{l3v3l_up!_t4k3_4_r35t!_524e3dc4}

