# markdownTrics (mostly using pandoc)

## HTML
Use -c to add a css (e.g. notes.css) file and -s to make the output file self contained.


## Beamer
images in beamer presentations can be resized with eg \!\[\]\(img/file.jpg\){width=50%}.

## ImageMagic for working with images
To change print size of image without changing number of pixels:

convert -units PixelsPerInch -density 300 original_img.png transformed_img.png

I usefull for slides which usually have a very small "print" size but will be viewed on full screen. Works with png imges at least. To check what pixel density the image has you can use:

identify -verbose img/microscopeSmall.jpg
