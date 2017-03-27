---
layout: post
title: "My Firefox Configuration (Dark Mode)"
date: 2017-03-26 11:25:06
tags: dark-mode firefox
description: My dark-mode Firefox configuration
image: firefox_preview.jpg
excerpt_separator: <!--more-->
comments: true
---

## Dark-Mode

Over the last years i've become more and more obsessed with dark-mode for all the programs i use. Also the reason why this website looks like this:) Especially in the morning and evening i find it extremely less eye restraining than looking on screen with a bright background. 

One of the most used programs is the browser thus i spent a lot of time to figure out on howto make reading websites less white but still look nice:)

<!--more-->

As you can see the background color of the article part of this website is actually identical to my global Firefox background color configuration. That's why you don't see any image borders:)

![My helpful screenshot]({{ site.baseurl | prepend:site.url}}/images/{{page.url}}/firefox.jpg){: .center-image }*Firefox with Addons*


#### FT Deep Dark Theme

Boy this is a great dark theme. On Windows and Linux it's pretty simple, just follow the link below and click the "Add to Firefox"-Button (opening the link in Firefox obviously).

Unfortunately this is not officially available for MacOS, but it works nevertheless. You need to download the xpi file (that the firefox extension file format) and manually install it. Here's how i do it but there a other ways:
* enable Develop Mode in Safari (Safari -> Preferences -> Advanced -> Show Develop Menu in menu bar)
* then you have a new menu Develop available in Safari where you can change the UserAgent, so change it to Firefox Windows. (Develop -> User Agent -> Firefox Windows)
* goto the following url [FT Deep Dark Firefox Addon](https://addons.mozilla.org/en-US/firefox/addon/ft-deepdark/) and right click on the "Add to Firefox" Button. Choose "Download Linked File As.." . This should open a File-Save dialog with an filename ending on xpi already entered. You can change it just keep the xpi ending and remember where you saved it. If you don't see the "Add to Firefox"-Button make sure that the UserAgent is set as described in step above and reload the page
* Next goto Firefox and Choose: Tools->Addons
* Now select "Appearance" and click on the gear wheel icon in the top right. Now a menu should popup where you select "Install Add-on from File .."
* In the file-choose dialog select the xpi file that was downloaded previously. Afte you pressed ok the FT Deep Dark addon should be listed in the Appearance list and it should have a notice that you need to restart Firefox to enable the it (click on it to restart Firefox)

Now Firefox whill have a nice themed menubar, url-bar and all other Firefox menus (eg. Prefences, Addon, New Tab etc.). One thing that's still missing is that normal websites still look the same. That going to be fixed the the next Addon.

#### Dark Background and Light Text

This addon works for all OSes out of the box, so there is no special install for MacOS. Open the Url in Firefox [Dark Background and Light Text](https://addons.mozilla.org/de/firefox/addon/dark-background-light-text/?src=search) and click the "Add to Firefox". 

Once it is installed it will overwrite the background, font and some other colors on each website. First it's possible to disable it per domain, so if you have a site which you prefer to see in the original colors just disable it for this domain. The default background color is black so if you open any site now you should have a white text on black background.

There should be a new icon in you Firefox Icon bar (Aa on black background). Once you click it you have several options. Click on the Global Preferences Button which will bring you to the configuration page for this addon. Here you can define the colors which are applied by default to every page.

![My helpful screenshot]({{ site.baseurl | prepend:site.url}}/images/{{page.url}}/darkbackground_menu.jpg){: .center-image }*Dark background menu options*

On the settings we want to change 2 properties:

* Default Foreground Color (Text Color): set this to #C0C0C0
* Default Background Color (Website background): set this to #252626

Now open any site will apply these colors that match the FT Deep Dark Theme. Feel free to change any other colors to your preferences. For some webistes this may cause issues as some things might not be visible anymore. Fortunately you can disable this override per domain.

![My helpful screenshot]({{ site.baseurl | prepend:site.url}}/images/{{page.url}}/firefox_twitter.jpg){: .center-image }*Twitter website*

P.S:

In addition i use Flux (MacOS and Windows) and Redshift (Linux) to reduce blue light. (With the next MacOS (10.12.4) and Windows (Creators) udpates both will get this as a build in OS-feature)