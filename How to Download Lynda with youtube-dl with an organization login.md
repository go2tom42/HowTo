# How to Download Lynda with youtube-dl with an organization login

## Needed:
[Cookies Export](https://chrome.google.com/webstore/detail/cookiestxt/njabckikapfpffapmjgojcnbfjonfjfg/related)
[youtube-dl](https://github.com/rg3/youtube-dl)

* Install Cookies Export
* Login to Lynda and navigate to the course you want
* Cookies export button in browser
* Copy "cookie.txt" to your desktop
* Open terminal


For OSX
```terminal
$ cd ~/Desktop
$ brew install youtube-dl
$ youtube-dl --write-pages --cookies cookie.txt --verbose --limit-rate 4M https://www.lynda.com/Drupal-7-tutorials/Creating-and-Editing-Custom-Themes/86650-2.html --verbose
```

Login is stored in the cookie.txt file. This has a limited life and will expire. It might leave "dump" files if there is any errors. These can be deleted. 
