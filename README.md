# markdownTrics (mostly using [pandoc](https://pandoc.org/))
These are basically privat notes made public.

## HTML
Use -c to add a css (e.g. notes.css) file and -s to make the output file self contained.

## Beamer
The pandoc command to make a beamer presentation is:

`pandoc -t beamer markdownfile.md -o presentationfile.pdf`

A common header can look like:

```
---
title: My Title
author: Martin Ryberg
theme: Singapore
---
```

Images in beamer presentations can be resized with eg \!\[\]\(img/file.jpg\){width=50%}.

## ImageMagic for working with images
To change print size of image without changing number of pixels:

`convert -units PixelsPerInch -density 300 original_img.png transformed_img.png`

I usefull for slides which usually have a very small "print" size but will be viewed on full screen. Works with png imges at least. To check what pixel density the image has you can use:

`identify -verbose img/microscopeSmall.jpg`
