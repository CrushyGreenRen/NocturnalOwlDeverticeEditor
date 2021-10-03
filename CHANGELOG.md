# N.O.D.E Changelog

## N.O.D.E v2.2s
**Final release.**<br>
**Release Date:** Nonexistember ??, 20XX

### General Additions
<!--
- **Added an update checker function! (wow, finally)**
  <br>If a new update has been detected, N.O.D.E will notify you at the bottom of the screen, right above the Welcome text.
  You may ignore the update for the current session or turn the update checker off.
  Note: The update checker might not work if you are using the SWF version.
- **Technical:** Added a "Fork" variable to aid with auto-update-checking if you wish to fork NODE despite the fact that Flash is dead.
  This separates the nodeWorkstationVersion and your fork.
-->
- **Brought back the Level Variable generator.** 2-path levels are now supported, and presets actually work.

### Workstation Additions
<!--- //Added a "Flip-Hidden" Node function - useful for 2-2 maps or symmetrical 1-1s that have an intersection where one (part of the) path is above the other instead of marking both areas as hidden. (examples being Pillar of Osiris).
  When the path has been mirrored or flipped either way, the copied Flip-Hidden nodes will be switched from either Visible or Hidden.-->
- **Added Warp Node support!** Luxor 2 modders, this is for you.
  <br>After placing a warp node, N.O.D.E will automatically change to Hidden mode.
  <br>Press X to toggle Warp Mode.
- **Added an experimental Show All Vertices function!** This uses ActionScript line methods.
  <br>Using lines for the dots instead of drawing individual boxes eases load, though vertices that are close to eachother will look "connected". I tried drawing individual boxes per vertice - it works, but it made N.O.D.E laggier the more vertices you add. :s
- **Added a Sparkle exporter!** Use N.O.D.E for both Luxor and Sparkle mods!
  <br>N.O.D.E will use positive Y-values for this one, as Luxor and Sparkle treat negative Y values differently.
  <br>To export your map as a Sparkle map, hold Alt and click Save. It's quite barebones, though!
- **Mirrored path creation!** Easily make maps like Ra's Journey to the West and Nepthy's Garden! They can be found in Edit Mode under Path Augmentation > Mirror.
  <br>Keep in mind for mirroring paths by 180° or mirroring paths vertically that the program assumes that your path is properly aligned in the first 500 pixels (i.e. path is centered vertically in a 800x500 area). Since N.O.D.E is for Luxor anyway. 
- **Added Ctrl+Z support.** Delete vertices with the well-known Undo shortcut! (only has support for vertice undoing. making an undo list would be very tricky, AND unlikely)
- **Added Ctrl+S support.** Easily save your maps!
  <br>Ctrl+Alt+S shortcut for Sparkle map export.
- Added warnings for soft limits in the Stage Mapper (logger only).
- More funni easter eggs. Find them yourself.
- Guess who's back, back again! Re-added Cowlppy in both Workstations (i felt bad for him)

### Bugfixes
- SM Discord button was clickable in Instructions.
- Clicking the Close button in the Instructions dialog didn't go back to page 1.
- Path preview color preview squares in the N.O.D.E Settings menu didn't go away when settings are reset.
- "Please switch to Trace Mode" log message was being triggered twice when you hold down the mouse and release it, causing it to duplicate. Now it respects your settings.

### N.O.D.E Changes
- The vertice limit is now 1000 instead of 999 vertices. (since obj faces are counted from ONE, dammit!)
- Changed Map Name functionality: textbox is toggleable. When editing the map name, hotkeys are disabled.
- Changed Custom Cursor behavior: focusing on the sidebar will now hide it (and vice versa).
- Fixed text box font oversights in the Import Path screen.
- Fixed font oversights in the Map and Stage Map editors.
- Fixed GVF output (removed leading whitespace and set Min/MaxScales to 1.00)
- UI/UX touchups, generally makes everything darker. ~~And look like a BeardLib Editor ripoff!~~
- Minor code optimizations.

