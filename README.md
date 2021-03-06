TrippyThumbs
============

An experimental approach to website thumbnails.


Mockups
-------

- [Demo page](mockups/index.html)


Sample websites
---------------

These are websites to try generating thumbnails from.

- [Facebook](http://facebook.com)
	- Facebook profile page
- [Google](http://google.com)
- [An Erowid Article](http://www.erowid.org/plants/tobacco/tobacco.shtml)
- [Github](https://github.com/)
- [A GitHub Profile](https://github.com/vtsatskin)
- [YouTube](http://youtube.com)

Identification Technqiues
----------------------------

These are certain aspects we can use from websites to generate identifiablity cues

- Logo
- Salient images on website
- Website dominant colours
- Title
- URL
- Favicon

Current Behaviour and Issues
----------------------------

![](images/current.design.png)

These are the current issues with the existing thumbnails

- Redirect got captured as a page
- Duplicates: https and http version
	- www. vs none.
- "Authorization Required" on sites with http auth such as [Mana](http://mana.mozilla.org)

Current Code
------------

- [Foreground service](http://mxr.mozilla.org/mozilla-central/source/toolkit/components/thumbnails/PageThumbs.jsm)
- [Background service](http://mxr.mozilla.org/mozilla-central/source/toolkit/components/thumbnails/BackgroundPageThumbs.jsm)

Inspiration
-----------

### Google Play Music ###

![](images/inspiration/google.music.2.png)
![](images/inspiration/google.music.2.hover.png)

- Relevant band image shown
- Hover state is interactable

![](images/inspiration/google.music.png)

- Album art as background with blur
- Displayed when no band image availible

![](images/inspiration/google.music.many.png)

### Opera Speed Dial ###

![](images/inspiration/opera.speed.dial.png)

- Some website such as Facebook, YouTube, Google, Twitter, will show logos.
- Others will show screenshot

### Interactions/Effects ###

- [Caption Hover Effects](http://tympanus.net/Tutorials/CaptionHoverEffects/index3.html)
- [Shape Hover Effect with SVG](http://tympanus.net/Tutorials/ShapeHoverEffectSVG/index2.html)

Misc. Ideas
-----------

### Custom Tiles ###

The tiles could be extendable via our existing addon infrastructure similiar to how Opera has [Speed Dial extensions](http://dev.opera.com/extension-docs/tut_sd_extensions.html).

Existing Research
-----------------

- [How People Recognize Previously Seen WWW Pages from Titles, URLs and Thumbnails][recognize] by Kaasten, S., Greenberg, S. and Edwards, C. (2002)
- [Visual Snippets: Summarizing Web Pages for Search and Revisitation][summarizingWebPages]

[recognize]:http://grouplab.cpsc.ucalgary.ca/Publications/2002-ThumbnailStudy.BHCI
[summarizingWebPages]:http://research.microsoft.com/en-us/um/people/cutrell/visual-snippets-chi2009-submission.pdf