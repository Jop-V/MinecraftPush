This is a Minecraft (Bukkit) plugin that allows for push notifications from your Minecraft server via [Pushover](http://www.pushover.net/).

Installation
-----
1. Put the plugin in your plugins folder.
2. Reload or restart your server.

Usage
----
Join and type the command: `/pushover enable <pushover user key>`. Get your Pushover user key by logging in at [Pushover's website](http://www.pushover.net/), copying it, and then pasting it in the chat using <kbd>Ctrl</kbd>+<kbd>V</kbd> or <kbd>⌘</kbd>+<kbd>V</kbd>. Your players can (and should 😀) do this too! Enjoy! Only offline players receive notifications.

You can disable notifications again at any time using `/pushover disable`.

Features
-----

- Get a notification when someone joins or leaves. 📲
   - Custom join/leave messages supported!
- Broadcast to all online players and all offline players with notifications enabled with `/broadcast <message>`. 📢
   - Permission is `minecraftpush.broadcast`; by default all ops can do it.
- [Name changing](https://mojang.com/2014/04/minecraft-1-7-6-pre-release/) ready! 📛
- More features coming! _(probably not unless I rewrite it)_

---------

### Notes for users of very old Minecraft versions (for example Tekkit Classic)
##### On a fairly recent Minecraft version? Don't read this. It doesn't contain anything even remotely useful for you. Otherwise:

- The plugin will crash by default on very old versions, due to Plugin Metrics being incompatible. Change `opt-out` to `true` in config.yml in the Plugin Metrics folder in the plugins folder to fix this.
- When resetting your world, everyone will need to re-enter their Pushover user keys. This is because of the way old Bukkit versions handle player UUID's.

-----

This plugin is powered by [pushover4j](https://github.com/sps/pushover4j).