### Projector Changes
- Removed built-in menu bar.
- Removed all Flash built-in shortcut functionality, including full screen, next/previous frame and zoom. (Hell yeah!)

### Removals
- Removed leftover music and Random Path Generator code.
- Removed leftover assets from previous versions.

## N.O.D.E v2.1c
**Release Date:** November 20, 2020
### Changes
- MASSIVE UI overhaul, getting rid of an inconsistent and messy UI.
- The EULA has been shred; N.O.D.E now uses GPLv3 with direct permission from the author and is also now open-source.
- Changed texture of sphere cursor and the latest placed vertice cross.
- Initialization now checks if you have a username set instead of checking for user volume.
- Default color is now #2182e5. You can also find this in the Presets.
- Preset color #3d3c3a is now #161616.
- Logger color no longer saves for the current N.O.D.E session when Save is not confirmed.
- Original placeholders for the background and stage_select image have been added.
- Removed mod showcases from instructions (most of them got cancelled or whatever)

### Additions
- Added the ability to customize the Visible and Hidden path line colors.
- Added the ability to set Path Preview Thickness with options of 2 (default), 4, 6, 8, 16 and 32.
- Resetting your data in the Settings menu now ask for confirmation before proceeding. (finally!)
- Added the spr and tga files of the top facing pyramid.

### Removals
- Removed ALL music tracks, which decreased the SWF file's size from 277 MB to 4.42 MB (!!)
  <br>Fun Fact: The fla source file was 1.3 GB - removing those tracks shrunk it to 23.9 MB!
  This removes the vol, tracklist and track commands and the jukebox.
- Removed the ability to pause the editor.
- Removed the Random Path Generator.
- nunya and rowlet/cowlppy have been removed. Yes, Cowlppy had to go. He felt too old to be in N.O.D.E, so old that Konis doesn't even use him as his profile picture anymore! :(
  - Fortunately, Cowlppy's legacy lives on as the outline in the icon.
- The Level Var generator and Luxor 3 segment generator have been removed (or rather, inaccessible by normal means).

### Known Bugs
Major:
- All known major bugs for current features fixed as of v2.0

Minor:
- if there is no background.jpg file in the N.O.D.E folder, N.O.D.E will show
  0% when importing the image. In a .swf file, an error will be returned.
- .exe version cannot import image if path directory contains Unicode symbols.
- when pasting a long vertice list into Import Path, the text will be invisible
  if it is too long. This does not affect importing, thankfully. As of v1.2, the
  textbox has been lengthened to attempt to prevent this as much as possible, and
  tested so that one of the longest Luxor vertice lists, Scroll of Thoth, works
  fine. However, vertice lists with estimated more than 500 vertices, especially
  those with decimals, may still turn invisible when pasted into the text box.
- The saved settings are stored as seperate cookies for the swf and exe files.
- when right click is followed with a Settings command, the mouse cursor will be
  visible with the custom cursor. This is fixed the moment a left click input
  is registered.
- bug regression: Path Importer doesn't load Node=HIDDEN values for non-N.O.D.E
  path.obj files in v1.3 & v2.0: tunnels cannot be imported for non-N.O.D.E paths.

## N.O.D.E v2.0
**Release Date:** 1 Mar 2017
- added Show Vertice Path function to draw a line/curve showing the level path.
- fixed bug where, if "Auto Load BG on Editor Start" is on, the first unload will
  fail; by loading the BG only after 7 frames (~0.1s delay) instead of instantly.
- added inbound parameters, coordinates must be within -400&lt;x&lt;1200 & -1000&lt;y&lt;400.
- fixed Luxor Evolved Import, array split "//1" broken in v1.3 & didn't import.
- lowered vertice limit to 1,000 due to stability of the new Show Path feature.
- fixed bug where auto loading BG would cause fade in to stop at the wrong volume
  due to hotkey scanner being reset by fading in music in 4 frames instead of 20.
- changed all Cowlppy images to the new design by Bastion.
- fixed bug where level variables exporter gives the wrong viseSpeedMidBzLerp
  and viseSpeedMinBzLerp values from dropdown box selection.
