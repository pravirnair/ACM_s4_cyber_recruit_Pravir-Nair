2.Letter from Hogwarts
CHALLENGE DESCRIPTION:
The challenge had a password protected pdf in it which contained the flag for the question. 


APPROACH:
After reading the question I understood that I had to use john the ripper to crack open the password. I first converted the pdf file into hash format then I renamed the hash file with a txt extension . I used john the ripper to find the password by searching the password from rockyou.txt which was already there in my laptop. 

COMMANDS USED : 
pdf2john Letter_from_Hogwarts.pdf > pdf.hash [extracts the hash from the pdf and stores it in a file called pdf.hash]

mv pdf.hash pdf.txt [converts the file type]
john --wordlist=/usr/share/wordlists/rockyou.txt pdf.txt [uses john the ripper to find the password]


FLAG : potter{w3lc0m3_70_h0gw4r75}

