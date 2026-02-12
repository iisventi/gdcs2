---
title: Static Objects
weight: 111
draft: true
---
## Guide info
Short: 7-9 minutes

## TLDR - What this guide covers
- Static objects are objects in the GD editor that have hitboxes the play can interact with; they include: blocks, slopes, spikes, and saws.
- Blocks can be stood on the top, but if the player hits them on the sides or the bottom, they will be killed.
- Slopes are similar to blocks, but they have an slanted side on the top and an angular hitbox.
- Spikes and saws kill the player on contact, but they differ in hitboxes.
- Static objects have many variations which can have different hitboxes.
- The properties of these objects can be modified by clicking their :EditGroup: Edit Group, and checking the Extra button to the right.

** **

# 1: Blocks

**Blocks** are contained in the first and second tab of the editor. They are solid, meaning they __can be stood on without death__. However, if a player comes into contact on the sides or bottom, they will be killed. Their hitboxes are always a rectangle, being identical to how they appear visually.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1G4IXGbzo7vRcRTJfrGZOaM35VjU_MBWJ/preview?usp=drivesdk></iframe></div>

Blocks, due to being a solid, cannot be rotated. The rotate trigger simply moves the block instead of also putting it at an angle.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1pR_VpQziA3ejZpAsYraNzBoDQRBi4X41/preview?usp=drivesdk></iframe></div>

There are four types of blocks:
- The Square:

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1G2Q_Z8mEiuhLtRzz7K3rErbKACW0yb3A/preview?usp=drivesdk></iframe></div>

- The Slab

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1uTRI6Gts4XD1wN2MQrl9OhIExJIcMVUF/preview?usp=drivesdk></iframe></div>

- The Small Square (½ of the Square’s size)

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/18nwsQZlttUGT5bMTQLbK0ur2XTB4H3ma/preview?usp=drivesdk></iframe></div>

- The Small Slab (½ of the Slab’s size)

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1KSZFzbDUP7ILZOGD6wLU2TmMD0bKn5dU/preview?usp=drivesdk></iframe></div>

## Outline Blocks
**Outline Blocks** __act identically to blocks, but work better as a blank canvas for decoration__, giving the player a clearer idea of what is and isn’t decorational.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1H3gKKFafLstmH6L02riW9taO6OErHCWB/preview?usp=drivesdk></iframe></div>

They have many more variations than just a simple box, having a single line (which has a different hitbox), an L shape, the pillar blocks, and a corner piece. There are also three different thicknesses.

## Other Blocks
**Breakable Blocks** get __destroyed when approached from the side or the bottom__. In Platformer mode, hitting it from the bottom bounces the player off of the block as if it has an H block on it, but in Classic mode they go through it.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/10zqkGBANs1QPmRqwsj3tsAEaapxeBrjA/preview?usp=drivesdk></iframe></div>

**Vanishing Blocks** __slowly fade away, reaching a near-zero opacity as they get closer to the center of the screen__. This effect then reverses as it moves away. This is purely visual, and does not have an effect on how the player interacts with it. This opacity can change depending on whether “NoGlow” is ticked in the Edit Group’s Extra menu. For the examples below, NoGlow is disabled.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1w9IbDE6aAnn0fRfA6GSLfY7wdB9CmGuh/preview?usp=drivesdk></iframe></div>

Some blocks also have different, more unconventional hitboxes.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1uWjAOwpSlFOST-chf8-lkqnsrjAe_Czb/preview?usp=drivesdk></iframe></div>

# 2: Slopes

**Slopes** are located in the second and third tab of the editor. They, just like blocks, can be stood on, and will kill you if hit from the bottom or a side. __However, they have a right-angled, triangular hitbox and appearance, with a hypotenuse as its surface.__

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1OARHTUlHRvLczPUyfM7eojzYQSqCVbIB/preview?usp=drivesdk></iframe></div>

Slopes, like blocks and all other solids, cannot be rotated.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1rTsHqQ8wOYsNCzb8FnsWTE4EP-WBmnRA/preview?usp=drivesdk></iframe></div>

There are only two types of slopes:

- The 45° Slope:

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1Ka0KDffi2bsT6GuvKX87Ifubn8IQAGyh/preview?usp=drivesdk></iframe></div>

- The 22.5° Slope:

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1CsVSjR5eVtOaTrv8okL_wYRv4UEe1N_5/preview?usp=drivesdk></iframe></div>

## Outline Slopes
Slopes also have outlines, although they have no thickness variations except on the corner pieces. They are still just as useful for decoration.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1Pb3gF6igYwPxrZiVizW41CIcq9Y97dmE/preview?usp=drivesdk></iframe></div>

