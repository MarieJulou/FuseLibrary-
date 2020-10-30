# FuseLibrary

The very first things you need to do is to install libfuse3-dev
So before installing it, you got to make sure your repository cache is updated

`sudo apt update`

then run the following lines

```
sudo apt-get install libfuse-dev
sudo apt-get install libfuse3-dev
```

and then install the fuse library 

`sudo apt-get install fuse3`

and now that your tools are ready you just have to compile the following line

sudo gcc -Wall hello.c `pkg-config fuse3 --cflags --libs` -o hello

and then you can run your file with this:

`./hello <mountpoint>`
you just have to replace the `<mountpoint>` by your mountpoint of choice 

>for example `./hello /home/marie/Documents/testing`

and now you can type the content of your file and you're done
