---
title: "Automating Daily Tasks"
layout: post
date: 2017-03-07 16:30
image: /assets/images/profile.jpg
headerImage: false
blog: true
projects: false
tag:
- shortcuts
- command-line
author: michellekim
description: Automating daily tasks
---

![](../assets/images/automating/automating-in-action.gif)

## Summary:

One way to speed up daily routines, or at least make it fun: making command-line shortcuts with aliases.

#### Inspired by:

- [Edmond Lau's book *The Effective Engineer*](http://www.theeffectiveengineer.com/), which I just started reading and got me started thinking about how I could make daily tasks quicker
- Seema Ullal's presentation at Hackbright on Git, especially the portion of her talk on setting up our terminals--[this is an article she referenced](https://medium.com/@mandymadethis/pimp-out-your-command-line-b317cf42e953)

#### How I made my aliases
1. open `~/.bash_profile` with your text editor
1. in the file, type `alias [name]='[whatever command you want to be shortened]'`
1. [From this page](http://apple.stackexchange.com/questions/83630/create-a-terminal-command-to-open-file-with-chrome), I found that you can just use the application name with `'open' -a` and a link to whatever you want the application to open.  This works with opening Spotify with a Spotify URL, such as that of a playlist! Examples:


```alias mcs='open -a "Google Chrome" https://www.youtube.com/user/mycodeschool/playlists'


alias mov_sc='open -a "Spotify" https://open.spotify.com/user/jmichellekim/playlist/5I12pB2PExI0YNbU2tEbhd'
```


Save bash_profile and try it out:
1. Reload or open a new tab in terminal
1. Type just the alias and return


#### Applications
- Email
- Going to a YouTube playlist you frequent
- Playing your favorite Spotify playlist quickly

___
