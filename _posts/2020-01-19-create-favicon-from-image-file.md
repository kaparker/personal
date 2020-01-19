---
layout: posts
title:  "How to create a favicon from an image file on mac"
date:   2020-01-19 22:00:00 +0100
categories: [article]
tags: [web development] 
backgroundurl: https://images.unsplash.com/photo-1506729623306-b5a934d88b53
time: 1 min
lang: en
description: Quick tips to create a favicon for your website from an image file on a mac.
---

When trying to create a favicon for my personal website I searched through a range of website to find a suitable way to do this and thought I'd add this tip here to make it easier to do again in the future. 
<br><br>
Whilst there are tools online that easily convert your image to a favicon, it's nice to be able to do the conversion locally, especially as the initial image I was trying to convert is my profile picture and I don't feel entirely comfortable uploading this to a random website!
<br><br>
For mac users there are two options:
<br><br>
1. Export image with Preview
    
    *Whilst this method is straight forward, I'm getting an error when exporting so used method 2 below.*

    Open your image in Preview, goto File > Duplicate to create a copy. Goto File > Save to save this new image and when selecting from the Format drop down hold the option or alt key. 
    To save a Favicon select 'Microsoft Icon' and save! As mentioned above, I was presented with an error on saving so searched for an alternative method.
<br><br>
2. Using `imagemagick`

    Install imagemagick and it's dependent package ghostscript.
    ```
    brew install imagemagick
    brew install ghostscript
    ```
    Run the following command:
    ```
    magick image.jpeg favicon.ico
    ```
    <br>

In one simple line, once `imagemagick` has been installed, your image can be converted to a favicon and easily added to your website!