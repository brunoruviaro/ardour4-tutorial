---
layout: post
title: "Creating a Track or a Bus"
description:
comments: false 
tags: [02 GETTING STARTED]
image:
  feature: Ardour3_Empty_Session_Transparent.png
  credit:  
  creditlink:  
---

What is an Audio Track?
--------------------------

An **Audio** **Track** is a place where you can drag a **Region**
from your **Region List** and where you can record sounds coming from an
outside source.

A Region represents an audio clip, i.e., one of your
sound files or just a portion of a sound file. In the image below, the
horizontal strip areas marked "*Audio 1*" and "*Audio 2*" are Tracks.
The rectangle containing audio information (named "*some-sound*") inside
track *Audio 1* is called a Region. 

![Tracks]({{ site.url }}/images/Ardour4_Tracks.png) 

What is a Bus? 
----------------

A **Bus** is similar to a track except that it does not contain its own
regions. You cannot record directly into a bus or drag regions into it.
In the image above, the area marked "*master*" is a Bus. Usually every
session has a **Master Bus**. All the audio to be **Exported**  from
your Session will be sent to the Master Bus.

How are Tracks and Busses Used? 
---------------------------------

Audio-processing **Plugins** and **Automation** can be applied to both
Tracks and Busses.

Audio tracks can be routed to Busses. In fact, many Tracks can be
simultaneously routed to one Bus. Busses are traditionally used as a
convenient way to apply any kind of signal processing to many Tracks at
once. For instance, you might find it useful to route all Tracks that
contain drum sounds to a single Bus that you would call '*drum bus*'.
Then, if you decide that all your drum Tracks are too loud, you can
quickly adjust the level of the '*drum bus*' rather than adjusting each
separate Track that feeds into it.

Another use of a Bus would be to have a common **Reverberation** Plugin,
so that any audio Track which requires the Reverb effect could be routed
to a single Bus. 

Adding Tracks and Busses
------------------------

Right-Click in the empty area beneath any existing Tracks and Busses.
Alternatively, click on the menu *Track > Add Track/Bus* (shortcut
"*Ctrl*" + "*Shift*" + "*N*"). The following window will appear:

![Add Track]({{ site.url }}/images/Ardour4_Add_Track_or_Bus.png) 

**Add** lets you specify how many Tracks (or Busses) you would to like
to create.

Choose **Audio Tracks** or **Busses** to specify whether you want to
create Tracks or Busses. You can also choose to create a **MIDI Track**
or an **Audio+MIDI Track**. Ardour offers three track types depending on
the type of data they contain, and differentiates between three track
modes, depending on their recording behaviour. This tutorial will only
cover Audio Tracks and Busses (see the [Ardour
Manual](http://manual.ardour.org/working-with-tracks/track-types/) for
details on all track types) 

You can optionally give a **Name** to the Track or Bus being created.
The **Configuration** drop-down menu allows you to specify how many
channels of audio you'd like the new Track or Bus to handle. For
example, if you will be recording your voice on this track using a
single microphone, choose **Mono**. If you plan to import a clip from an
existing song and place it on this Track, choose **Stereo**. The choice
made here will also affect which Plugins you can use on the track (Mono
tracks cannot use Stereo Plugins and vice versa).

The menu **Track Mode** gives you a choice between **Normal**,
**Non-Layered**, and **Tape**. Normal Mode creates a new Region for each
Recording **Take**, and is suggested for beginners. For information on
the other modes, check the [Ardour
Manual](http://manual.ardour.org/working-with-tracks/track-types/).
Additional information on the **Instrument** and **Group** options can
be found on [this other page of the
Manual](http://manual.ardour.org/working-with-tracks/adding-tracks-and-busses/).

Finally, click the **Add** button to create the Tracks or Busses you
have just configured. You will see them appear as new rows in the **Main
Canvas**.

Continuing
----------

Once you've added one or more Tracks, you will want to put some audio
material into them to work with. Continue on to the **Importing Audio**
and **Recording Audio** chapters to learn how to do this. 

Next: [IMPORTING AUDIO](../importing-audio)
