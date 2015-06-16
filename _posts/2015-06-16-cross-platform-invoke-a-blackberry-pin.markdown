---
published: true
title: Cross Platform Invoke a BlackBerry PIN
layout: post
tags: [coding, blackberry, bbm]
categories: [Coding, BlackBerry]
permalink: invoke-blackberry-pin-cross-platform
---
A simple line of code to link a **BlackBerry PIN** on any website in order to invoke the PIN contact within your BlackBerry browser.

{% highlight html %}

    <a href=”bbmi://2BAFF6CC”>Start BBM Chat or Invite User</a>

{% endhighlight %}

This code works Cross Platform, BlackBerry, Android and iOS. **bbmi://<PIN>** can be used to start a BBM conversation if the PIN is an existing contact.  If it’s not an existing contact the user will be prompted to invite the user to BBM.