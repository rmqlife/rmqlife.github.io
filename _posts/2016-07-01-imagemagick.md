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
...{% highlight bash %}
convert image.jpg -resize "20%" image-icon.jpg
{% endhighlight %}

3. rename images
{% highlight bash %}
convert '*.jpg' pic%03d.jpg
# as pic001.jpg pic002.jpg pic003.jpg ...
convert *.jpg %d.jpg
# as 1.jpg 2.jpg 3.jpg ...
{% endhighlight %}


[ImageMagick help]: http://www.imagemagick.org/script/command-line-processing.php#geometry