Due to the more specific shape of slopes, there are no variations in shape.
## Vanishing Slopes
Vanishing Slopes do the exact same thing as Vanishing Blocks. The only difference is that they are a slope.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1-sJIqRYn3FgZYyExyfi5SapWujLLwdcw/preview?usp=drivesdk></iframe></div>

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1x55XnecNDXjPp6HSMy_frBsxX5qoAqTV/preview?usp=drivesdk></iframe></div>

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/12p8IoQuUYwne3OxWMQ7B8zwXkA50u1qV/preview?usp=drivesdk></iframe></div>

# 3: Spikes

**Spikes** are located in the fourth tab of the editor. They are hazards, __killing the player upon contact__. Their hitbox is rectangular, being elevated around ~¼ of the spike’s height.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1dRr20ezZcc9PiaycVrsoROVQShLtQNff/preview?usp=drivesdk></iframe></div>

Unlike blocks and slopes, spikes can be rotated, as it is not a solid; however, the slope spikes are an exception to this since they have a solid slope hitbox on them.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1GQklMwnxta7zwMYDBolmG3OMhYUxcmSW/preview?usp=drivesdk></iframe></div>

There are four types of spikes:

- The Spike:

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1WNedAQSQxXT69916ADgDxZsjOVo22NRk/preview?usp=drivesdk></iframe></div>

- The Flat Spike:

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1YHmM9vP1xKVck7lUXf7xqloI2cmA3v6l/preview?usp=drivesdk></iframe></div>

- The Small Spike (~⅔ of the Spike):

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1WCEIPJKGO6l7cs8MLt5ED69-iZ-Iu14q/preview?usp=drivesdk></iframe></div>

- The Mini Spike (~½ of the Spike):

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1r5ETG8yDAp-GWWXaF32M8mi16p5mTQiB/preview?usp=drivesdk></iframe></div>

Unlike solids, spikes do not have outline objects. They can be recreated using the color spikes, but they are not a default object in the editor.
## Ground Spikes
**Ground Spikes** are __spikes made to be put on the ground__. They are often used to catch the player, preventing skips while looking more natural in groups. They are more useful for decoration, but are still good to know about. Their hitboxes vary, and don’t follow the same conventions that traditional spikes do.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1G-mNV9530BGGzddOFwEMrNlRW7ZJgHl-/preview?usp=drivesdk></iframe></div>

## Other Spikes
Vanishing Spikes act the same way as any other Vanishing object.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1KSaYn20I6JbNQU9jb0aueA0aZWnACnsy/preview?usp=drivesdk></iframe></div>

Some of the spikes have slightly unconventional hitboxes.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1WWrg3ygHMKnU9G3Vny7wAkHtSpAVI5lt/preview?usp=drivesdk></iframe></div>

# 4: Saws

**Saws** are located in the twelfth tab of the editor. __Just like spikes, saws are hazards and kill the player upon contact. Instead of the spike’s rectangular hitbox, the saws’ hitboxes have a circular shape__, usually extending (approximately) until the teeth.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1RYtcqJ_0fEQrRDG7vVIyAiPpkD3pIywL/preview?usp=drivesdk></iframe></div>

Saws can also be rotated, - just like spikes - although it isn’t as noticeable since they spin anyway; however, it allows for custom rotations if you only make the saw spin.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1CYhJOv5Y2IOellQmptCprT_ouQUMw2rO/preview?usp=drivesdk></iframe></div>

There are three types of saws:

- The Big Saw:

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/16b--3-kAZjBDwe3_SEDQ9vmvUB9QfLa9/preview?usp=drivesdk></iframe></div>

- The Medium Saw:

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1QqVfq458qOPQMfMiKZmUysdtbhJM1uFR/preview?usp=drivesdk></iframe></div>

- The Small Saw:

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1Yug_iyuFk6IBDMOvyhO5rKnBX4Et-PYI/preview?usp=drivesdk></iframe></div>

## Variations
Saws have a lot of variations - 8 of them, to be exact. These all share different hitboxes between each other. These differences need to be kept in mind when making gameplay (especially with the last one), since choosing the right saw can make a positive or negative impact on the gameplay.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1yQa73pc1j-14LKiw5W66f0RwtOqa5iOb/preview?usp=drivesdk></iframe></div>

Vanishing Saws also exist, having a blue button instead of a grey one. They do exactly what all other vanishing objects do - slowly fade away as they come nearer to the center of the screen.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1etQnWDATTFPtnBAL0WC8t9OtQP0Y7v6m/preview?usp=drivesdk></iframe></div>

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1D4XKMDwK6T9wvo6DWRvlHnpFwrglW5_q/preview?usp=drivesdk></iframe></div>

These objects are a hybrid between saws and spikes. Despite being in the saws tab, looking like saws, and having the same circular hitboxes as them, they act more like spikes, due to having no automatic rotation.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1qgqSXPfgYIu0k-DF3SL2O8KuKiadHdQE/preview?usp=drivesdk></iframe></div>

