# Change-worlds.
Switch worlds from editor mode to Minecraft preview and and vice versa without export-import.

# Intro.
According to Microsoft's instructions  https://learn.microsoft.com/en-us/minecraft/creator/documents/editoroverview#editor-file-operations---create-import-export, to switch the world from editor mode to Minecraft preview and vice versa, you must follow this ##### instruction. But I will show you a more correct way, which I came up with on 03/09/2023, the day after the release of Minecraft preview 1.19.80.02

But why did I call this instruction from Microsoft - #######? it's simple, because imagine that you have created a 5 GB world in Minecraft preview or editor mode and you need to send it to Minecraft preview or editor mode. you will first have to export this world as an archive using game functions, then import it using game functions, and this process, given the size of your world, will take quite a bit of time. It is an absolutely stupid decision on the part of Mojang not to provide for this. in fact, only one NBT tag in the level.dat - isEditorWorld file is responsible for the fact that the world will be displayed in the list of worlds editor mode or Minecraft preview: 1 its presence or absence will affect whether the world will be in the list of some of the games or not.
and it will only take you a few seconds to edit this NBT tag, which is much more reasonable, so use my instruction, not nonsense from Microsoft!

# 0

