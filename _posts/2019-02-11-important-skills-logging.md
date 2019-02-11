---
title: "Important skills for software development - Logging"
tags:
  - skills
  - logging
---
Log things in a meaningful way. 


Too much logging and you won't be able to find what you need on a moment of crisis. Too little and you won't have the info you need. Both extremes are bad.


To find the right balance I like to think about what I need to be able to reproduce the current system state. Maybe the properties of the objects that I am currently dealing with, sometimes the inputs that I get from a different system. In other words, do I have what I need to reproduce the execution on a controlled scenario if I need to? Log that and not much more.


It helps me to think "Why am I logging at all?" or "Why should logs exist?". They are there to help me understand what was going on when something didn't work as I expected. If everything is working fine I will rarely look at the logs. Therefore I try to always keep that in mind, that I will need this information on a moment of difficulty. Too much information is as bad as too little.