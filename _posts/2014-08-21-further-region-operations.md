---
layout: post
title: "Further Region Operations"
description:
comments: false 
tags: [03 EDITING SESSIONS]
image:
  feature: Ardour3_Empty_Session_Transparent.png
  credit:  
  creditlink:  
---

In this section you will learn a few more things you can do with Regions.

Right-clicking a selected Region reveals a context menu. The first item
in the menu (labeled with the Region's name) contains a large sub-menu.
All of these operations are also available from Ardour's main *Region*
menu.

This section describes a few of the most commonly used operations
accessible from these menus.

![region menu 1]({{ site.url }}/images/Ardour3_Region_Menu_1.png)

-   **Play**: play back from the beginning to the end of
    that Region (shortcut "*H*").
-   **Loop**: set the loop range to fit that region's duration, and
    start looping it right away.
-   **Rename**: change a region's name.
-   **Properties**: lots of information on the region, plus ability to
    change its gain.
-   **Position**: among other options, in this sub-menu you will find
    The **Lock** toggle box: it locks the Region so that it cannot be
    Moved or Trimmed. It can still be Split, however, and the resulting
    Regions will be unlocked.
-   **Edit**: in this sub-menu you find useful tools such as
    **Mute**(shortcut "*Control*" + "*M*"), **Pitch Shift** (shortcut
    "*Alt*" + "*T*") and **Reverse** (shortcut "*Alt*" + "*R*"). Mute
    renders the region silent. Pitch Shift alters the pitch of a region
    without changing its duration. Reverse makes the region play
    backwards.
-   **Gain**: useful options such as **Normalize** (shortcut
    "*N*"), **Boost Gain**, and **Cut Gain**.
-   **Duplicate**: includes Duplicate, Multi-Duplicate, and Fill Track.
    These were explained in detail in the chapter [Working with
    Regions](../working-with-regions). 
-   **Spectral Analysis**: window displaying the overall frequency
    content of the Region.

Feel free to explore by yourself other sub-menus not mentioned above.
Many of them are mirrors of the options you find under Ardour's
*Region* menu. Below we go into a bit more details on some of the most
useful functions. 

## Pitch Shifting

The **Pitch Shift** function (shortcut "*Alt*" + "*T*" with a selected region)
alters the pitch of a region without changing its duration. The function
applies a pitch-shifting algorithm to create a new audio clip based on
the source clip.

The Pitch Shift window the user to specify the amount and direction of
transposition desired. The window includes a **Preserve Formants**
button. When pitch shifting by large amounts, the Preserve Formants
option can give results that sound slightly more natural, particularly
when used on vocal material.

![pitch shift]({{ site.url }}/images/Ardour3_Pitch_Shift_Window.png) 

## Normalize

The **Normalize** function (shortcut "*N*" with a selected region)
non-destructively boosts the level of the selected Region so that the
**Peaks** are at 0 dB or less. When Normalizing to 0.0, the region will
be as loud as possible while avoiding **Clipping**. Sometimes you may
find useful to normalize a region to a value less than 0, such as -1.0,
-3.0, or -6.0 decibels, so it doesn't become too loud. 

![normalize]({{ site.url }}/images/Ardour3_Normalize_Window.png) 

## Reverse

The **Reverse** function (shortcut "*Alt*" + "*R*") reverses the
selected region of audio, in effect causing it to play backwards.
Reversing a region creates a new audio file 'behind the scenes'.

## Operations on two or more selected Ranges

If more than one range is selected, the operation will apply to all of
them (for example, Normalize, Reverse, etc.)

### Combine

Some operations from the context menu will only become available when
two or more regions are selected. For example, take a look at the
"Combine" function, under the sub-menu "Edit". First we select two
adjacent regions:

![combine]({{ site.url }}/images/Ardour3_Region_Combine.png)

Then we choose "Combine" from the right-click context menu, or from
Ardour's main menu *Region > Edit > Combine*: 

![combine 2]({{ site.url }}/images/Ardour3_Region_Combine_2.png)

As a result, the selected regions are combined into one. This is
particulary useful when you have found an exact sequence of regions that
works just as you want, and then you would like to copy and/or move the
whole sequence as group.

Notice that the resulting combined region has the word "compound"
attached to its name. 

![combine 3]({{ site.url }}/images/Ardour3_Region_Combine_3.png) 

## Continuing

In the following chapter, we will learn a bit more about the powerful
tools Ardour has available by changing **Edit Modes**.

Next: [CHANGING EDIT MODES](../changing-edit-modes)