- "Auto Load BG on Editor Start" now also loads stage_map.jpg in Stage Mapper.
- added a hotkey enabling/disabling button, fixing bug where entering Map Name
  will interfere with hotkey maps.
- random vertices coordinate range has been changed to -50&lt;x&lt;850, -490&lt;y&lt;50.
- added CTL function "rowlet".
- disabled 2-2 path support in Level Variables as it is broken: returns undefined.
- added Discord Server invite link to main menu and right click context menu.
- fixed numbering of import modes in Path Importer.
- added 21 new music tracks, bringing the total to 163 Jukebox tracks.
- changed Level Variables generator background due to contrasting colors.
- fixed additional anti-aliasing and device font errors.
- added "stage_select.uis" title to Stage Mapper UI.
- made minor logger/editor grammar and punctuation changes.
- *As v1.3 was skipped over public release, it's worth seeing the changes there
  as well.*

## N.O.D.E closed beta v1.3
**Release Date:** 20 Dec 2016
* closed beta release to beta testers by request for compatibility and bug
  testing.
- workstation has custom 32x32 sphere-shaped mouse cursor for greater accuracy!
- program framerate changed from 30fps to 60fps.
- added a Level Variable Creator to batch generate level_txt files.
- map.ui generator now outputs full map.ui file instead of just Node=HIDDEN list
  and pyramid sprite locations.
- added Cowlppy Talking Language (CTL) for command line interaction with Cowlppy.
  Functions "clear", "clock", "track", "tracklist", "nunya" and "vol" were added.
- Node=Hidden vertice import bug fixed, Importer can now remember/load hidden vertices
  from non-N.O.D.E paths. (regressed in v2.0)
- added beta Luxor 3 .LX3TRK segment creator.
- added Luxor Evolved Import support for Path Importer.
- created Enter hotkey for CTL command shortcut.
- revamped random text color code, actual random hex values (A-F) are now generated
  compared to numerical pseudo random numerical 000000-999999 values in v1.25.
- added Map Name textbox to editor as well as default map name which tracks number
  of times N.O.D.E workstation is open.
- music is now seamless when switching tracks if tracks playing are set the same.
- added a username prompt screen on first entry/data deletion.
- added a crash screen and DRM protection to closed beta releases.
- "Auto Load BG on Editor Start" function added, auto loads background.jpg to editor.
- music track number added to Cowlppy introduction message.
- pause function no longer restarts the editor music track when unpaused.
- music handling code rewritten, some tracks changed from .wav to .mp3 to prevent
  memory crash error, tradeoff for perfect loops.
- added 77 new music tracks, bringing the total to 142 Jukebox tracks.
- default workstation log text color changed from teal to dark blue.
- jukebox now allows jumping to specific track.
- changed and revamped jukebox background and design.
- Cowlppy N.O.D.E editor introductory message changed again.
- Fixed Table of Contents bug where Stage Select option shows up twice.
- other minor bug/graphics fixes and changes.
- v1.3 exclusive: vertice limit is set to 9,999 for beta stability testing.

## N.O.D.E nightly build v1.25
**Release Date:** 22 Oct 2016
- added beta Stage Mapper function that generates stage_select.uis output.
- added Face List support to the importer, effectively making N.O.D.E able to
  import all Luxor 1, Amun Rising, 2, mods & 5th Passage files with no problem.
- path.obj files now have custom headers, included generated time.
- fixed the broken HTML N.O.D.E file in v1.2.
- added a "Move All Vertices" function to Edit Mode.
- reduced logger line margin from 2px to 0px for increased visibility,
  increasing maximum visible height from 12 lines to 14 lines.
- added GSJ's custom top facing pyramid option to the map.ui Pyramid Placer.
- restrict input on Enter Vertice List to letter v, 0 through 9, minus sign,
  decimal point & space to try prevent invalid vertice lists from being entered.
- fixed missing output text in Importer frame.
- added a Random Path Generator to Trace Mode.
- added a Cowlppy Text Color option to Options, in hexadecimal color format.
- vertice point turns green in Hidden mode.
- fixed bug where not entering the number of vertices in the textbox of the
  Importer displays the wrong error message.
