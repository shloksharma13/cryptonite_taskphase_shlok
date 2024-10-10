# Heads up, tails down
In this challenge, we're given a corrupted `png` file. We play around by converting it to `pdf` and `jpeg` etc file formats but nothing seems to work. 
But then we open the file in its hexadecimal code and find a statement `fix me to crack me` so we play around and research into file forensics and notice that the typical header for a png file is missing.
Hence we google up the header for a typical png file and change the hexadecimal code to that header and save the file. The file is now fixed and the flag has been captured.
