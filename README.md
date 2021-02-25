# markdownTrics

## ImageMagic for working with images
To change print size of image without changing number of pixels:

convert -units PixelsPerInch -density 300 original_img.png transformed_img.png

I usefull for slides which usually have a very small "print" size but will be viewed on full screen. Works with png imges at least. To check what pixel density the image has you can use:

identify -verbose img/microscopeSmall.jpg
