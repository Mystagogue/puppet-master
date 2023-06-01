<p align="center">
  <img src="./images/PuppetMasterBETA2.png" alt="Puppet Master Icon" width="200px" height="200px"/>
</p>
<h1 align="center" style="color: #00D7A0;">Puppet Master</h1>

Puppet Master combines browser automation with regular surfing! You can **use** the browser while automating it - and it makes doing that super easy! Never underestimate the value of convenience. Perfect for manual testing, webscraping and power users.

<p align="center">
  <img src="./images/firstScreen.png" alt="Puppet Master Interface" width="1000px"/>
</p>

The app has a big red button. When you click this button it searches your computer for the first install of Chrome it can find, then it spawns an entirely **new** instance of Chrome. One that is brand new and has _no_ profile, _no_ history, _no_ cookies, _no_ cache, _no_ storage, _no_ prior memory of anything at all! If you click the button multiple times you will get **multiple** instances of Chrome, all of which are in complete **context isolation** from one another! This means you can sign into the same site with mutliple different users at the same time! The app connects to each instance via websocket and shows you a preview of its screen which updates automatically. When you close these instances, they are gone forever - no need to refresh browser cache again, just close the browser and start a new instance!

<p align="center">
  <img src="./images/secondScreen.png" alt="Multiple Browsers" width="1000px"/>
</p>

<p align="center">
  <img src="./images/chromeIcons.png" alt="Multiple Chrome Icons" width="200px"/>
</p>

But theres more... There is a fully featured file system and a code editor. Any **puppeteer** automation code you write in the code editor can be executed on any of the new browsers you have created. There is no need to launch the browser as this is done for you (when you clicked the big red button) and user input code is wrapped in an _async_ function so you can use the _await_ keyword immediately. This really takes the hassle out of writing automations. Unlike regular test automation software you can keep using the browser as a regular manually surfing browser while doing this. Run as many scripts on a browser as you like, the scripts retain no memory of each other, only the browser persists! _Need to test something on the 3rd step of a multi-step form?_ Run an automation to get you there then keep going manually. You can run a whole file at a time, or just the currently selected code or you can even run whatever you have copied to your clipboard. Great if you want to test one line at a time, **the browser won't crash if the code fails**, the app will just give you a debug message and the browser will keep running so you can keep using it.

<p align="center">
  <img src="./images/debug2.png" alt="Multiple Browsers" width="700px"/>
</p>

Theres even more... There are environment variables and preload scripts that allow you to create complex wrapper methods for your automation script meaning it is even easier and faster and more convenient to write. Since this app has an integrated file system you can store your automation code in multiple files, perhaps corresponding to each of your projects and have different environment variables and preload scripts for each.

There is even more... Any data can be extraced from the page and added to the "log" object. The log object is a POJO (Plain Old Javascript Object) that is in scope all the time. Just add properties to it as you like and they will be visible in the out put window. Perfect for Web Scraping!

There is even more...You can use the "require()" function in any of your scripts and it will look for a node_modules folder at the top level of the currently open folder. So you can create complex scripts. Why not look up the data for the current user in the database using the script, then log it to the output window WHILE you are browsing, so you have all the data you need to debug any problems with your site!

Even if you have 100% automated test coverage you can never get around the need to manually test. What do you do when you are in the process of building a new feature? No test exists yet! What if you have to triage bugs?

_Puppet Master is a desktop app built with Electron and React._
