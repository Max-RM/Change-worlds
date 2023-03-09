
# Change-worlds.
Switch worlds from editor mode to Minecraft preview and and vice versa without export-import.

# Intro.
pay attention. first you have to turn off Minecraft preview and Editor mode (if they are enabled) and only then follow the instructions!

According to Microsoft's instructions  https://learn.microsoft.com/en-us/minecraft/creator/documents/editoroverview#editor-file-operations---create-import-export, to switch the world from editor mode to Minecraft preview and vice versa, you must follow this ##### instruction. But I will show you a more correct way, which I came up with on 03/09/2023, the day after the release of Minecraft preview 1.19.80.02

But why did I call this instruction from Microsoft - #######? it's simple, because imagine that you have created a 5 GB world in Minecraft preview or editor mode and you need to send it to Minecraft preview or editor mode. you will first have to export this world as an archive using game functions, then import it using game functions, and this process, given the size of your world, will take quite a bit of time. It is an absolutely stupid decision on the part of Mojang not to provide for this. in fact, only one NBT tag in the level.dat - (isEditorWorld: 1) file is responsible for the fact that the world will be displayed in the list of worlds editor mode or Minecraft preview its presence or absence will affect whether the world will be in the list of some of the games or not.
and it will only take you a few seconds to edit this NBT tag, which is much more reasonable, so use my instruction, not nonsense from Microsoft!

# Guide.
# Minecraft Prewiev > Editor Mode.
First download (UME) Universal Minecraft Editor from web.archive because Matt G blocked the download from his site: https://web.archive.org/web/20211024121354/https://www.universalminecrafteditor.com/software/UniversalMC_setup.exe?fdl=1
you will need exactly UME because NBT studio and NBT Explorer for some reason believe that the level.dat file from new worlds is empty.

1. Now assuming that you have already created a world in Minecraft Preview and want to send it to Editor mode. You need to open UME and press one of these buttons: ![IMG_20230309_131645](https://user-images.githubusercontent.com/81485476/223963037-8b9ca96b-cb25-4db2-b25b-f1bc97367029.jpg)

2. Then in the window that opens, click this button:

![IMG_20230309_131955](https://user-images.githubusercontent.com/81485476/223962249-19d15a12-77a1-49cf-8182-ec321ebbd9d4.jpg)

3. This window will open:

![IMG_20230309_132513_460](https://user-images.githubusercontent.com/81485476/223963524-d801ec53-57b2-4d5e-b109-692f38f03e59.jpg)

4. The folder is empty because the path of the worlds of Minecraft preview differs from Minecraft retail, and UME always opens the folder: ```C:\Users\(Username of PC)\AppData\Local\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\minecraftWorlds```
so you just need to go to another folder. at the top there is a line with the path to the folder. Click on it with the cursor:

![IMG_20230309_133521](https://user-images.githubusercontent.com/81485476/223966056-9504b81e-e36e-4fe0-97ce-fe31aa6d2bd6.jpg)

5. And then paste this path: ```C:\Users\(Username of PC)\AppData\Local\Packages\Microsoft.MinecraftWindowsBeta_8wekyb3d8bbwe\LocalState\games\com.mojang\minecraftWorlds``` in this line, before paste, replace ```(Username of PC)``` in path with your PC username! then click ⍈:

![IMG_20230309_140513](https://user-images.githubusercontent.com/81485476/223973240-571984e2-fb39-43cb-b930-b026b9831b38.jpg)

6. A folder with your worlds will open. Most likely they will have names from random characters, select the desired world by clicking on the desired folder 1 time, then click - select folder at the bottom right:

![IMG_20230309_141117](https://user-images.githubusercontent.com/81485476/223974773-0bab0f58-3649-4b5f-9977-9bfbee33a426.jpg)

7. In the window that opens, click - open:

![IMG_20230309_141249](https://user-images.githubusercontent.com/81485476/223975154-ae8a64c1-7eb6-4ed6-b508-4dcfbff23dd2.jpg)


8. Your world will open in UME, then click - View Files:

![IMG_20230309_141421](https://user-images.githubusercontent.com/81485476/223975742-85651eee-8518-49ed-9c89-e1ca4bfd1207.jpg)

9. In the window that opens, open the level.dat file:

![IMG_20230309_141738](https://user-images.githubusercontent.com/81485476/223976355-291b9ee6-b864-48de-aede-381c674638d4.jpg)

10. Now copy this text: ```0a00010101000d6973456469746f72576f726c640100```

11. Click on this thing:

![IMG_20230309_141855](https://user-images.githubusercontent.com/81485476/223976672-9c16f796-6e8b-4aa3-a5ff-2c9c9c1b5809.jpg)

12. Then simultaneously press the (ctrl) and (v) buttons on the keyboard. This will add the needed NBT tag to level.dat
Now clink this Button and close UME:

![IMG_20230309_142326](https://user-images.githubusercontent.com/81485476/223977825-4b9a43be-6100-43fd-b3f7-11d295c64ba3.jpg)

now, the next time you open Editor Mode, this world should appear in the list of worlds.

# Editor Mode > Minecraft Preview

If you want your world from Editor Mode to be in the list of Minecraft Preview worlds, you must: 

1. Follow the steps 1-9

2. In level.dat, find ```isEditorWorld: 1``` and delete it by pressing the - ```del``` button on the keyboard:

![IMG_20230309_143412](https://user-images.githubusercontent.com/81485476/223982476-485a67fe-9042-490d-9c08-400a6945de2c.jpg)


3. clink this button and close UME:

![IMG_20230309_142326](https://user-images.githubusercontent.com/81485476/223982601-f27ddad3-152b-4bec-a37d-5aa345c20914.jpg)

Now this world from editor mode should appear in the list of worlds in Minecraft preview.

as you understand, this instruction must be followed every time you want to change Minecraft Preview > Editor Mode, Editor Mode > Minecraft Preview, but it will still be faster than export-import if you have a big world.

# Outro.

I hope this instruction will be useful to you;) 
if you have any questions, write them to https://github.com/Max-RM/Change-worlds./issues
