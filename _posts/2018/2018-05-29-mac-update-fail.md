---
layout: post
title:  "Macbook Update Fail"
date:   2018-05-29 16:16:01 -0600
description: A brief history of trying to update a Macbook Pro.
tags: apple
---

Family members do not hesitate to ask me for help with their IT problems.  It can be anything.  I've helped my in-laws upgrade their computer.  I've also video chatted with others trying to help them find a hidden HDMI port on a television.  I don't really mind helping.  I like to help people.  Often times I see it as a challenge - me versus the machine.

What I can't stand is when the computer's win.

Recently, my lovely wife tried to update her 2012 Macbook Pro to what I suspect was High Sierra.  I never actually found out.  The update went for about 5 minutes, before displaying the message "Update Failed: Press Restart to Try Again".  Of course, restarting only got you back to the same page 5 minutes later.

Closing the application got you to an error log, and combing through it found this message:  updateSystemInputSources false but old data invalid

Do you know what that means?  Because I have no idea.  So I decided to consult the smartest tech support person I know - Google - and what I let down.  There were a few people with the error.  Nothing really concrete to go off of.  It did seem clear the update was a wash, and it was best to try and restore a backup, which we didn't have.

I tried what I could.  It allowed me to get to Disk Utility, so I ran repairs on hard drive and found no issues.  I tried to restart using that as the main disk, thinking it would bypass whatever update procedure it was going to, and got nothing but the same error message.

At this point I'm getting desperate.  I tried to start in 'Diagnostic Mode' by holding the 'D' key at startup, which got me to a real retro looking hardware diagnostic page.  No problems with the hardware.

Note: I was trying to get to the Internet Recovery OS - Command + Option + R

Finally, after an hour or two of combing helpless through blog and forum posts - I had a breakthrough and found Recovery Mode.  Holding cmd + R at startup.

It gave me 4 options - Restore from Backup, Reinstall OSX, Get Help Online, and Disk Utility.

Reinstalling OSX was the door of choice.  From what I could find it wouldn't completely remove the hard drive, but we didn't care at this point.  I select the option, it tells me it needs to verify something with the hardware, I hit okay, and then nothing.  Try again, select the same option, and nothing.

I wasn't connected to the internet.  

Okay, second try - select the option, verification happening, and... error: UNTRUSTED_CERT_TITLE

And.. back to Google!  A few dead ends, and eventually I found what I needed - most likely my time was off.  I managed to open up the Terminal using the menu at hte top - ran the date command, and sure enough, "Jan 1 2018" was the date.  

It SHOULD have been as simple as running the command 'date MMDDHHMMYY'.  Of course, it wasn't.  I kept getting an invalid date formate error.

I'm not to happy to admit it was my fault.   What can I say?  I was tired, it was a long day, and this machine would not give me anything.  The format is MM - Month, DD - Day, HH - Hour, MM - Minute, and YY - Year.  Why the year comes after everything I don't know.  This is why you read instructions.

Okay, got the internet connected, got the date set, got the right option... FINALLY!!!! Things were verified, and the reinstall process started.  Not the upgraded OS, but the original OS before starting this mess.  

A long time (about 2 hours) later, we got logged into the computer.

Needless to say I was not impressed with this update, the Apple UX, or Mac UI to try and troubleshoot it.  Multiple times I through up my hands and set get a Genius on it.  I don't know why it was so difficult to figure out what was wrong with the update.  I still have no idea what the original error was.  I had no idea reinstalling the OS was an option.  It seems like after the upgrade process started, Apple had no way to back out of it.  

Either way, I fought back the machines again!  Hopefully we won't be upgrading that laptop anytime soon.  
