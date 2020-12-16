---
layout: article
title: How to Convert Scratch Projects to EXE For Free
description: A full walkthrough guide on how to convert Scratch Projects to windows executables (.exe) easily, and for free!
permalink: /convert-scratch-to-exe
thumbnail: public/article-assets/convert-scratch-to-exe/thumb.png
featured: false
category: how-to
tags: [how-to, installation, walkthrough]
---

### Overview
In this guide, you will learn how to convert your Scratch Project into a Windows executable with a free program called Scratch2Gamemaker. Not only will you be able to export your Scratch Project as a Windows Executable, but you will also be able to export for macOS, Linux, mobile, and even HTML5!

### Installing The Program
To convert your Scratch project, we must first install a free program named Scratch2Gamemaker. Go to the [Scratch2Gamemaker download page](https://scratchconvert.com/scratch2gamemaker), and click on the install button. Once your download has completed, navigate to your downloads folder and run the installer by double-clicking it. Simply follow along with the installer, and customize it as you'd like.

Now that Scratch2Gamemaker is installed, run the program by double-clicking the icon on your desktop. If there is no Scratch2Gamemaker icon on your desktop, hit the Windows key and type "Scratch2Gamemaker" and select the first program in the search results.

### Converting Your Scratch Project
Now it's time to convert your Scratch Project! But to do that, we must first prepare it for conversion. Currently, Gamemaker Studio 2 supports vector graphics, but only in the .swf format, not the .svg format that Scratch uses, so unfortunately, we will need to rasterize our art temporarily. Note that there is a workaround for adding vector graphics that we will discuss later. To rasterize your art, simply go to the art editor, and click on the "Convert to Bitmap" button on the bottom-left of the preview panel. It is also worth noting that custom blocks are currently unsupported in Scratch2Gamemaker.

Now that your project is all set for conversion, we are ready to download your Scratch Project. If you are using the web version of Scratch to create your projects, navigate to your game and click "See inside." Once your are in the editor, click on the "File" button on the top tab, and in the dropdown, select "Save to your computer."

![Saving a Scratch Project As a Local File](public/article-assets/convert-scratch-to-exe/save-scratch-project.png)

Now, in the Scratch2Gamemaker program, drag and drop your project file (it should end in .sb3) right onto the Scratch2Gamemaker program where it says "Drag and drop your .sb3 file here.." Once you drag-and-drop the project file into the program, click on the "Convert" button. Please note that this will NOT delete your Scratch Project file, but will rather create a new folder in the directory where the Scratch Project file originates.

Once the conversion finishes, you can navigate to the newly created directory which contains your project's files, which have been converted to Gamemaker Studio 2.

### Installing Gamemaker Studio 2
In order to export your project as a Windows Executable, macOS program, a Linux Executable, or as a HTML5 game, we must first install Gamemaker Studio 2. To do this, go to the [Gamemaker Studio 2 download page](https://accounts.yoyogames.com/downloads) in your browser of choice. You may need to log in or create a Yoyo Games account first. On the downloads page, click "Download" under the "Windows IDE" section.

![Installing Gamemaker Studio 2](public/article-assets/convert-scratch-to-exe/download-gamemaker.png)

In your downloads folder, run the Gamemaker Studio 2 Installer by double-clicking it, like last time, simply follow along with the installer. Once the installation has finished, navigate to your converted Scratch Project's directory and double-click the .yyz file.

### Exporting your Scratch Project as a Windows Executable
Now that your Scratch Project is converted and Gamemaker Studio 2 is installed, all you have to do now is export your project! You can do that with ease by clicking on the "Build" dropdown, and selecting "Create Executable."

Now have to choose in what format you want you want it to be exported as-- either an installer or a .zip file. With an installer, the user will get an .exe installer file which they will have to go through before they can play your game. With a zip file, the user will not have to go through a setup process, but they will have to extract the zip and run the exe file. For now, let's package it as an installer by clicking "Package as Installer." Select the location you want to compile it to, and click "save." The program is now compiling! Once the compile completes, all you need to do is run the .exe file.

### How to use vector graphics
Unfortunately, Gamemaker Studio 2's vector graphics are limited to .swf files only. So, you'll have to convert them from .svg files to .swf files. Fortunately, there is a free program called [svg2swf](http://svg2swf.sourceforge.net/) which you can use to convert your svg files to swf files. To import swf files, double-click on the desired sprite located in the Asset Browser, and click the "Import" button in the newly created window.

### Changing the window size
If you want to change your program's window size, simply navigate to the room asset titled "rm_game" and double-click it. In the room editor under the "properties" pane, click on the "Creation Code" button. This should bring you to a window with code that looks like the following:

```
/// Creation code

// Resize the window to native Scratch resolution
window_set_size(480, 360);

```

This code will resize the window to whatever size you input (width as the first value, and height as the second.) You *could* set it to resize to 1920x1080, but that will leave black bars on the left and right sides of the window. To prevent black bars from appearing, make sure you keep it at a 4:3 aspect ratio.

### Other customizations
**To change the FPS from Scratch's default 30**, go to the "Game Options" panel by clicking the little gear icon at the top of your screen. Under the "General" tab, look for the input box labeled "Game frames per second", and change it to whatever you desire, giving your game a smoother feel.

**To change the default window name** from the default "Converted With Scratch2Gamemaker", go to the "Game Options" panel by clicking the gear icon at the top of your screen. Under the "Platform Settings > Windows" tab, you can change the product information from the default values.