---
title: Editing Objects
weight: 102
draft: false
---
## Guide info
Short: 7-9 minutes

## TLDR - What this guide covers
- Z layer and Z order let you place objects on top of or behind each other.
- As of Update 2.2, tilesets override Z order when objects share the same Z layer.
- Groups are used by triggers and can be added in the :EditGroup: menu.
- Two extra tabs exist to further tweak your objects.
- Anim serves as a shortcut to creating keyframes.
- Edit Object lets you change an object’s color.
- You can copy an object’s Z layers and color using Copy Values, then paste them using Paste State and Paste Color.

** **

# 1: :EditGroup: Z Layer & Z Order

**Z Layer** and **Z Order** change __how objects render on top of each other__.

If you wish to change an object’s Z layer, select an object, and go to :EditGroup: Edit Group. At the bottom you’ll see a section called “Z Layer”. Click on any of the buttons to set an object’s Z layer.

T Layers (T1, T2, etc) render above the player’s icon. B Layers render below T Layers and the player’s icons.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1Pb6NB3xVCUcXZ_gZRKGxNwlzQf-axi6U/preview?usp=drivesdk></iframe></div>

Z Order can be found in the Edit Group menu as well, just at the top right. You can either click on the buttons or type a specific number to set an object’s Z Order. This is a more “specialized” version of Z Layer; objects with a higher Z Order number will render in front of the ones with a lower Z Order.

Z Layer takes priority over Z Order, so an object on layer T1 and order -5 will render above an object on layer B1 with order 10. Feel free to try this out yourself!
## Tilesets
However, as of 2.2, there is a __new layering value__ called **tilesets**. These values are different for most objects, but similar objects share the same tileset number. You can check an object’s tileset by checking the value inside the parenthesis next to “Z Layer.” If you select many objects with differing tileset numbers, it will show a - in the parenthesis.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1ThDEWCIk2bmPvnOqptCKacg5eLBrGyth/preview?usp=drivesdk></iframe></div>

Objects with a lower tileset will *ALWAYS* be above objects with a higher tileset, as long as both objects are in the same Z Layer. Tilesets completely override Z Order since Z Order *only affects objects with the same tileset*. If you ordered and layered everything correctly and still see something off, your problem might come from the tileset number, in which case you need to change the Z Layer.

# 2: Groups

