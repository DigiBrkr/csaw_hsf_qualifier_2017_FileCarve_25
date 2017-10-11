# File Carve
25 points
> He was frantically deleting files when we detained him. Maybe you can find a way to recover them from the flash drive?
>This is the same file as Mount Image, but we have it here for your convenience. MissingPage's pdf is also included in the file.
## Solving it

We know that Herbert was deleting files from the image so we need to use a tool to recover deleted files.
The tool to do that is called `foremost` originally created by the U.S. Air Force (now in the public domain).  

To recover the data we type the following commands:

`# foremost fat.fs`. Ignore the junk it puts in your terminal window, for the purposes of this challenge it is irrelevant.
In the same directory as the original file `foremost` will create a directory called `output`. Next, `cd` into this
directory.
`# cd output`
Then we do an `ls` to see the contents of this directory. 
```
# ls
audit.txt  pdf  png  zip
```
We see a file and three folders. At first glance, to me, the directory that seems most interesting is `png`.
Now open up the `png` directory in your **GRAPHICAL** file browser and open the image:

![flag](https://github.com/DigiBrkr/csaw_hsf_qualifier_2017_FileCarve_25/blob/master/00008592.png?raw=true)

`flag{remember_deleting_doesnt_delete}`
