<h1 align="center">
  <img src="logo_node.png" alt="Nocturnal Owl De-vertice Editor">
	<br>
</h1>
<center>
2016 - 2021, Konisbored

[Release Thread][rt] · [Old Release Thread][ort] · [ModWorkshop Page][mws] · [Changelog][cl]
</center>

<!--
To Konisbored or any other contributor:

remove my mess of comments here after you read the entire file. it's basically the node readme rewritten in Markdown and some stuff too for GitHub (change the embedded HTML to BBCode for ModWorkshop). feel free to implement my plans or improve over them,
2.2s is indeed my planned final version, flash is dead and soon i wanna make a better NODE
probably written in HTML/JS when i'm back, or you guys could do that. i say that since C++/C# may
be hard and JavaScript may be a better alternative and you could just use Electron or the web
browser, plus JS and AS use both ECMAScript standards so it won't be much of a hassle to rewrite from scratch, minus: offscreen vertices, Show All Vertices/Path Preview, etc. And for the MWS site, just upload a separate NODE "mod" and append the version number to the end
-->

[rt]: https://spherematchers.boards.net/thread/62/nocturnal-devertice-editor-luxor-creator
[ort]: http://spherematchers.proboards.com/thread/413/nocturnal-devertice-editor-luxor-creator
[mws]: https://modworkshop.net/mod/29923
[cl]: CHANGELOG.md

> ### 🥀 **2.2s will be the final release of N.O.D.E!** See [N.O.D.E: End of Life](#node-end-of-life) for more details.

| Info            | Status                    |
| --------------- | ------------------------- |
| Current Version | 2.2s                      |
| Status          | Final Release             |
| Release Date    | ?????????????????         |

