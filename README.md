# Puppet Master

Puppet Master is a desktop app built with Electron and React.

The app has a big red button. When you click this button it searches your computer for the first install of Google Chrome it can find, then it spawwns an entirely new instance of Chrome that has no cache, no cookies, no profile, no storage. If you click the button multiple times you will get multiple instances of Chrome, all of which are in context isolation from each other. This means you can sign into the same site with mutliple different users on the different versions of Chrome! The app connects to each version via websocket and shows you a preview of its screen which updates automatically.

But theres more... There is code editor, any puppeteer automation code you write in the code editor can be executed on any of the new browsers you created. Unlike regular browser test automation software with puppet master you can continue to use the browser while it is executing automation code. SO you can use the code a sophisticated shortcut and continue using the browser normally.

Theres even more... There are environment variables and preload scripts that allow you to create complex wrapper methods for your automation script meaning it is even easier and faster and more convenient to write. Since this app has an integrated file system you can store your automation code in multiple files, perhaps corresponding to each of your projects and have different environment variables and preload scripts for each.

There is even more... Any data can be extraced from the page and added to the "log" object. The log object is a POJO (Plain Old Javascript Object) that is in scope all the time. Just add properties to it as you like and they will be visible in the out put window. Perfect for Web Scraping!

There is even more...You can use the "require()" function in any of your scripts and it will look for a node_modules folder at the top level of the currently open folder. So you can create complex scripts. Why not look up the data for the current user in the database using the script, then log it to the output window WHILE you are browsing, so you have all the data you need to debug any problems with your site!