Groups are a fundamental system that allows triggers to target certain objects, however more detail will be in the [Groups](<https://discord.com/channels/414295025883545600/1198062001499418704>) guide. For now, we will only cover how to assign groups.

Here’s how to add groups:
1. In the middle of the :EditGroup: menu, there is a counter labeled “Add Group ID.” 
2. You can type in or select an ID, then click Add to add the object to the group. 
3. If you want a brand new group that hasn’t been used before, click Next Free and then click Add.
4. Alternatively, click P to make the object the Parent Group, which will once again be covered in the Groups guide. 
5. To delete a group, click its number in the Group Box. To remove an object from Parent Group, click its number once.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/13JcEGWsaAwKEBx8_bu-ZmtKSzDH-YhDB/preview?usp=drivesdk></iframe></div>

# 3: Extra Tabs

The two extra tabs give you more options to customize your objects. 
## Extra Tab 1
**Extra Tab 1** __lets you select different options to give your objects different properties__. This section will go over the different options.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1ApFT8E7higf7WeAfVDrdMJ9pVH92CXN9/preview?usp=drivesdk></iframe></div>

- **Don’t Fade** and **Don’t Enter**: __Stops the object from having an effect at the edge of the screen.__
- **No Effects**: __Stops pads and portals from having effects as you interact with them__, like the background flashes in size portals.
- **Group Parent**: When rotating or scaling several objects, the objects will transform relative to the group parent; in other words, the group parent __acts as the center point__. This is not to be confused with Parent Group.
- **Area Parent**: __Functions as a group parent, but for area triggers__. Make sure you link a set of objects together before making one object the area parent.
- **Don’t BoostY** and **Don’t BoostX**: __Stops the player from being boosted by moving blocks.__
- **High Detail**: __When enabling “Low Detail Mode” outside the editor and playing the level, objects with High Detail will disappear__, making the level less laggy.
- **NoTouch**: __Removes collisions from objects with a hitbox (e.g [Static Objects](<https://discord.com/channels/414295025883545600/1189377547625041971/1206106317379338381>)), converting them to [Detail Objects](<https://discord.com/channels/414295025883545600/1189378955174752367/1189378955174752367>).__
- **Passable**: __Allows the player to go through the block from the bottom or side__, making for passable platforms. 
- **Hide**: __Makes the object completely invisible__. Toggling off Hide Invisible in the editor pause menu allows you to see the hidden objects.
- **NonStickX and NonStickY**: When moving objects in platformer mode, the __player will not stick to the object if they’re on top of it.__
- **ExtraStickY**: When moving objects downward fast with the player on it, __this keeps the player on the object rather than having the player fall as if walking off a platform__.
- **Extended Collision**: __Makes the hitboxes of objects match correctly when scaled up by a lot__.
- **IceBlock**: __Makes objects extremely slippery__, like an ice block. Useful in Platformer mode.

- **GripSlope**: __Stops the player from sliding off a slope__. Useful in Platformer mode.
- **NoGlow**: [Static Objects](<https://discord.com/channels/414295025883545600/1189377547625041971/1206102299928428626>) have an inherent glow on their outlines only visible in normal mode; __this option removes the glow__.
- **NoParticle**: __Removes particles from objects like portals and pads__.
- **ScaleStick**: When using a scale trigger on an object with the player on it, the player will only move up. However, __with this option, the player will move to the side as well relative to the center of the scaling__.
- **NoAudioScale**: __Disables the scaling/pulsing on objects that pulse relative to the song__, like the big pulsing circles.

In addition, some objects can have more options, which include the following:
- **Reverse**: __Reverses the gameplay direction as soon as you hit an orb or a pad__. *Orbs and Pads Only*.
- **Single P Touch**: If one player touches an arrow trigger :ArrowTrigger: in Dual Mode, the __trigger will only activate for the player that touches it__. *However, this feature is currently bugged as of Update 2.205.*
- **Center Effect**: __Touch Triggered triggers will only activate once the player touches the center of the trigger__.
- **Smooth Ease**: __Moves the camera smoothly rather than instantly when using any kind of teleport.__

## Extra Tab 2
This tab is somewhat self-explanatory. There are various counters, and these counters allow you to change the IDs shown in the [Using IDs](<https://discord.com/channels/414295025883545600/1189381677978484877/1189381677978484877>) guide. For more information on each of the counters, check that guide.

Keep in mind that not all objects are able to have certain IDs, meaning that some objects will not have some counters that other objects do have.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1iRSBsrj-PS2xdcgpjb4eVgFEXSrnLZsV/preview?usp=drivesdk></iframe></div>

## Anim
The **Anim** button right under the Extra2 button serves as a __shortcut to creating keyframes__. 

If you give some objects a group, and have only one object as the “parent group”, you can click the anim button and it will spawn a keyframe object (the diamond shaped object) on top of the parent group. You can then use the keyframe object as normal.

Keep in mind that **this ONLY WORKS if you have a parent group**. Check out the [Keyframes guide](<https://discord.com/channels/414295025883545600/1194069847982751775/1194069847982751775>) for more information.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1_dwwemy6bVCXSeEoA8lJQyJ85bewaaFQ/preview?usp=drivesdk></iframe></div>

# 4: :EditObject: Edit Object

This is where __you can set object colors. You can also set what text objects say in this menu.__

Objects will either have a “Base” color, a “Detail” color, or both. This doesn’t mean much at this stage; just know that some objects can have two color channels and some cannot.

To change an object's color, choose its "Base" or "Detail" tab, then click on one of the buttons. Each numbered button, along with the "P-Col 1", "P-Col 2", "Light BG", and "Default" buttons, are color channels. You can change their color by clicking on the color square in the bottom right.

You can use the "Next Free" button to select the next unused color channel, the "HSV" button to modify an object's colors independent of its color channel, and the :RGB: button to adjust a color channel in real-time. Clicking the :RGB:  button a second time adjusts an object's HSV as well in real-time.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1GpPxgfWcftJS2kZaeraL1f0fUcsfTGES/preview?usp=drivesdk></iframe></div>

# 5: :CopyValues: Copying & Pasting Values

:CopyValues: To copy an object’s properties, such as Z Layer and color, press the Copy Values button.
:PasteState: To paste Z layer to another object, press the Paste State button. This button will also paste groups from one object to another unless "Disable Paste State Groups" is enabled in editor settings.
:PasteColor: You can use Paste Color to paste an object’s colors to another object.

<div><iframe src=https://drive.google.com/file/d/1Yk_o8yAb6AJwg_CYCvgik80R5zwW9iev/preview?usp=drivesdk></iframe></div>





## Credits
Created by @koma5
