## shutup.css

shutup.css is a CSS stylesheet ([?][css-about]) that can be applied to your web browser to hide comment sections on many popular websites. It is maintained by [Steven Frank][site-steven] and [Ricky Romero][site-ricky].

## Why would I use it?

Some people feel that website comments are an annoyance or distraction from the main content. Some choose to use shutup.css to avoid being drawn into protracted arguments or avoid being exposed to statements that instill anger or sadness in them.

## How do I install it on my computer?

The simplest way to use shutup.css on a conventional desktop or laptop computer is with a browser extension. There are official extensions available for all mainstream browsers:

* [Shut Up for Chrome][ext-chrome]
* [Shut Up for Safari][ext-safari] (Shared link for macOS, iOS, and iPadOS)
* [Shut Up for Firefox][ext-firefox]
* [Shut Up for Edge][ext-edge]
* [Shut Up for Opera][ext-opera]

These extensions by [Ricky Romero][site-ricky] automatically include or retrieve the latest shutup.css stylesheet, and allow you to toggle comment blocking on and off with a toolbar button.

Shut Up for Safari on macOS requires macOS Sierra or later.

If you don't want a separate extension, you can instead use the [Stylus][stylus-plugin] plug-in, in combination with the raw shutup.css stylesheet (detailed below).

### Installation on Opera

Shut Up works well on Opera, but you have to install it from the Chrome Web Store. Here's how:

1. Go to [the page for Shut Up on the Chrome Web Store][ext-chrome].
2. Click the "Install Extension" button that appears under the address bar.
3. After the page reloads, click the "Add to Opera" button.
4. Dismiss the compatibility notice, which takes you to Opera's settings page for Shut Up.
5. Click the Install button.

Though Opera has an official add-ons website, Shut Up can't be listed there due to months-long approval cycles.

## How do I install it on my iPhone or iPad?

You must have a 64-bit device running iOS/iPadOS 9 or later.

The following content blocker apps include shutup.css:

* [Shut Up][ext-safari] by [Ricky Romero][site-ricky] (Shared link for macOS, iOS, and iPadOS. Requires iOS/iPadOS 12 or later)
* [Content Blocker+][content-blocker-plus] by [Dynamic App Design LLC][site-dynamic-app-design]

## How do I install it on an Android device?

Firefox on Android can run add-ons. Simply use [the official Shut Up extension for Firefox][ext-firefox].

## Do I have to use an extension or plug-in?

shutup.css can be used in any web browser that allows the loading of custom user stylesheets. Most popular browsers do for accessibility reasons; for example, to allow a visually impaired user to make text larger.

To use shutup.css as a custom user stylesheet:

1. Download the auto-updating [shutup-user-stylesheet.css][css-user] file to your system.*
2. In your browser's preferences, configure your browser to use shutup-user-stylesheet.css as a custom user stylesheet. In Safari for Mac, for example, it looks something like this:

<img alt="Safari screenshot" src="docs/safariprefs.png" width="406" />

After selecting "Other..." from the pop-up menu, select the shutup-user-stylesheet.css file you downloaded in step 1. This process will vary in other browsers, but the general idea is the same.

If you make changes to the stylesheet, or download a new version of shutup.css, you may need to quit and restart your browser to make sure it takes effect.

**If you don't trust a remotely-imported CSS file being applied to every web page you see, or if you want to make additional customizations, you can [download the most recent non-updating version][css-main] instead, but you will have to occasionally update this file manually.*

## How about a bookmarklet instead?

Another option is to install the shutup.css bookmarklet. The bookmarklet lives in your bookmarks toolbar, and applies the shutup.css stylesheet only when you click on it rather than automatically when pages load.

The bookmarklet can be installed by selecting the text below and dragging it into your browser's bookmark bar:

`javascript:%21function%28%29%7Bvar%20e%3Ddocument.getElementsByTagName%28%22head%22%29%5B0%5D%2Ct%3Ddocument.createElement%28%22link%22%29%3Bt.type%3D%22text/css%22%2Ct.rel%3D%22stylesheet%22%2Ct.href%3Dlocation.protocol+%22//rickyromero.com/shutup/updates/shutup.css%22%2Ce.appendChild%28t%29%7D%28%29%3B`

*Original bookmark by Justin Ridgewell. HTTPS fix by Alexandre Vallières-Lagacé*

## Anything I should watch out for?

shutup.css works by looking for blocks of content on the page that are identified in the page's source code as "comments" or similar identifiers. The stylesheet instructs the web browser to simply not display these blocks.

This may affect some web applications in unexpected ways. I'm told it hides the "discussion" section of Bugzilla installations, for example. Remember to try disabling shutup.css if you think you might be missing important page content.

## What about privacy?

Stylesheets like shutup.css contain no executable code, so they cannot track or spy on you.

The official browser extensions by Ricky Romero are designed to protect your privacy. None of these extensions track or spy on your browsing activity. They all have similar features, but differ in how they integrate with your browser. [Read the plain-English privacy policy here][ext-privacy] for info specific to your browser.

## Can I contribute to shutup.css?

Sure! You can [send me a pull request on GitHub][css-pull-request]. If you speak CSS but not Git, just [email me][email-steven] your proposed changes.

## How do I contact you?

You can contact me at [stevenf@panic.com][email-steven], or on Twitter as [@stevenf][twitter-steven].



[ext-chrome]: https://chrome.google.com/webstore/detail/oklfoejikkmejobodofaimigojomlfim?hl=en-US&amp;gl=US  (Shut Up on the Chrome Web Store)
[ext-safari]: https://apps.apple.com/app/id1015043880  (Shut Up on the App Store)
[ext-firefox]: https://addons.mozilla.org/en-US/firefox/addon/shut-up-comment-blocker/  (Shut Up at Firefox Add-ons)
[ext-edge]: https://microsoftedge.microsoft.com/addons/detail/giifliakcgfijgkejmenachfdncbpalp  (Shut Up at Edge Add-ons)
[ext-opera]: #installation-on-opera  (Installation on Opera)
[ext-privacy]: https://rickyromero.com/shutup/privacy/  (Shut Up Privacy Policy)

[css-main]: shutup.css  (Main Stylesheet)
[css-user]: shutup-user-stylesheet.css  (User Stylesheet)
[css-about]: https://en.wikipedia.org/wiki/Style_sheet_(web_development)  ("Style sheet" on Wikipedia)
[css-pull-request]: https://github.com/panicsteve/shutup-css/edit/master/shutup.css  (Submit a Pull Request for shutup.css)

[site-steven]: https://stevenf.com  (Steven Frank's personal website)
[site-ricky]: https://rickyromero.com  (Ricky Romero's personal website)
[site-dynamic-app-design]: http://dynamicappdesign.com  (Dynamic App Design LLC)

[email-steven]: mailto:stevenf@panic.com  (Steven Frank's email address)
[twitter-steven]: https://twitter.com/stevenf/  (Steven Frank's Twitter profile)

[content-blocker-plus]: https://apps.apple.com/app/id1040960141  (Content Blocker+)
[stylus-plugin]: https://add0n.com/stylus.html  (Stylus Plugin)
