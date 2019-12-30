INFERNO CTF 2019:

Forensics Challenges:

1. Merry Christmas :

This challenge supplied a .zip file which was password protected. The hint given to extract the .zip file was : MrT4anTra's Last name.The hint being pretty straight forward all you had to do was Search the same in google,Voila There you have the password "Malhotra". 

After extracting the zip file , we stumble across this file called "flag.gif"
Running the "file command" on this file we realize its not a gif file but is just a data dump.

If you open this file in any sort of "hexeditor" you will find that the header bytes are " 41 41 41 41 41 ", This is not the default gif header bytes,What we do now is replace these bytes with the actual gif header format bytes which is "47 49 46 38 39". Now we save this file.Voila! There you get your flag.

![Screenshot from 2019-12-30 21-36-02](https://user-images.githubusercontent.com/46860321/71590356-2667c600-2b4e-11ea-8c34-a94ead0b1c58.png)

After replacing the hexbytes...

![Screenshot from 2019-12-30 21-37-15](https://user-images.githubusercontent.com/46860321/71590394-47301b80-2b4e-11ea-9531-0a2b5c4f60d4.png)



