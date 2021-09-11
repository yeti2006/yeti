---
title: "SpotiLike"
toc: true
---

# Welcome to SpotiLike

My favourite project of em all.

 If you're looking for my first attempt in this project(the one which requires config file typing), I suggest you head over to [Version 1](/docs/spotilike_/spotilikev1)

{{< button "https://github.com/yeti2006/SpotiLike/releases/download/2.0/SpotiLike_v2.0.exe" "Download SpotiLike">}}
{{< button "https://github.com/yeti2006/SpotiLike" "Source Repo">}}
<br>

## What is SpotiLike?

`SpotiLike` is a simple application that allows you to configure custom keyboard shortcuts(hotkeys), that's gonna let you add songs to your private playlists, or your own personal liked songs library in [**Spotify**](https://spotify.com/), while you're listening to them.

Doesn't make sense?

Ok, imagine you're gaming whilst listening to Spotify, then a track that's of your deep interest comes to view. You may want to save that track to a custom playlist or just like it -> to add to your Liked Songs library. Returning to the Spotify application could be troublesome and annoying.

To overcome this, this application might be your aid; you can save them with your keyboard!

## But...why?

I created this project cause' I needed a way to save my songs as a collection with my keyboard, without returning to the Spotify application while listening.

As Spotify itself doesn't provide this functionality, I tried to find a solution.. but, I didn't find a solution that matched my requirements so I attempted to come up with my own.

The reason I found this annoying is because returning to the Spotify application interrupted my workflow, and I didn't want to miss that cool song too ¯\\\_(ツ)_/¯

This might come in handy if you're a gamer and loves music.

## How2Use

The application is pretty straight forward. All you gotta do is type out your hotkey with `+` as the separator.

After installation when you first start the app after authorizing your account, it would look like:

![SpotiLike_Initial](/images/SpotiLike_GXXFfYVj2m.png)

The application is now in a state of fetching all of your private playlists. Once that is done, you will be able to see all of your playlists when you click the drop down.

{{< tip "warning" >}}
Please note that it might take some time for the application to start the first time you open it. It attempts to download all the icons of your playlists. Well, this depends mostly on your interent connection.
{{< /tip >}}

![SotiLike_dropdown](/images/Dropdown.png)

{{< tip "warning" >}}
Also keep in mind to not close the application when it's fetching. This is a bug that I didn't fix (sorry)
{{< /tip >}}

## Configuring the hotkeys

And now, all you have to do is type out your hotkey using "`+`" as the separator.

For instance, if you want to _like_ your current playing song when you press `ctrl` and `l` together, the value would be **`ctrl+l`** selecting `Saved Songs` in the drop down.

Here's what I use to save a song to my playlist named **Chill**:

![Chill_hotkey](/images/SpotiLike_zu54lTX5VA.png)

{{< tip >}}
Closing the application would automatically save it to the System Tray. Wanna get it back again or close it? Right click the tray icon and you'll see a list of options.
{{< /tip >}}

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



**Startup**

When you install the application, the app would automatically register itself as a start up application. This means it would open itself when you log in to Windows. 

Don't like startup apps? You can disable it by opening Task Manager: navigate to the startup tab, find SpotiLike, right click and disable.

## Available Keys

The hotkeys can be literally anything you want. Even `a+b` works. 

Below given are a list of keys that are available so far. 

```
alt
backspace
caps_lock
ctrl     
cmd      
delete   
down     
end      
enter    
esc      
f1       
f10      
f11      
f12      
f13      
f14      
f15      
f16      
f17      
f18      
f19      
f2
f20
f3
f4
f5
f6
f7
f8
f9
home
insert
left
media_next
media_play_pause
media_previous
media_volume_down
media_volume_mute
media_volume_up
menu
num_lock
page_down
page_up
pause
print_screen
right
scroll_lock
shift
space
tab
up
```

_I can't find `media_next` keys in my keyboard..help!_ Those keys have special functions. Most keyboards have the functionality to skip the current playing song using a function key. F5 and F6 in most keyboards act as them. Even some headphones have this functionality too. You can specify these too so you can maybe save songs using your headset? Iunno.

{{< tip >}}
To avoid possible errors, when you enter a key as a hotkey the application goes through a matching process to match to the nearest existing key. For instance, if you type `ct+l` the application would error internally as a key called 'ct' doesn't exist. The closest match would be `ctrl` so the application would take it as `ctrl+l` internally.<br>
TL;DR: `ct+l` works as `ctrl+l`.
{{< /tip >}}