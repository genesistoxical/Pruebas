<p align="center"></p>
<p align="center"><a href="#"><img width="115px" src="docs/assets/Logo-115px.png" align="center" alt="Drop Icons"/></a></p>
<h1 align="center">Crystal Folders</h1>
<p align="center">Drop Icons is a utility to convert images to icons (.ico) for Windows, with a simple Drag and Drop feature.</p>

<p align="center">
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/badge/License-MIT-9280FF?style=flat-square&labelColor=343B45"/></a>
 <a href="https://github.com/genesistoxical/drop-icons/releases/latest"><img src="https://img.shields.io/github/v/release/genesistoxical/drop-icons.svg?color=9280FF&label=Release&style=flat-square&labelColor=343B45"/></a>
 <a href="#"><img alt="NET" src="https://img.shields.io/badge/.NET_Framework-4.8-9280FF?style=flat-square&labelColor=343B45"/></a> 
 <a href="/installer%20src"><img alt="Installer" src="https://img.shields.io/badge/Installer-ISS-9280FF?style=flat-square&labelColor=343B45"/></a>
 <a href="#"><img alt="Languages" src="https://img.shields.io/badge/Languages-2-9280FF?style=flat-square&labelColor=343B45"/></a>
</p>

<p align="center">
<a href="README.md">English</a> :speech_balloon: <a href="README-es.md">Español</a>
</p>

