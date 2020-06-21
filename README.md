# Dustforce Recolour

## Installation
**Windows 64bit:**
- Download {INSERT LINK TO LATEST FULL ZIP}, which contains everything needed to run the app.
- Extract the zip file to any location.
- Run **Dustforce Recolour.exe**.

**Other/Manual:**
- Download the appropriate version of [NW.js](https://nwjs.io/) for your operating system.
- The current version of NW.js the app uses is **0.46.0**, so that or most newer versions should work.
- Extract to any location.
- Download {LINK TO JUST PACKAGE.NW ZIP}.
- Extract that into the NW.js directory.
- Run NW.js (**nw.exe** on Windows)

## Loading Into Dustforce
- Click the **Render** button.
- Once rendering has completed, the folder containing the new sprites should automatically open.
- Paste the new folder into **/content_src/sprites** in your Dustforce install location.    
  A valid folder path will look like this: **content_src/sprites/player/dustman/**
- Open **/content/sprites** and delete (or rename) the corresponding sprite file, eg. **/content/sprites/dustman**
- Run Dustforce and a new sprite file will be generated from the custom sprites in **content_src**/

** .rar archive with every sprite in the game: https://www.dropbox.com/s/11pa1cdqhv68etv/sprites.rar?dl=0

## Hats
**Ctrl + Click** a hat image to delete it.

### SVG Hats
It is possible to load an svg file as a custom hat.  
If it is being rendered at the incorrect size, explicitly setting the width and height may help.  
eg. change this:  
`<svg viewBox="0 0 26.393 20.545">`  
to this:  
`<svg viewBox="0 0 26.393 20.545" width="26.393" height="20.545">`

## Replacements
Some important things to take note of:
- To start, use the export template buttons to create template svg files to edit.  
- The template will contain **template_origin** and **template_bounds** objects that are required for alignment when importing and should not be modified or deleted.  
- The image viewport (eg. called an art board in Illustrator) should contain all artwork, and ideally fit it as closely as possible
- A preview image will also be included that should be deleted once it's no longer needed.
- Dustworth's **Vacuum Generic** is stretched vertically slightly, so the artwork will need to be drawn squashed.