- lowered vertice limit from 2,500 to 2,000 due to loop unresponsive stability issues.
- changed around many of the Cowlppy error log output texts.
- added On/Off toggle for Auto-Randomize Music on startup, Automatic Pyramid
  Cover, and a "Turn All Music to Pikku-Orava" Acorn Mode function to Config.
- added "Browse Mods" Sphere Matchers hyperlink to right click context menu.
- added Select All Ctrl-A/Cmd-A tip to outputter.
- fixed minor typo: Cowlppy was incorrectly spelt Cowlipy in the introductory
  workstation message. Thanks to Crushy for being the first to notice after I
  did. (and kept my mouth shut)
- added Date/Time function.
- added 26 new music tracks, bringing the total to 65 Jukebox tracks.
- increased rowcount for comboboxes from 5 to 8.
- changed default background jpeg from Khufu's Revenge to an unused Caffeine map,
  and added a stage_map.jpg file: Luxor Mod 2016's map of Oddworld Island.
- added Table of Contents and changed instructions arrows to allow looping
  between the 1st/last pages.
- optimised loop code to prevent freezing with large number of vertices.
- other minor bug/graphics fixes and changes.

## N.O.D.E v1.2
**Release Date:** 10 Sep 2016
- N.O.D.E has moved out of beta phase.
- tunnel support: added option to switch between visible/hidden vertices.
- latest vertice added is now visible in the workstation, marked with a cross
  symbol. (beta "Show Visible Vertices" Function)
- added Map.UI generator, which generates pyramid coordinates and hidden nodes.
- sorta fixed the invisible text bug when a long vertice list is pasted into
  Import Path vertice list textbox by lengthening the textbox width.
- added a function to delete a specific vertice point to Edit Mode.
- new username function to save & reference user name, up to 20 characters.
- added an unload background function to N.O.D.E, fixing the inconvenience of
  restarting N.O.D.E to replace the background.
- option to user customize and choose the tracks playing in N.O.D.E from all
  the music in the Jukebox under Configuration Options.
- changed right click menu, now has 4 URLs which hyper-links to: Sphere Matchers
  Forums, personal Konisbored Youtube channel, N.O.D.E Offical Thread, and
  Konisbored's personal "Cowlppy & The Luxor Scepter" mod.
- fixed music beginning offset bug found in v1.1 by removing the attachSound
  "stream value=true" tag and increasing fade in time in the Jukebox frame.
- minor bugfix: added additional check for config file, N.O.D.E will auto
  create a new config file if the version of N.O.D.E has changed to avoid
  inconsistent variables.
- added a Random Shuffle Wildball to auto-randomize music tracks.
- added a "Reset to Default Settings" button in Config Options.
- enabled and imported complete tracklist into Jukebox Mode, total 39 tracks.
- added hotkeys, B and H keys.
- changed default volume from 100% to 50%.
- fixed bug in v1.1 where N.O.D.E icon is missing in confirmation box.
- Music Track Order ordered changed from date added to alphabetical order.
- fixed minor overlook where pauseNode was called twice when creating path.obj
  file, which was the cause of mild lag when outputting the path file.
- switched most text anti-aliasing from "AA for animation" to "AA for
  readability", ensuring that text is clearer to read.
- added a "Shut Up" button to clear the Cowlppy logger cache.

## N.O.D.E v1.1 beta
**Release Date:** 18 Aug 2016
- added full Edit/Trace mode functionality.
- added manual vertice input in Trace Mode.
- added a flip/mirror path on axis function in Edit Mode.
- added a reverse path function in Edit Mode.
- major bugfix: Import Vertice code revamped! N.O.D.E can now detect if an
  imported path.obj vertice list has garbage values and throws an error message
  specifying the specfic vertice that has the problem. N.O.D.E no longer
  imports any NaN values!
- added Options Menu which saves a configuration file to local cache, saving
  user specified settings.
- added Mute/Volume control in Options Menu.
- graphical and UI touchups.
- added a "Delete All Vertices" button to add to the previous "delete one at a
  time" function in Edit Mode.
