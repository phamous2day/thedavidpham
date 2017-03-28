# http://thedavidpham.com (new UX Portfolio site)


## CHALLENGES

Took me a week to work on this new portfolio website. Lots of challengs along the way:
* npm serve was out of date, had to update it ... but in turn found out my Homebrew was out of date
* ended up removing homebrew because I didn't like the dependence NodeJS had on it
* Using FTP I got my files hosted ... but nothing got published. Support agent said he had to change the name server to get it working
* After 15 minutes, my files slowly get published ...then stopped ... wondering if it's because AWS is down or something?
* Ended up making a [redirect page](http://stackoverflow.com/questions/5411538/redirect-from-an-html-page) to my portfolio that's hosted on Github.
* Changed z-index from 60 to 9999: header[role="header"] nav ul{ display:none; position: fixed; z-index:9999; text-align:center; width:100%; height:100%; top:0; left:0; right:0; background-color:rgba(255,255,255,0.8); padding:0; margin:0; padding-top:199px;} --> This will allow popup menu to inline the links rather than have people click through into the contents of the page.
* Ended up removing hamburger menu [for these reasons](https://uxplanet.org/the-hamburger-icon-problems-solution-17c01b07f000#.dylzfam6n)
* Added spacing between h4 subheaders for easier paragraph chunking: bootstrap.min.css
```
.h4, .h5, .h6, h4, h5, h6 {
    margin-top: 10%;
    margin-bottom: 2%;
```
* Images on my home page are stretched in Safari browser ... turns out it's how Safari renders height. Removed height & min-height 6values for the "grid figure" and "grid figure img" in reference to this [article](https://css-tricks.com/forums/topic/images-stretched-in-safari-and-chrome/)

