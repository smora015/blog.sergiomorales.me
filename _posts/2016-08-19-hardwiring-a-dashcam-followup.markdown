---
layout:   post
title:    "Hardwiring a Dashcam in a Vehicle - Follow Up"
date:     2016-08-19 21:07:00 -0400
tags:     
          - projects
          - electronics
          
comments: true
summary:  Follow up on hardwiring my dashcam.
---

A couple months ago I tried hardwiring my dashcam. I mentioned I was using a voltage regulator to step down from 12 V to 5 V. Worked like the charm for a couple days, until I realized the dashcam was intermittently shutting on and off? I took out the circuit and tested it out, and found out it was overheating to the point where the regulator shuts itself off. Silly me...I didn't even bother calculating the amount of heat generated from stepping down by 7 V on a device that's easily drawing up to 1 A of current!

Ohms law tells me that the power being dissipated would be:

Power = I x [ Vin - Vout ]

Power = 1 A x [ 12 - 5 ] V

Power = 7 Watts that needs to be dissipated into heat for the regulator to stay at 5 V!

Even with a heatsink attached, I still found the circuit to be overheating...


For some reason, I forgot that I could have salvaged the circuit inside the charging cable that came with the original camera packaging...I basically tore apart the casing (cigarette lighter connector) and soldered the input voltage, output voltage, and the ground wires. That did the trick!

Lesson learned- linear voltage regulators are not good at dissipating lots of power if you don't have a nicely-sized heatsink...pictures to be added soon!