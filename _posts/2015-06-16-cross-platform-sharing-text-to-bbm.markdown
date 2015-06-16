---
published: true
title: Cross Platform Sharing Text to BBM
layout: post
tags: [coding, blackberry, bbm]
categories: [Coding, BlackBerry]
permalink: sharing-text-bbm-cross-platform
---
A simple line of code for **Sharing Text** to a BBM Contact. The code opens BBM Contact picker for the user to select the contact or contacts.

{% highlight html %}

bbmi://api/share?message=Hello&userCustomMessage=BBM%20message

{% endhighlight %}

On a web page:  

{% highlight html %}

    <a href=”bbmi://api/share?message=Hello World&userCustomMessage=BBM%20Message”> Share in BBM</a>

{% endhighlight %}

The *message* parameter is not editable by the user and is required. The *userCustomMessage* parameter is optional and populates part of the message that the user is able to modify and send.  

This code works Cross Platform on BlackBerry, Android and iOS. Windows Phone will be supported in the future!
