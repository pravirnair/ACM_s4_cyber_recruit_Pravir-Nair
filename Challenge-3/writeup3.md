3.WAND
CHALLENGE DESCRIPTION:
The challenge gave a jpeg file and the question also hinted that the file may contain hidden data(flag)


APPROACH:
I used exiftool to extract he metadata of the jpeg file . There I saw a comment which stated that the password is the full name of the wand wielder. I tried the binwalk method to find hidden files inside the jpeg image but I was not able to find anything .I searched for all the owners of the elder wand . I learned that you can use steghide to find further info of any image. I used the password hint and understood that there is a hide.txt file hidden inside the image . I extracted it and then got the flag


COMMANDS USED : 
exiftool wand.jpeg
steghide info wand.jpeg
steghide extract wand.jpeg

FLAG:potter{1_570l3_7h47_3ld3r_w4nd}
