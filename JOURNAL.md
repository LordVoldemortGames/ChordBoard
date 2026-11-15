---
title: "ChordBoard"
github: "https://github.com/LordVoldemortGames/ChordBoard"
description: "I'm building a music tool. It's a little capacitive one-octave keyboard with pads to control what chord is played over the root note. What you play will be put out via USB-MIDI to your pc. On top of that there will be some settings, which you can edit over a rotary encoder, two buttons and a small display."
created_at: "2026-11-15"
total_time: "7h"
---

# November 15, 2026: Design of the ChordBoard
<!-- fabricate:entry 3077 -->

Well... originally I only wanted to try out KiCad today and research a bit about capicitive touch pads, inspired by the midi keyboard from the example projects. In the end I designed the whole board today.
I started with deciding which microcontroller to use since it has to be one which can use capacitive touch pads. The obvious answer would've been to use an ESP32 but then I read about some projects, where someone used the PIO of the RPi Pico for capacitive touch pads and since it is even cheaper and got way more pins I decided to use this one. Then I continued to design a schematic, which actually worked pretty well on the first try. In the end I got a schematic for an idea I had a while ago. A keyboard with only one octave to choose a root note and some more touch pads to choose which chord to play over this root note.
Then I designed the pcb itself, which first brought me some problems because of some bad routing in my schematic, but nothing that couldn't be fixed in under 5 mins. At the end I put down some text on the silkscreen and there it is, a finished design for my ChordBoard.

![](https://fabricate.hackclub-assets.com/24722fb8cd4426410b99be177e46a4f846204c0565494741bbd7506c99bc6704/image-png/Bild_2026-11-15_163507972.png)
![](https://fabricate.hackclub-assets.com/5a5d32616a10c9c3a04cef401bcf3c9c9ceaba640264f706affc0fec962e1426/image-png/Bild_2026-11-15_163544369.png)
![](https://fabricate.hackclub-assets.com/b6699871f7f751916c6daf56ede5c288636df5b5a6bda7361083e7252def3db7/image-png/Bild_2026-11-15_163658554.png)
![](https://fabricate.hackclub-assets.com/2211a1ee4545c273d255deef1fd204d5254ca9cd79e8f91f2acc465a47b337b3/image-png/Bild_2026-11-15_163718512.png)

**Total time spent: 7h**
