---
layout: single
title:  "Improving Gnome notifications"
date:   "2019-08-04T23:24:00"
---
I've moved from the Slack Electron app to its web version, because the Slack window was constantly breaking in my desktop. It works better in the browser, but I was really missing the new message's icon in my desktop.

The web notifications I get in Gnome 3 for slack messages are just pop-ups that show up for a moment, then disappear forever. There is no alert icon to remember me that those important messages are laying in Slack, just waiting for me to answering them, or to react to them with the coolest emoji available.

Luckily, there are Gnome extensions available to fix that mess!

If you've never installed Gnome extensions before, you may usually install them from your distro package repositories, or directly from the Gnome website.

I prefer installing them from the website, because there are only a few extensions in my distro default repositories, and they are usually outdated. If you want to do the same, you'll have to setup the Gnome extension's integration for your browser.

1. If you're using a Debian based distro and Chrome, you must ```sudo apt-get install chrome-gnome-shell```
2. But if you're using a Debian based distro and Firefox, you must ```sudo apt-get install chrome-gnome-shell``` AND install the [GNOME Shell integration plugin][gnome-shell-integration]
3. And if, perhaps, you're using anything else, I wish you the best of luck.

You can go to the [Gnome extensions website](https://extensions.gnome.org/) now. If you use Gnome in multiple computers, you probably want to create a Gnome account now, so you can synchronize your installed extensions.

Now let's fix the damn notifications, right? Hell yeah.

Install the [Notification Center](https://extensions.gnome.org/extension/1526/notification-centerselenium-h/) extension, so you will have a nice bell icon in your top bar if you have any unread notifications, and will get a dot indicator every time you have new unread messages.

Finally, install the [Grown up notifications](https://extensions.gnome.org/extension/1335/grown-up-notifications/) extension, so Slack will stop deleting its own notifications and they will stop disappearing from your notification area. I had to restart my computer to get this one working.

That's all, congratulations, you're the brand new owner of a beautiful notification center in your Gnome 3 desktop.

[gnome-shell-integration]: https://addons.mozilla.org/en-US/firefox/addon/gnome-shell-integration/
[github]: https://github.com/
