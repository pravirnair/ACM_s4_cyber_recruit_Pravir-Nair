4.This is for u know who 
Someone from the Hogwarts send this file given below to the voldemort.I don’t know who it is and what is the information in it. What ever the information is but it will definitely harm harry so find the person who send it. The flag lies there.

CHALLENGE DESCRIPTION:
The challenge was to find the flag which is hidden somewhere in the zip folder. 

APPROACH:
The first step I did was to unzip the given file. And inside the extracted directory I saw a receiver.txt which contained a normal message and there also was a hidden directory. In that hidden directory was a png file which was actually a webp file . I used binwalk to extract all hidden binary files. and inside the directory was another directory which contained a text file and a hidden directory.In that directory was a jpg file. I used exiftool to get the metadata and in that the author section had a base64 encoded message which was the flag when decoded using an online base64 decoder.


Tools/Commands used:
Binwalk, unzip, exiftool , ls -a 



FLAG:potter{7h15_15_D010r35_Um8r1dg3}
