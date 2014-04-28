My Tiny Core Linux extensions
===================

This repo contains the tiny core extensions I've built and the scripts I wrote to make them (one extension as of this writing).

How to use it
--------------

To build the extension, clone the repo to a Linux system (I used Tiny Core). Install mksquashfs and tcztools. 

To download and build s3cmd, run:

    $./s3cmd-get
    $./s3cmd-build
    
This will set up your `/tmp` dir, and now if you want to build the extension, run:

    $./tcz-pack s3cmd.tcz
    
I had to fix an issue in the tcz-pack in tcztools, which is why I included my own. You could not use tcz-pack, but then you have to do the list, md5, and mksquashfs stuff some other way.

Now, you should have a new tcz extension in `/tmp/tcztools/`.