# Table of Contents
1. [Introduction](#introduction)
2. [N.O.D.E: End of Life](#node-end-of-life)
3. [What is N.O.D.E?](#what-is-node)
4. [Game Support](#game-support)
5. [Feature List](#feature-list)
6. [How To Run](#how-to-run)
7. [File List](#file-list)
8. [System Requirements](#system-requirements)
9. [Troubleshooting](#troubleshooting)
10. [Contact Me](#contact-me)
11. [License](#license)
12. [Acknowledgements](#acknowledgements)

# Introduction
If you have this program, or if you're looking at this paragraph right now,
chances are that you are interested in creating your Luxor mods. If so,
welcome to the Sphere Matchers community!
Marble poppers are both easy to pick up and play, but hard to master. With 
that said, that genre of games never had the most active modding community...
until now that is.

# N.O.D.E: End of Life
Since Flash has been dropped since December 2020, 2.2s will be the **final version**
of N.O.D.E.

<!-- if someone else will publish this in my behalf, change this up
make it say that I had to disappear for personal reasons BUT DONT MENTION
THE EXACT REASON WHY!!! -->

## Why was N.O.D.E coded in Flash in the first place?
The original coder, Konisbored, probably was only proficient at ActionScript.
Now, I don't know what else he knew during that time. Granted, ActionScript
is **very** similar to JavaScript. However, Flash's animation aspect is
easier to work with in a glance than attempting to create everything in HTML.
Plus, N.O.D.E was created ~4 years before Flash has been discontinued. It
was probably a choice of familiarity.

## But why did 2.1c exist before then? And why not release this after 2.1c?
It was a fork by someone else who wanted to improve on N.O.D.E. Meanwhile,
the forker, CrushyGreenRen, disappeared from the internet due to personal
reasons. I only stepped in since I had ideas that may or may not help
modders.
<!-- FUCKING HELP ME UGH WHY DID THIS SHIT HAPPEN TO ME FUCKING HELL -->

## Wait. 2.1c's a fork right? Why are you guys treating the 2.1c fork and this version as official?
The original coder, Konisbored, no longer actively works on this program.
So thus, these two forks are pretty much considered "official", regardless
if they are actually forks or not.

## If you knew Flash has been discontinued, then why release this version?
<!-- because i'm actually the missing forker and was held at gunpoint to
     deny internet privileges because being true to yourself is a fucking
     sin appaprently LIJSDUHKESDRHJKBESTRJHKBER56409ibn5i7bb ui567bnu85ny 
     and alsO FORCE YOUR BELIEFS ON SOMEONE ELSE SDKJFNFHSDJKBSFHDJBERGHJB
     HAHA HAHA LOL XD GO TO HELL STUPID ME FOR BELIEVING IN WHAT I WANT
     AND LOVING WHO I WANT LOL XXFDTASDFHGYDASVHJGFHGJSVFGHGH
     ALL I DO IS MAKE LOTS OF SIDE PROJECTS TO KEEP ME SANE ALL DAY HELP -->
For one, it's harder to recreate everything in this program from scratch,
especially in another programming language. So it's better to work with
it for now, until the decision to recreate this program has been made.
Which well, has been made. Yeah.

When a door closes, another one opens. If you're interested,
feel free to check out **NeoNODE**, which is a project aiming to recreate
(and build upon) the concept of N.O.D.E using HTML and JavaScript.

http://github.com/Shambles_SM/NeoNODE
<!-- actually doesn't fuckign exist because HAHA FUCK YOU

     i actually have two "versions" of this conceptual NODE successor, one
     written in C#, which I'm not really proficient in, and in JavaScript which
     might make more sense to create in since after all, NODE was created in
     Flash, Flash has ActionScript, and both AS and JS are based on ECMAScript.

     and the name "NeoNODE" might be really ugly, i thought of "SphereMapper"
     but it's ambiguous with "SphereMatchers". I can't use "NODE.js" as well
     for obvious reasons.
     
     i have nowhere to vent to -->

# What is N.O.D.E?
N.O.D.E is short for Nocturnal Owl Devertice Editor. It is a program that
provides a custom workstation for simplifying the process of creating your own
paths for Luxor, and more!
Why should you use N.O.D.E?
- simplifies the path making process by automatically logging vertices with a
  simple mouse click instead of the old copy and paste method.
- reduce human errors in path making by having N.O.D.E generate the path.obj,
  map.ui and stage_select.uis file output for you.
- curved paths and corner vertices are MUCH easier & less time consuming to map.
- drastically speeds up path making and hence, the mod creation process.
- imports paths from other Luxor games for you to edit easily!
- new features are constantly being updated and added.
- a logger to replace Clippy.
- completely freeware. Credit to me and N.O.D.E in your mod is optional.

With the release of this program, custom paths are much less
time consuming to make, which makes the process of path modding
less daunting, which means more people will get into the marble popper modding
community, and revitalise the genre through fan level mods.

> *Marble poppers were a dying niche. They were popular in the 2000s but have all
but died out with the turn of the decade. Interest in them has however been
revived through the Sphere Matchers forums, whom decoded how the .obj path files
work in Luxor, allowing it to be edited for custom paths. (I think the main
reason is people wanted to try to make more challenging paths)
So, I tried dabbling into modding Luxor Amun Rising paths myself but along
the way I realised that with the current method, it is extremely tedious to
copy the node points one by one from GIMP to Notepad.
Hence, me being lazy, I decided to streamline the process. While coding a
reverse face-path app, I caught the attention of site administrator Bobik,
whom suggested a full custom application for custom node tracking. After
chatting via PM the concept turned into the full fetched Luxor path creator
you see today, N.O.D.E!*

Ever since it's v1.0 beta release on 13 Aug 2016, N.O.D.E has been an invaluable
tool for every Luxor modder. It is now the tried and tested program for making maps
for almost every Luxor mod.

Check out Luxor mods **[HERE!](https://modworkshop.net/game/luxor)**

N.O.D.E is completely FREE - no money required, and crediting N.O.D.E and Konisbored in your mod if you use it for creating your own paths is COMPLETELY optional!

# Game Support
Luxor games supported as of this version:

| Features                | Games                                                              |
| ----------------------- | ------------------------------------------------------------------ |
| `path.obj` output       | Luxor 1, Amun Rising, 2*, 5th Passage                              |
| `map.ui` output         | Luxor 1, Amun Rising                                               |
| `rules.gvf` output      | Luxor 2                                                            |
| `level_x_y.lvl` output  | Luxor 1, Amun Rising                                               |
| `stage###.xml` output   | Sparkle                                                            |
| Stage Select output     | Luxor 1, Amun Rising                                               |
| Path Import             | N.O.D.E/mod paths, Luxor 1, Amun Rising, 2, 5th Passage, Evolved   |

\*Z-axis not properly supported

# Feature List
Full N.O.D.E Feature List. Here's a summary of what N.O.D.E can do!

- Automatic one-click mapping of vertices points by clicking left mouse key
- Removal of latest vertice by hitting `Delete`
- Manual vertice insertion
- `background.jpg` importing
- `path.obj` exporting & importing
- Sparkle `stage###.xml` exporting
- `map.ui` (1/AR) and `rules.gvf` (2) exporting
- Luxor 1/AR Stage Select exporting
- Customizable path outline thickness & color
- Luxor 1/AR `level_x_y.lvl` export
- Toggleable ustom cursor for easier tracing
- Hidden & Warp vertices
- -500px shooter area bleed warning
- Move entire path

For more details, bugs, bugfixes or changes, refer to the [CHANGELOG](CHANGELOG.md).

# How to Run
Since Flash is no longer supported, and assuming you run on a Windows machine,
just open the exe file. It's just a projector file running the N.O.D.E swf file,
so there's no need to scavenge through the Internet for an old Flash version that
doesn't redirect you to the Macromedia web site.

If you run on a Macintosh, open the swf file if you have a Flash projector.

# File List
The following files should be in the downloaded N.O.D.E directory:
* background.jpg
* changelog.txt
* letter_n.ico
* gpl-3.0.txt
* logo_node.png
* N.O.D.E v2.1c.exe
* N.O.D.E v2.1c.html
* N.O.D.E v2.1c.swf
* pyramid_top.jpg (from Bobik's Galactic Space Journey mod)
* pyramid_top_alpha.tga
* pyramid_top.spr
* stage_map.jpg
* and this ReadMe.txt file

Those three pyramid files are included with N.O.D.E if you wish to have a top-facing pyramid in your mod, which Luxor 1/AR does not have in vanilla.

If any of the above files are missing, try re-downloading from the original
release thread: http://spherematchers.proboards.com/thread/413/nocturnal-devertice-editor-luxor-creator
or the ModWorkshop page: https://modworkshop.net/mod/29923

# System Requirements
Minimum Requirements:
- Operating System:
  - Windows - Windows 2000, XP, Vista, 7, 8.x and 10.
  - Macintosh - Mac OS X v10.3 and above.
- Disk space: 286MB available disk space.
- Screen Resolution: 1366x768 display.
- CPU: 1.6GHz Intel Pentium 4 processor.
- Memory: 512MB RAM, 128MB graphics memory.

Recommended Requirements:
- Operating System:
  - Windows - Windows 7, 8.x and 10.
  - Macintosh - Mac OS X v10.6 and above.
- Disk space: 1GB available disk space.
- Screen Resolution: 1600x900 display.
- CPU: 2.16GHz Intel Celeron N2840 processor.
- Memory: 2GB RAM, 256 MB graphics memory.

Software Requirements:
Only for HTML/swf version - A standalone Flash player, or an old version of
Flash for a web browser that still supports Flash.

# Troubleshooting

## I see 3 "Nocturnal Owl Devertice Editor" files! Which do I run?
Run the Adobe Projector (.exe) file first. (if using Windows) This does not
require Flash Player.
If it does not work, the other files are both fallbacks. This requires a web
browser with Flash Player or Shockwave Player, however.

## Mac user. How do I open the .swf file?
If you have Shockwave Player, simply double click it. Else, download a
standalone player. If it's for Windows, open with Wine. Or you could
just open the included projector with Wine.

## Flash Player nags about Internet access!
If you are using the standalone Adobe Flash Player and a dialog pops
up about a security warning, follow these steps:
  - Click on Settings.
  - Go to Advanced > Trusted Location Settings...
  - Click on "Add...", then click "Add Folder...".
  - Navigate to the N.O.D.E swf file (or select the drive where
    N.O.D.E is on) and click OK.
  - Click on OK for the Trusted Location settings dialog.
  - Restart the swf file.

## I can't use the HTML file!
Most likely you're using the latest version of your browser, which likely
tells you that Flash is no longer supported , or you're seeing the Macromedia redirect.
In that case, either:
- find an old version of Flash AND an old version of some browser that supports Flash.
- open the swf file in a Flash projector.

## The application is too big and auto-downscaled and all my coordinates are wonky!
Do not rescale the application! Try increasing your screen resolution, full
screen (F11) if using a web browser, or hiding the Windows taskbar and then
restarting N.O.D.E.
Use the .html version instead of the .exe version if it does not fit since I
believe the .html version has scrolling support.
I have tried to cater between a nice screen resolution and program size, but
I recommend a minimum 1366x768 resolution (which is pretty standard by now)
to avoid any errors.

## But I'm using Linux as my OS!
Adobe doesn't support Flash in Linux since Flash Player 11.2, so it's possible
that there might be some issues, although it's unlikely since I'm coding with
Actionscript 2 and Flash 8, a very backdated version.

## I can't seem to get pixel-perfect inputs!
If you're using a touchpad, or if your mouse feels too sensitive, or if your
hands jitter every time you try to place a vertice, you can try using Magnifier,
if you're on Windows. That and the custom cursor greatly helps! You can also
try lowering the mouse speed in your mouse settings, or if you have a DPI
button in your mouse, use it!

## Ctrl-F compatilibity support! :)
If you're a Flash nut, you know Ctrl-F in Shockwave Player is
fullscreen. It'll go fullscreen, but not be scaled up to prevent the vertice
coordinates from being messed up.

## Custom resolution size and rescaling support! :D
See above. Yeah, not happening.

## The program is slow and skipping frames!
Go to Options and change Quality options to Low or Medium. I don't recommend
this, however, as it lowers accuracy of the bitmaps generated.

# Contact Me
With the end-of-life discussion being had, bugfixes are highly unlikely,
but you are free to comment on the ModWorkshop page.

If you want a more quick response, my Discord is Shambles#3117. You're also
free to join the Sphere Matchers Discord server for further support:
https://discord.gg/gJgy5x5

# License
GPL v3. See the [LICENSE](LICENSE).

# Acknowledgements
- Konisbored, for coding the original software.
- MumboJumbo, for creating the Luxor series. (no duh)
- Bobik, for giving the original idea, and to Stage13-10 & Caffeine
  for being the reason Konis picked up modding via the community mod (and as a result
  got irritated enough to make this, because lazy.)
- A thumb ups to all of the beta testers and people feedbacking bugs back to me.
  Your feedback has and will continue to help contribute to the stability of N.O.D.E.
- Thanks to the ones who decoded how Luxor map/obj files work, and to the many,
  many folks at the Sphere Matchers forums! I never imagined a forum dedicated
  to this genre of games existed. If it didn't exist, then honestly neither would
  this program.

v2.2s fork by Shambles. Original software by Konisbored.

N.O.D.E is brought to you by:
```
  _________
 /_  ___   \
/o \/o  \   \
\__/\___/   /
 \_\/______/
 /     /\\\\\ 
|     |\\\\\\ 
 \      \\\\\\\ 
   \______/\\\\\
    _||_||_
```
All owls everywhere.

AND
```
       ____        _                       
      / ___| _ __ | |__   ___ _ __ ___     
      \___ \| '_ \| '_ \ / _ \ '__/ _ \    
       ___) | |_) | | | |  __/ | |  __/    
  __  |____/| .__/|_| |_|\___|_|  \___|    
 |  \/  | __|_| |_ ___| |__   ___ _ __ ___ 
 | |\/| |/ _` | __/ __| '_ \ / _ \ '__/ __|
 | |  | | (_| | || (__| | | |  __/ |  \__ \
 |_|  |_|\__,_|\__\___|_| |_|\___|_|  |___/                                           
	       spherematchers.boards.net
```