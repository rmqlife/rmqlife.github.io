---
layout: post
title: "Use of ImageMagick"
date: 2016-07-01
categories: note
---
ImageMagick is a powerful tool which can do most "converting" things about images.

1. a substitution of the `Acrobat`, convert multiple images to a pdf file.
...{% highlight bash %}
convert image*.jpg scan.pdf
{% endhighlight %}

2. resize images
{% highlight bash %}
# save as
convert image.jpg -resize "20%" image-icon.jpg
# change on the file
mogrify *.jpg -resize "20%"
{% endhighlight %}

3. rename images
{% highlight bash %}
convert '*.jpg' pic%03d.jpg
# as pic001.jpg pic002.jpg pic003.jpg ...
convert *.jpg %d.jpg
# as 1.jpg 2.jpg 3.jpg ...
{% endhighlight %}

4. for transfer images from SD card
{% highlight bash %}
# copy to local
cp ./images ~/local
# resize images to load faster, build icons
mogrify ./*.jpg -resize "20%"
# delete the bad images
# list the remained
find ./ -name "*.JPG" >> filelist.txt
# copy filelist, change directory to SD　card
# copy the images to the local as you selected on the icons.
cat filelist.txt | xargs -t mv ~/Pictures/
{% endhighlight %}

[ImageMagick help]: http://www.imagemagick.org/script/command-line-processing.php#geometry
