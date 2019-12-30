INFERNOCTF2019:

2. COLORBLIND:

This was another challenge under the forensics category in the INFERNOCTF2019. The challenge supplied to us a image file named 'colorblind.png'. Running the file command we find out its a 64x1 image which is pretty small.Running programs like "binwalk" also dont open any new doors to finding the flag, all they do is display the .zlib file which all state of the art PNG files use. 

What we do now is we find the RGB pixel values of the image.You can accomplish this using python or any online image converters.The output resembles:

![Screenshot from 2019-12-30 22-13-27](https://user-images.githubusercontent.com/46860321/71591401-308bc380-2b52-11ea-91f1-0c2bc15f7f26.png)

We remove all the occurences of "255" and "," using sed commands:
	sed 's/old-character/new-character/g' filename
After formatting the output , the final output looks like this :

![Screenshot from 2019-12-30 22-14-17](https://user-images.githubusercontent.com/46860321/71591403-31245a00-2b52-11ea-8670-2c96f603407d.png)

Now converting all these decimal values to ascii We get the FLAG!!! :

![Screenshot from 2019-12-30 22-12-53](https://user-images.githubusercontent.com/46860321/71591400-308bc380-2b52-11ea-990a-014a9417cb01.png)


