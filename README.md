INFERNO CTF 2019:

Forensics Challenges:

1. Merry Christmas :

This challenge supplied a .zip file which was password protected. The hint given to extract the .zip file was : MrT4anTra's Last name.The hint being pretty straight forward all you had to do was Search the same in google,Voila There you have the password "Malhotra". 

After extracting the zip file , we stumble across this file called "flag.gif"
Running the "file command" on this file we realize its not a gif file but is just a data dump.

If you open this file in any sort of "hexeditor" you will find that the header bytes are " 41 41 41 41 41 ", This is not the default gif header bytes,What we do now is replace these bytes with the actual gif header format bytes which is "47 49 46 38 39". Now we save this file.Voila! There you get your flag.



