python-code / imageGrab.py
===========
I addressed an issue when migrating from Go Daddy Quick Shopping Cart to Shopify, which was when I exported the QSC product list,
it only gave me a list image names. This was an issue since I did not have the original image files, and there was no way to
get them. Go Daddy assigned a random name to the images when trying to download them, so all I had was the list of file names.
If I access the image files directly in the browser, it worked.

I decided to create a raw text file with a list of image names. Once I did this, I ran this code to open the file, remove the 
new line character ("\n"), and then save that into a variable. From there, I ran a loop through all file names and used 
string formatting to create a variable with the proper URL in front of the image name, and once I did this, all I had to do
was write/save the image to my current directory (a.k.a. where this code is on your computer).

Run code with ./imageGrab.py in terminal on Mac OSX
