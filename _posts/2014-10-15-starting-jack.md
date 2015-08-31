---
layout: post
title: "Starting JACK"
description:
comments: false 
tags: [02 GETTING STARTED]
image:
  feature: Ardour3_Empty_Session_Transparent.png
  credit:  
  creditlink:  
---

Ardour 4.X no longer requires that you have JACK (the JACK Audio Connection Kit) installed on your system. But you may want to have JACK available so that Ardour can share audio and MIDI with other Linux audio applications. If you are wondering just what on earth JACK is then take a look here: http://ardour.org/jack

In a nutshell, JACK is an audio system which manages connections between Ardour and the soundcard of your computer, and between Ardour and other JACK-enabled audio programs on your computer. Ardour used to require JACK in order to run, but since version 4.0 this is optional.

More info on JACK: [http://jackaudio.org/](http://jackaudio.org/) and [http://jackosx.com/](http://jackosx.com/).

On Ubuntu, you may use either Qjackctl or Cadence to start and stop JACK and control its settings.
If you have a properly configured [KXStudio](http://kxstudio.sourceforge.net/) installation, JACK may be already running in the background. If not, you may have to manually start it.

On a Mac, you will need to use [JackPilot](http://www.jackosx.com/). This page may be of help: [http://en.flossmanuals.net/ardour/ch005_installing-jackosx/](http://en.flossmanuals.net/ardour/ch005_installing-jackosx/) (**Warning**: details on that page may be outdated. Eventually we hope to include an updated page like that in this tutorial).

## Using Cadence (Linux)

Launch Cadence. If JACK is already running, you will see a window like this:

![cadence]({{ site.url }}/images/Ardour3_JACK_Cadence.png)

More info on Cadence: [http://kxstudio.sourceforge.net/Documentation:Manual:cadence_introduction](http://kxstudio.sourceforge.net/Documentation:Manual:cadence_introduction)

## Using Qjackctl (Linux)

If using Qjackctl instead, this is how it should look like:

![qjackctl]({{ site.url }}/images/Ardour3_JACK_qjackctl.png)

If not yet running, use the "Setup" button to configure JACK, and hit "Start" to start JACK.

## Using JackPilot (OS X)

Please check this page: [http://en.flossmanuals.net/ardour/ch013_starting-jackosx/](http://en.flossmanuals.net/ardour/ch013_starting-jackosx/) (**Warning:** this page may be outdated. It's provided here just as a starting point. Eventually we hope to include an updated version of it in this tutorial).

## JACK Settings

More info on Jack configuration: [http://kxstudio.sourceforge.net/Documentation:Manual:jack_configuration](http://kxstudio.sourceforge.net/Documentation:Manual:jack_configuration) (explanation shown using Cadence, but same basic information applies to Setup window in Qjackctl).

## Continuing

Next: [STARTING ARDOUR](../starting-ardour-on-ubuntu)
