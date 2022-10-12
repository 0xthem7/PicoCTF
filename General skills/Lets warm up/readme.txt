	``` let's warm up ```

Description 
If I told you a word started with 0x70 in hexadecimal, what would it start with in ASCII?

Hint:
Submit your answer in our flag format. For example, if your answer was 'hello', you would submit 'picoCTF{hello}' as the flag.

Lets crack it;


Step 1:
	Lets talk about ascii;
	ASCII stands for American Standard Code for Information Interchange;
	It is one of the most used encoding system which has 128 aphabatic, numeric as well as special character encoding;
	
	For Example ;
	Sn.     Normal Form				Ascii Encoded Decimal	Ascii Encoded HexaDecimal
	 1      A						65						0x41
	 2		a						97						0x61
	
	And the list goes on;

Step 2 :
	From the Question we have an clear Idea that the encoded data is in hexadecimal formate of ascii so lets convert that into normal form
Step 3 :
	Search for hex to ascii converter ;
	I used https://www.rapidtables.com/convert/number/hex-to-ascii.html this website.

Now finally we got the letter which is p 
lets make it look like flag as mentioned in hint section.

picoCTF{p}
