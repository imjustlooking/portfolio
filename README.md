# Personal site

Visit [site](http://www.gabrielu.xyz).
This is where I store the code for my personal site for now.

Initially I had hosted it using herokuapp with a node.js framework, thinking to add routing. However, herokuapp limits your app active time and only wakes it up when the url is visited in a 30 minute window. Read more about heroku's policies for free hosting [here](https://www.heroku.com/free).

As of Dec 29, "When it idles (automatically, after 30 minutes of inactivity), or when you scale it down, your app will stop consuming dyno hours." What this means, is that after at least 30 minutes, your site becomes inactive, and requires a long initial load time, in my experience. That's not something your visitors would like; Github pages are pretty fast on the other hand.

I used [namecheap.com](http://www.namecheap.com) to purchase the domain, and that is also where I made adjustments to the advanced DNS settings.

If you are keen to find out how to use a custom domain for your github page hosting, I have added some pictures below to show you my current configuration.

* Disclaimer: There may be more updated resources out there documenting how to host between your domain site and github. It's best to do your own homework and follow those instead :)

Github settings
======

This part's easy.
Navigate to your github repository >> Settings >> Scroll down to Github Pages >> adjust custom domain to 'yourdomainname.com'.

I also assume you have already hosted the project on github pages. If you have not, adjust source to master branch >> Save.

![Github pages settings](/pics/github_settings.png "Github pages settings")


Made with
======
Javascript + Html + Slight CSS + [Instascan API](https://github.com/schmich/instascan)

Requirements
======
As long as you have a device with a camera and browser access. Seems to not work properly with iPhones, but tested well on my android phone(Samsung S7). Works best on Chrome browser, but default Samsung Internet browser allowed to toggle the active camera too.


Features
======
  * QR scanner API (obviously)
  * Using DOM selectors:
    * Copy scanned content to clipboard
    * Visit scanned content as url
    * Clear scanned content
  * Adjust default starting camera based on device camera numbers. E.g.: For my phone (android), defaults to the back camera, whereas for laptop, uses just the front/ any available camera.