These saws have incredibly unconventional hitboxes, so use them wisely.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1RYZdPrPUSDVJSv8u-OV9Zu_Fp9aByveg/preview?usp=drivesdk></iframe></div>

## Rotation
You can select a saw and click on :EditSpecial: Edit Special to give them a custom rotation. There are three options: the default rotation, which randomly fluctuates between a set of rotation speeds; the custom rotation which lets you input a specific rotation speed measured in degrees per second; and the disable rotation, which ceases all rotation on the block.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1qYYVLJlhcQVqDTTYzUatCLoAg94QIIxp/preview?usp=drivesdk></iframe></div>

# 5: Object Options

In addition to these objects, you can modify their properties to your liking. To do this, select an object, click on :EditGroup: Edit Group, and click on the Extra button to the right.

- **IceBlock** __gives blocks in Platformer an ice-like property__, making acceleration much slower when the player attempts to do so on the block’s surface.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1TSlMDTVPWB45myZm7rJuWZSeAWMU8_RE/preview?usp=drivesdk></iframe></div>

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1FD4oGA58867i9EeD0kT-9laKu9s41-nL/preview?usp=drivesdk></iframe></div>

- **NoTouch** __removes the object’s hitbox completely__, making it unable to be interacted with by the player.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1yhkBYgZnFhYFg8LuXc-Gc3KesqWFcMzK/preview?usp=drivesdk></iframe></div>

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1r47OkEwtQksfthVICz7W9QMQd7xuQ6N_/preview?usp=drivesdk></iframe></div>

- **GripSlope** __allows the player to stand still on a 45° slope__, instead of sliding down it in Platformer.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1gob0D7oJ2paa3UpK-rDPjKTWVq9zZ5kx/preview?usp=drivesdk></iframe></div>

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/10vKWCx6EyLmc5kF_2ksuMx05Z-AQVACB/preview?usp=drivesdk></iframe></div>

- **Passable** __allows the player to pass through a block from the bottom, but still allows the players to stand on the block__. You can move onto the top from below too.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1dkR6fbq-2UD0aoEefUUPkQ2SNyqgz2qr/preview?usp=drivesdk></iframe></div>

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1mNQsmC9UKXH8ZgB8EBzMULNMVji9OEs7/preview?usp=drivesdk></iframe></div>

- **Hide** __completely removes the visual appearance of an object__. You can press F6 in the editor to show these hidden objects if needed.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1XK-4cyA_wFJ86juqLeyKEP0KQYsEV5FI/preview?usp=drivesdk></iframe></div>

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1JAA7RVTZbiV0RWapMdYfXi8LGnChvtJc/preview?usp=drivesdk></iframe></div>

- **NonStickX/NonStickY** __stops the player from sticking to moving blocks in Platformer__.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1nIugS0VRHjjPBgmEcpYg03gItaBhYmHn/preview?usp=drivesdk></iframe></div>

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1j0yt72iktMMp00Q38ZG9aFlLamq3Jazb/preview?usp=drivesdk></iframe></div>

- **DontBoostX/DontBoostY** __stops the player from being boosted by moving blocks__.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1LiJSLoQaeBfmp--O_VtVCXKKAsemGwNR/preview?usp=drivesdk></iframe></div>

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1kvB3bHaIm7KyWwIlSPgz7IhYetGfk0dL/preview?usp=drivesdk></iframe></div>

- **ExtraSticky** __keeps the player stuck onto blocks moving downwards at higher speeds__. This has a limit, however - moving too fast can still cause the player to stop sticking to the block.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1ixiYaIj0SvYVpJtzr6QFW3ff63O0plfc/preview?usp=drivesdk></iframe></div>

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1fEcA5vGTo078PCWeD6Je1vE5PUFZVZVU/preview?usp=drivesdk></iframe></div>

- **ScaleStick** __allows the player to move along the X axis of a block relative to its center when it is scaled__.

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1NHYm2FqTxGyGykqTHyjx2E3Ulrk3tjir/preview?usp=drivesdk></iframe></div>

<div style="width: fit-content; height: fit-content"><iframe src=https://drive.google.com/file/d/1vmjbirbPpilWCntLvwRmiZG03mQOPYxm/preview?usp=drivesdk></iframe></div>

- **Extended Collision** __fixes the hitboxes of objects with a scale above 6__.

<div><iframe src=https://drive.google.com/file/d/1PV8LK4QG3ToTXgWZVFIoXmvRopaIkMXH/preview?usp=drivesdk></iframe></div>

<div><iframe src=https://drive.google.com/file/d/1VC5dvc3mqq7lXdcLQYAZC6u7CD5rG0k-/preview?usp=drivesdk></iframe></div>





## Credits
Created by @DangerChampion and @Xplode
