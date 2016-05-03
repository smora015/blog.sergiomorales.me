---
layout:   post
title:    "Visual Studio 2015 Installer is Terrible"
date:     2016-04-23 12:00:00 -0400
tags: 
          - programs
          - tools
comments: true
summary:  My struggle with Visual Studio on Windows 10.
---

So, I finally decided to try out __Unity 3D__. I finally went out and bought a book for myself, because I honestly don't like to sit through crappy YouTube videos or stare at a screen to read for hours. I ended up getting __Joe Hocking__'s book, [Unity in Action: Multiplatform Game Development in C# with Unity 5][unity-book], and wow, I'm amazed out how quick it is to develop something from scratch. Before I start talking about my progress in the world of crossplatform game development, I'd just like to rant about the week long struggle I went through just install the damn thing for C# scripting.

<center>
   <img src="http://blog.sergiomorales.me/images/vs-error.PNG">
</center> <br>

For anyone wondering what this even means, I'll save you the trouble of having to run around only to have Microsoft act like you're an idiot and think you just downloaded a corrupted installer and having to compare checksums. This [Stack Overflow][stack-overflow] post will save you the trouble.

First off, if you get the steam explorer error, this is from the depencies it needs, which leads to NuGet package installer failing due to your system having an outdated copy of some system library. Save the crap, just install an older version...at the time of this post, the VS RTS version should do the trick. There should be a link to it in the stack overflow post above. Just for reference, you can inspect all of the files in case your problem is unrelated:

<center>
   <img src="http://blog.sergiomorales.me/images/vs-error-logs.PNG">
</center> <br>

This is the perpetrator. I found the error by trying to workaround the issue and installing a standalone version of the NuGet Package manager, but to no avail:

<center>
   <img src="http://blog.sergiomorales.me/images/vs-error-nuget.PNG">
</center> <br>

Anywho, just do what the post says. Sometimes its better to start everything from scratch than to spend hours like me trying to figure it out. But that's just me. I just hate error logs that don't give you a proper indication of what exactly is freaking failing. Good job VS team.

[unity-book]: http://www.amazon.com/Unity-Action-Multiplatform-Game-Development/dp/161729232X?ie=UTF8&psc=1&redirect=true&ref_=oh_aui_detailpage_o06_s00

[stack-overflow]: http://stackoverflow.com/questions/34889317/error-installing-visual-studio-2015-enterprise-update-1-with-team-explorer