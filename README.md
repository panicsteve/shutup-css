## shutup.css

shutup.css is a CSS stylesheet ([?](https://en.wikipedia.org/wiki/Style_sheet_(web_development))) that can be applied to your web browser to hide comment sections on many popular websites. It is maintained by [Steven Frank](http://stevenf.com/).

## Why would I use it?

Some people feel that website comments are an annoyance or distraction from the main content. Some choose to use shutup.css to avoid being drawn into protracted arguments or avoid being exposed to statements that instill anger or sadness in them.

## How do I install it on my computer?

The simplest way to use shutup.css on a conventional desktop or laptop computer is with a browser extension.  Currently there are extensions for Safari and Chrome on any operating system:

* [Shut Up for Safari](http://rickyromero.net/misc/SafariExtensions/ShutUp.safariextz) by [Ricky Romero](https://rickyromero.com)
* [Shut Up for Chrome](https://chrome.google.com/webstore/detail/oklfoejikkmejobodofaimigojomlfim?hl=en-US&amp;gl=US) by [Ricky Romero](https://rickyromero.com)

These official browser extensions automatically update themselves with the latest shutup.css stylesheet, and allow you to toggle comment blocking on and off with a toolbar button.

Although there is no official Shut Up extension for Firefox at this time, Firefox users have reported success using the [Stylish](http://userstyles.org/) plug-in, in combination with the raw shutup.css stylesheet (detailed below).

## How do I install it on my iPhone or iPad?

You must have a 64-bit device running iOS 9 or later.

The following content blocker apps include shutup.css:

* [Shut Up](https://itunes.apple.com/us/app/shut-up-comment-blocker/id1015043880?mt=8&amp;at=1l3vbmm) by [Ricky Romero](https://rickyromero.com)
* [Content Blocker+](https://geo.itunes.apple.com/us/app/content-blocker+/id1040960141?mt=8&amp;at=1l3vbmm) by Dynamic App Design LLC

## Do I have to use an extension or plug-in?

shutup.css can be used in any web browser that allows the loading of custom user stylesheets.  Most popular browsers do for accessibility reasons; for example, to allow a visually impaired user to make text larger.

To use shutup.css as a custom user stylesheet:

1. Download the auto-updating [shutup.css](http://stevenf.com/shutup/shutup.css) file to your system.
  If you don't trust a remotely-imported CSS file being applied to every web page you see, or if you want to make additional customizations, you can [download the most recent non-updating version](http://stevenf.com/shutup/shutup-latest.css) instead, but you will have to occasionally update this file manually.
2. In your browser's preferences, configure your browser to use shutup.css as a custom user stylesheet. In Safari for OS X, for example, it looks something like this:

<p><img src="https://stevenf.com/gfx/safariprefs.png" width="406" height="270" alt="Safari screenshot"></p>

After selecting "Other..." from the pop-up menu, select the shutup.css file you downloaded in step 1. This process will vary in other browsers, but the general idea is the same.

If you make changes to the stylesheet, or download a new version of shutup.css, you may need to quit and restart your browser to make sure it takes effect.

## How about a bookmarklet instead?

Another option is to install the shutup.css bookmarklet.  The bookmarklet lives in your bookmarks toolbar, and applies the shutup.css stylesheet only when you click on it rather than automatically when pages load.

The bookmarklet can be installed by dragging it into your browser's bookmark bar:

`javascript:%21function%28%29%7Bvar%20e%3Ddocument.getElementsByTagName%28%22head%22%29%5B0%5D%2Ct%3Ddocument.createElement%28%22link%22%29%3Bt.type%3D%22text/css%22%2Ct.rel%3D%22stylesheet%22%2Ct.href%3Dlocation.protocol+%22//rickyromero.com/shutup/updates/shutup.css%22%2Ce.appendChild%28t%29%7D%28%29%3B`
<p><a href=""><img src="/web/20170419093034im_/https://stevenf.com/gfx/shh.png" width="39" height="20" alt="Shh!"></a></p>

Original bookmark by Justin Ridgewell. HTTPS fix by Alexandre Vallières-Lagacé

## Anything I should watch out for?

shutup.css works by looking for blocks of content on the page that are identified in the page's source code as "comments" or similar identifiers.  The stylesheet instructs the web browser to simply not display these blocks.

This may affect some web applications in unexpected ways. I'm told it hides the "discussion" section of Bugzilla installations, for example. Remember to try disabling shutup.css if you think you might be missing important page content.

## What about privacy?

Stylesheets like shutup.css contain no executable code, so they cannot track or spy on you.

If you are using one of the browser extensions, it will periodically contact Ricky's web server solely to check for an update and download it if one is available.  When this happens, the date and time, your IP address, and "User-Agent" string (which identifies your web browser) are logged by the web server.  These logs are kept temporarily for diagnostic purposes only.

## Can I contribute to shutup.css?

Sure! You can [send me a pull request on GitHub](https://github.com/panicsteve/shutup-css/edit/master/shutup.css).  If you speak CSS but not Git, just email me your proposed changes.

## How do I contact you?

You can contact me at [stevenf@panic.com](mailto:stevenf@panic.com), or on Twitter as [@stevenf](http://twitter.com/stevenf/).
