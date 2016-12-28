---
title: Minium Release 1.5.0
header:
#  image: /assets/images/code.jpg
  teaser: /assets/images/code.jpg
categories:
  - Minium
  - release
author: zem3
---

[Minium 1.5.0](https://github.com/viltgroup/minium-developer/releases/tag/minium-developer-1.5.0) has just been released. This new version brings the following enhancements in relation to the previous release:

* Minium Developer is now available as a native application for Linux, macOS and Windows. In a future post, we will give more details about how we did it.
* Upgrade to Selenium 3. One of the benefits of this upgrade is that you can now run your tests on the latest versions of Firefox. Firefox 48 and later require the geckodriver, but you don't need to worry about it because Minium Developer takes care of downloading and configuring it for you.
* Allows the configuration of ChromeDriver-specific capabilities. You can add additional command line arguments to be used when starting Chrome, set the path to the Chrome executable, add Chrome extensions to install on browser startup and set Chrome preferences. See [here](http://minium.vilt.io/docs/developer/minium-developer/#chrome) how to do it.
* Support for a plugin mechanism like jQuery's. This allows you to, for example, [add a method that waits for an animated element to stabilize](http://minium.vilt.io/docs/code-samples/snippets/#add-new-methods-to-elements).

For more information, visit [Minium's documentation page](http://minium.vilt.io/docs/).
