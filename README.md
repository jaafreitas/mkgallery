# [MkGallery](https://jaafreitas.github.io/mkgallery/)
Generate you own gallery with thumbnails for the internet with this simple shell script. In the top of the script you have some things you can change (or not). All pages are HTML 4.0 and CSS compatible.


## Let's start with some history
This project was developed in 2000 when I decided to learn shell script and I had a problem to solve: generate galleries for my pictures. What you will see here is an old code that was hosted on [SourceForge](https://sourceforge.net/projects/mkgallery/) for more than 20 years on a CVS repository. Even though the mkgallery script still works quite well, maybe it's not the best option for your needs nowadays.

This project was used by many websites in the earliest 2000 and we can still find some of them online, like the [latest plots](http://astroserve.mines.edu/clf/latest/crlf01.html) from http://astroserve.mines.edu/.

It is still available on some linux distributions like [gentoo linux](https://gitweb.gentoo.org/repo/gentoo.git/tree/media-gfx/mkgallery).


## How it works
Enter in a folder with jpg files and choose a name for the gallery.
You can also specify other option in the command line. See the help
('mkgallery -h') for more information.


## Dependencies
Basicly we need ImageMagic packages (convert and identify). The other
utilities are essential in any Unix system.


## Features
The script is divided in many functions to help we change anything
without breaking other functions. In the files start_html and
end_html we can put html code to be inserted in the top and bottom
respectively. All pages are HTML 4.0 checked with the validadtor in
the W3C website. With the CSS file is possible to change any color,
font, style without changing all HTML pages. Also you can specify
only one css file for all your pages. Comments can be added for
any image.


## TODO
* Add recursive option with a list of folders
* Make the script works with any kind of image
* Fix input file names to be filter by s/[^[:alnum:]]/\\&/g


## Bugs
* Something must be done to avoid 8bit characters in IMG SRC (maybe others?) Netscape seens to understand but I dont think it will work with all browser
* Netscape doesnt handle CSS very well. After the TABLE it doesnt display the font color of BODY defined in CSS
* text-transform: uppercase is not working for 8bit characters (like á, ç, etc)
* files cant start with a '-'. Will be fix soon.


## Thanks
### Martin Aspeli
Addition of comments system, addition of command line options, addition of
config file, various adjustments and optimizations and changes to the way
images are 'discovered' and included in the gallery
### Adilson Freitas
MkGallery logo image.

