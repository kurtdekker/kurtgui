# kurtgui
Quick-and-dirty temporary replacement for Unity GUIText stuff

NOTE: this uses the old GUI system to "Sorta" replace the GUIText
and GUITexture classes, which went away in Unity2019 or so.

Use at your own peril, see the enclosed license file.

NOTE: This is not a 1-1 replacement, but rather a start.

NOTE: if you have improvements, commit them and send me a pull request!

NOTE: You might be able to replace the existing uses of GUITexture
and GUIText in your own prefabs by hand-editing the GUIDs in your
own files. Do this at your own peril and only with source control!

Some info about Missing script warnings, GUIDs, renaming GUIDs, etc:

https://forum.unity.com/threads/problem-with-git-and-missing-scripts.1090876/#post-7024801
https://forum.unity.com/threads/scriptable-object-data-not-read-after-loading-editor.998413/#post-6487297
https://forum.unity.com/threads/scriptable-object-data-not-read-after-loading-editor.998413/#post-6488230

EVERYTHING in Unity is connected to the above GUID. It is super-easy to inadvertently change it by renaming outside of Unity. Don't do that. Instead:

- close Visual Studio (important!)
- rename the file(s) in Unity
- in Unity do Assets -> Open C# Project to reopen Visual Studio
- now rename the actual classes, and MAKE SURE THE FILE NAMES DO NOT CHANGE!
