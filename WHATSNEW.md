# N.O.D.E v2.2s
Release Date: (I Don't Fucking Know)

Status: Final Release

Hope this release of N.O.D.E will be of very great use, as 2.2s will be the final version.

## General Additions
<!--
- **Added an update checker function! (wow, finally)**
  <br>If a new update has been detected, N.O.D.E will notify you at the bottom of the screen, right above the Welcome text.
  You may ignore the update for the current session or turn the update checker off.
  Note: The update checker might not work if you are using the SWF version.
- **Technical:** Added a "Fork" variable to aid with auto-update-checking if you wish to fork NODE despite the fact that Flash is dead.
  This separates the nodeWorkstationVersion and your fork.
-->
- **Brought back the Level Variable generator.** 2-path levels are now supported, and presets actually work.

## Workstation Additions
<!--- //Added a "Flip-Hidden" Node function - useful for 2-2 maps or symmetrical 1-1s that have an intersection where one (part of the) path is above the other instead of marking both areas as hidden. (examples being Pillar of Osiris).
  When the path has been mirrored or flipped either way, the copied Flip-Hidden nodes will be switched from either Visible or Hidden.-->
- **Added Warp Node support!** Luxor 2 modders, this is for you.
  <br>After placing a warp node, N.O.D.E will automatically change to Hidden mode.
  <br>Press X to toggle Warp Mode. Warp nodes will be automatically be marked as Hidden for you.
- **Added an experimental Show All Vertices function!** This uses ActionScript line methods.
  <br>Using lines for the dots instead of drawing individual boxes eases load, though vertices that are close to eachother will look "connected". I tried drawing individual boxes per vertice - it works, but it made N.O.D.E laggier the more vertices you add. :s
- **Added a Sparkle exporter!** Use N.O.D.E for both Luxor and Sparkle mods!
  <br>N.O.D.E will use positive Y-values for this one, as Luxor and Sparkle treat negative Y values differently.
  <br>To export your map as a Sparkle map, hold Alt and click Save. It's quite barebones, though - add the tunnels and shooter positions yourself.
- **Mirrored path creation!** Easily make maps like Ra's Journey to the West and Nepthy's Garden! They can be found in Edit Mode under Path Augmentation > Mirror.
  <br>Keep in mind for mirroring paths by 180° or mirroring paths vertically that the program assumes that your path is properly aligned in the first 500 pixels (i.e. path is centered vertically in a 800x500 area). Since N.O.D.E is for Luxor anyway. 
- **Added Ctrl+Z support.** Delete vertices with the well-known Undo shortcut! (only has support for vertice undoing. making an undo list would be very tricky, AND unlikely)
- **Added Ctrl+S support.** Easily save your maps!
  <br>Ctrl+Alt+S shortcut for Sparkle map export.
- Added warnings for soft limits in the Stage Mapper (logger only).
- More funni easter eggs. Find them yourself.

## Bugfixes
- SM Discord button was clickable in Instructions.
- Clicking the Close button in the Instructions dialog didn't go back to page 1.
- Path preview color preview squares in the N.O.D.E Settings menu didn't go away when settings are reset.
- "Please switch to Trace Mode" message gets called both when you hold down the mouse and release it, causing it to duplicate. Now it respects your settings.

## N.O.D.E Changes
<!-- - Vertice limit can now be set to different values if you're that insane with subpixel vertices: 1000, 1500, 2000 and 2500.
Warning: A lot (and I mean, a lot) of vertices can make the workstation laggy and long loops may make the program unresponsive. Use at own risk. -->
- The vertice limit is now 1000 instead of 999 vertices. (since obj vertices count from ONE, dammit!)
<!-- - Luxor 1/AR map.ui output: Sprite positions are now floored. -->
- Changed Map Name functionality: textbox is toggleable. When editing the map name, hotkeys are disabled.
- Changed Custom Cursor behavior: focusing on the sidebar will now hide it (and vice versa).
- Fixed text box font oversights in the Import Path screen.
- Fixed font oversights in the Map and Stage Map editors.
- Fixed GVF output (removed leading whitespace and set Min/MaxScales to 1.00)
- UI/UX touchups, generally makes everything darker. ~~And look like a BeardLib Editor ripoff!~~
- Minor code optimizations.

## Projector Changes
- Removed built-in menu bar.
- Removed all Flash built-in shortcut functionality, including full screen, next/previous frame and zoom. (Hell yeah!)

## Removals
- Removed leftover music and Random Path Generator code.
- Removed leftover assets from previous versions.