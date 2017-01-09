---
title: Minium Developer is now an Electron app!
header:
  teaser: /assets/images/code.jpg
author: josemorgado
---

If you already downloaded the latest version of Minium Developer, you have noticed that it is now available as a native application for Linux, macOS and Windows. In this post, I am going to briefly explain how we did it using [Electron](http://electron.atom.io/), a framework based on Chromium and Node.js for creating native applications with web technologies like JavaScript, HTML, and CSS.

The process is actually quite simple. Basically, we have developed an Electron app that creates a browser window, starts the web application and then loads the editor. To start the web application, we use [Node's Child Process API](https://nodejs.org/api/child_process.html) to execute the script that you used to run previous versions of Minium Developer.

To build the different native applications for each operating system, we use [Electron Packager](https://github.com/electron-userland/electron-packager). We have integrated it in our existing Maven build process through the [frontend-maven-plugin](https://github.com/eirslett/frontend-maven-plugin).

If you want to know more, you can take a look at the code at https://github.com/viltgroup/minium-developer.

Nevertheless, you still can run Minium Developer from the browser as before. To do it, run the executable from the console and pass it the `--browser` option. The same executable is now also used to run Automator projects. See the [documentation](http://minium.vilt.io/docs/developer/minium-developer/#run-minium-scripts) for detailed instructions on how to do so.
