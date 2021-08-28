---
title: "SpotiLike v2"
autosize: true
---

# SpotiLike version 2

`SpotiLike` is a simple application that allows you to configure custom keyboard shortcuts(hotkeys), that's gonna let you add songs to your private playlists, or your own personal liked songs library in **Spotify**, while you're listening to them.

## But...what's the point and why?

I created this project cause' I needed a way to save my song collection with my keyboard, without returning to the Spotify application while listening.

As Spotify itself doesn't provide this functionality, I tried to find a solution.. but, I didn't find a solution that matched my requirements so I attempted to come up with my own.

The reason I found this annoying is because returning to the Spotify application interrupted my workflow, and I didn't want to miss that cool song too ¯\\\_(ツ)_/¯

This might come in handy if you're a gamer and loves music.

## How does it work?

The version 2 is pretty straight forward and easy to use.

After you have installed the application through the setup, it's gonna take a while to start up at the first time. As described in the setup's readme:

```fix
The application initially fetches all your playlists and downloads the playlist's icons. This icon downloading part is the reason it might take a while. Well, depends on your interent connection.

After this process is done, you can click the drop down to list all your private playlists. The default selected item would be "Saved Songs" and that's the option for your Liked Songs library. It's ctrl+l by default but you can change it to anything you want.

Don't want a playlist to be "hotkey-d"? By default every playlist's hotkey is set to "None". You can just leave it blank or type none if you don't want a hotkey.

As you might have guessed, the format to do a hotkey is x+y+a+b+c. For example, if you wanted to register a hotkey like ctrl and f, you would type:

ctrl+f in the Hotkey section :)
```
As simple as that.

To register the hotkeys you can either click the "Apply Changes" button or just hit the X to close the application alternatively.<br>
It would minimize itself to the system tray and register your changes!

## Settings

The settings page consists of 4 options, namely:

* Fetch All your playlists
* Fetch Songs on startup
* Show notifications
* Auto Like  With playlists

| Setting   |      Description     
|----------|:-------------: |
| **Fetch All your playlists**         |  This option is enabled by default. Fetches all your private playlists from the API. If you don't wish to enable hotkeys for playlists and just your Liked songs library, consider disabling this setting. _(Faster startup: if disabled)_| 
| **Fetch Songs on startup**|    This option would fetch the first 100 tracks from each of your private playlists. This would allow the application to prevent creating duplicate saves  for a track in the same playlist. Due to a Spotify limitation, if you save a song in a playlist that has that specific song, there would be a duplicate. _(Faster startup: if disabled)_
| **Show notifications**| Allow or disable notifications, when you do a hotkey. 
| **Auto Like With playlists** | Save the song to your liked songs library when you save to a playlist, automatically. If you saved the song to `x` playlist and you want the song to automatically get saved to your library Liked songs library too, consider enabling this option. 

## Errors

...