- bugfix: touched up fadein sound code loop to fix a glitch where music volume
  is always 100% for 1/30th of a second before changing to user-specified volume.
- fixed bug where flag URL hyperlink to Sphere Matchers only works in the .exe
  version by changing publish settings. Now even .swf and .html versions
  hotlinks to Sphere Matchers. (http://spherematchers.proboards.com/)
- added more error flags/functions to the Cowlppy logger.
- added Change Quality settings to Options Menu.
- minor bugfix: only numerical values are now allowed in the "Enter Number of
  Vertices" textbox in the Import Path frame.
- Music added for path.obj output dialog box: "Luxor 2: Main Menu".
- Music added for Options Frame: "Kirby 64 - The Crystal Shards: Gourmet Race".
- updated instructions, help, and other text files.
- and other minor bug fixes and general code cleanup.

## N.O.D.E v1.0 beta 
**Release Date:** 13 Aug 2016:
- N.O.D.E has moved to beta phase.
- Import Background to Workstation support! N.O.D.E now loads background.jpg
  image files from the parent folder in the workstation!
- new file formats Projector (.exe) and HTML (.html) files added for
  accessibility to people without Adobe Flash or Shockwave Player.
- added an event logger via Cowlipy the Owl, whom doubles as a vertice list logger.
- added a scroll bar and autoscroll feature for dynamic text.
- added basic support for importing path's vertice lists into the N.O.D.E
  editor. (only paths with linearly descending face lists work)
- added an Undo Vertice Function via Delete Key.
- added a Pause Function via P key.
- added a vertice limit of 2,500 to prevent high CPU usage, and possible
  slowdown/crashes with too many vertices - to be used with loadMovieClip+
  getNextHighestDepth to allow a Show Vertice function to work.
- added a pause layer for outputs and instructions, as well as a N.O.D.E
  dialog box.
- fixed scaling bug if users were to fullscreen N.O.D.E in Shockwave by
  disabling scale.
- added an official logo for N.O.D.E
- fixed bug where hotkeys do not work after importing image file - instead of
  _root, hotkey detection functions now mapped to a movie clip and re-called
  after every onEnterFrame() function change.
- music now linked & played using attachSound() via Actionscript instead of
  manually by frames - speed up/code cleanup fix!
- fixed a minor glitch where mouse_x values from 830 to 859 still captures
  vertices although the mouse is in the UI.
- music now fades in gradually with a settable fade in time on call.
- fixed bug where N.O.D.E refuses to read imported path values by using
  parseFloat to convert strings to numbers.
- major graphical touchups.
- added an .ico file for N.O.D.E
- added a warning line when below -500px.
- fixed bug where buttons and functions still enabled when pausing.
- added Jukebox/Sound Test mode.
- added URL to Sphere Matchers forums.
- Music added for editor frame: "Kirby Planet Robobot: True Arena Intermission".
- Music added for instructions_mc: "Kirby Super Star Ultra: Spring Breeze Intro".
- Music added for importer frame: "Kirby Nightmare in Dreamland: Butter Building".
- fixed spelling of Nocturnal from Noctornal (thanks to Bobik for spotting the
  inconsistent typo)
- and other minor bug fixes.

## N.O.D.E v0.1 closed alpha
**Release Date:** 6 Aug 2016
- closed alpha release to beta testers by request for compatibility and bug
  testing.
- most of the fixes and new features in this version are listed under the v1.0
  beta section as this version is not publicly released.

## N.O.D.E v0.01 alpha
Initial release.<br>
**Release Date:** 1 Aug 2016
- X and Y axis mouse coordinate tracker.
- Add vertices points by clicking mouse key in Trace mode.
- Output a complete path.obj file.
- additional 30px around 800x600 main workarea for offscreen nodes.
- SPACE key switches between Trace mode (where you map a path) and Edit mode
  (where it doesn't map) - not useful in alpha
- Music added for Main Menu: "Kirby Super Star Ultra: White Wing Dynablade".