## Features
* Customize many folders in seconds.
* Add folders within Documents, Images, etc. with one click.
* Drag and drop option.
* Choose between different default icons or your own.
* Option to include subfolders.
* Possibility to remove directories from the list once added.
* Number of folders and subfolders to customize.
* Option to create portable folders with a custom icon. [𝐢](#details)
* Avoid duplication of folders that have been previously added.
* Notifications directly on the desktop.
* Avoid customizing folders with system icons.
* Switch between English and Spanish language.
* Save settings in a .ini file, except for switches.
* Customize theme color.
* Modifying the Desktop.ini file without losing previous information.
* Adaptive corners (rounded or metro), depending on the OS version.

## Preview
<a href="#"><img src="docs/assets/Drop-Icons-v2.gif"/></a>

## Usage
On the left panel there is an area where the directories or folders list to customize will be displayed. Below we can find icons with their respective checkboxes, which are: Documents, Images, Music, Videos and Desktop.

<br/>

① Add folders, there are two ways:
   * Check the box(es) you want to customize, for example: if you selected Documents, all the folders inside will be added to the list. You can deactivate them at any time to remove those directories.
   * By dragging and dropping folders into the area mentioned above, even if you have already checked boxes.

To remove folders one by one, you must select it in the list and click the ⦵ icon.

② Choose an icon:
   On the right panel press the “Choose…” button, a window will open with different color icons although you could use your own as long as it is in ICO format. Once you select it and press “Open” it will appear in the preview.

③ Add subfolders:
   Further down you can turn on the “Add subfolders” switch, which will also indicate the total number of. If you find there are too many or you are not interested, you could simply turn it off, this only helps to have a better customization experience.

<br/>

>We will skip the second switch for now.

<br/>

④ Customize all:
   Finally, press the “Customize” button, which, likewise, indicates the total number of folders whose icons will be changed. Once this is done, a small waiting window will be displayed and then a notification on your desktop confirming that it has completed successfully.

That’s it, it’s that easy! Now all that’s left to do is look at your customized folders; if you don’t see any changes, just refresh or close and reopen the Windows Explorer’s window.

Remember, is not necessary to close the application to clear the list or options you have chosen, just click on the ⟳ button.

<br/>

Restore folders:

① You will have to follow the first steps again; checking the boxes or dragging and dropping them to the list. The difference is: instead of choosing a new icon, you will have to click on the “Restore” button and as you can see, a little arrow will appear in what would be the preview, to indicate this action.

② You will notice the switch below has changed to “Restore subfolders,” turn that on if you’ve customized them before.

③ Finally, click on the “Restore” button. The small waiting window will appear again, then the notification on the desktop that it has been completed and that’s it, your folders are back to normal.

<br/>

Folders with customized icons on another PC:

The second switch “Configure to portable” allows you to customize the icon for up to 30 folders (including subfolders) to be displayed with that icon on any other computer, since it copies it inside. This option only works by dragging them to the list area; If any box is checked on the left panel, the switch cannot be turned on.

In the same way, when restoring a folder with a portable icon you will need to follow the same steps, just remember to turn on the “Restore from portable” switch.

<br/>

Crystal Folders also has some security measures:

* You cannot customize special folders that already have a system icon, such as “Documents”, only directories within it.
* There are folders whose icon cannot be changed due to their protection level or privileges, so a notification will be displayed on the desktop warning about how many have been skipped.
* It directly modifies the Desktop.ini file, thus avoiding deleting it and creating a new one, without losing its information.

<br/>

<br id="details"/>
By clicking on the upper Info button, a new window will appear in which you can:

- **Change theme:** Click on `Change Theme` to open the color picker and choose a custom one, then click Apply. To return to default values, repeat the previous steps and press the purple button below the tone selector. Finally click Apply.

- **Change language:** In the **Language** section below, click on the little arrows icon to change between English or Español, finally click on the return button to apply and see changes.

- **Format:** Clicking on `Format` will display a menu with two options to choose the sizes that will be included within the icon: **Multiple** generates a high quality icon that include all necessary sizes such as 16, 32, 48, 64, 128 and 256 pixels, although the output dimensions will be 16px. The last option is **256 px** which generates an icon with a single size but look pixelated in the details view.
     >Note: If the **Generate tiny icon** switch is on, a small icon will be created regardless of its format.
     
- **Third-party content:** On the left side are the names of each library, project, icons or fonts that were used, click one to read its license and author(s), as well as a short description. You can click on the clip icon to go to each repository/official site and change pages with **Next 🢖🢖** or **🢔🢔 Back**.

## Options
<a href="#"><img src="docs/assets/Drop-Icons-Options-v2.gif"/></a>

## Installer
To compile the installer you need [Inno Setup](https://jrsoftware.org/isinfo.php), the files are located in the [installer src](/installer%20src) folder. You just need to open the project (Installer.iss) and compile it, unless you want to make a change. When finished, it will leave a folder called Output in the same location.

>* You must first compile the source code in Visual Studio to get the binaries, otherwise, you will get a [📍Compiler Error](https://github.com/genesistoxical/drop-icons/issues/3).
>* ⬇️ Alternatively, you can download the compiled app from the Drop Icons [page](https://genesistoxical.github.io/drop-icons/).

**Portable with 7zip.bat** allows you to quickly zip the portable version. It only works with [7zip](https://www.7-zip.org/).

Both .iss and .bat get the files that are needed within their folder and/or the Release folder (because of relative paths).

## Contributing
* **HandyControls** package will no longer be updated (for now or permanently) as the latest version does not allow resizing of ToggleButtonSwitch.
* If you make comments in the code, preferably in Spanish, please.
* Variable names must be in English.
* If you open an **Issue**, it can be in English o Spanish.
* **Pull request** in English, in the description you can add details in English or Spanish.
* When converting **.svg** it is first converted to **.png** in a temporary folder and then from **.png** to icon. The priority would be **.svg** "directly" to icon.
  
## Config
`Config.ini` file stores information about the language, theme color, icon format and whether or not the Topmost option is enabled.

~~~
[Options]
Language = en
Topmost = false

[Theme]
#FF9280FF

[Format]
Size = multiple
~~~

>Note: The two switch-type options are not saved because they are not options that are usually activated all the time.

## Adaptive corners
<a href="#"><img src="docs/assets/Drop-Icons-Corners-v2.png"/></a>

## Credits
Drop Icons is based on [Iconizer](https://github.com/willnode/Iconizer) under [MIT License](https://github.com/willnode/Iconizer/blob/master/LICENSE).

* [HandyControls](https://github.com/ghost1372/HandyControls) under [MIT License](https://github.com/ghost1372/HandyControls/blob/develop/LICENSE).

* [FolderBrowserEx](https://github.com/evaristocuesta/FolderBrowserEx) library under [MIT License](https://github.com/evaristocuesta/FolderBrowserEx/blob/master/LICENSE).

* [Noto Music](https://fonts.google.com/noto/specimen/Noto+Music) under [SIL Open Font License](/src/DropIcons/Docs/Noto%20Music/OFL.txt).

* Icons are part of [Teenyicons](https://github.com/teenyicons/teenyicons) under [MIT License](https://github.com/teenyicons/teenyicons/blob/master/LICENSE).

* [SharpVectors](https://github.com/ElinamLLC/SharpVectors/) under [BSD 3-Clause](https://github.com/ElinamLLC/SharpVectors/blob/master/License.md).

* [WinVersion](https://github.com/shaovoon/win_version_detection) detection under [MIT License](https://github.com/shaovoon/win_version_detection/blob/main/LICENSE).

*You can find all licenses [here](/src/DropIcons/Docs).*

## License
**MIT License**

Copyright (c) 2022 - 2023 Génesis Toxical ([read here](LICENSE)).

<br>

## Related:

`🩷 Image to Icon` Convert image to icon online: [`imagetoicon.glitch.me`](https://imagetoicon.glitch.me/) or [`Repository`](https://github.com/genesistoxical/imagetoicon).

`🩷 Pixie Folders` Set of six minimalist and editable folder icon designs: [`Download`](https://genesistoxical.github.io/pixie-folders/) or [`Repository`](https://github.com/genesistoxical/pixie-folders).
