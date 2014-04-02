---
layout: post
author: yonghao
title: yonghao's twitter hack with tweet img function
date: 2014-04-02
---

I have add the following code to my tweethack.py file and then user can tweet image message. 
I create a folder called img to store image file. 
And then `open('img/unc.jpg','rb')` can open the image file.



```

elif tos == "tweet pictures":
    print "Let's tweet a picture from the command line!"
    
    while exit != True:
      tweet = raw_input("What would you like to tweet?  ")
      photo = open('img/unc.jpg','rb')
      twitter.update_status_with_media(status = tweet, media = photo)
      exit = raw_input("Type exit to go back or press enter to Tweet again.  ")
      if exit == "exit":
        exit = True
        
```
