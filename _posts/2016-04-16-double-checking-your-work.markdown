---
layout:     post
title:      "Double Checking Your Work is Not Enough, Seriously"
date:       2016-04-16 12:00:00 -0400
categories: electronics engineering
comments:   true
---

After going through 3 different phases of my [IAS PCB][ias-pcb], I learned its never a bad thing to double check things...in my case a simple check of temperature limits in  the datasheets for the components I used could have saved me another full revision of my previous layout...I basically couldn't put up with surface mount components so I limited the amount I needed and revised it:

- v05 PCB here. -
Never again, tiny SMD components. Never again...

Anyways, I found the problem with my last revision was not the design of my board, but simply my soldering strategy...turns out one been burning out my voltage regulators...can't blame my botchy soldering skills on cheap Chinese parts. What I thought was accidentally shorting of smd components and wires was actually just me being silly and burning out the regulator from too high temperatures. Keeping my iron at 300 C is not a good idea apparently...at least for the components I'm using. I never thought soldering for such a small amount of time would burn out components. Busting out my multimeter proved it burned. Anyways, the new revision of my board is better ish. Don't know if the extra 40 bucks I had to shell out to [OSHPark][oshpark] could make another 3 batches is worth it though.

- v06 PCB here. -

So back to the point. This all applies to the real world too. I've been working in the industry for less than a year, so this may be obvious to _most_, but its still good to explictly say it. I catch small mistakes _all_ the time. So make sure to not only triple or quadruple check your work, but to get a fresh pair of eyes to see your work, you never know if they may catch mistakes that you overlooked. Now to finally solder this baby completely and move on to re-coding the mess of the state machines I had done for the breadboard prototype version...fun...


[ias-pcb]: http://sergiomorales.me/ias.html
[oshpark]: https://oshpark.com/