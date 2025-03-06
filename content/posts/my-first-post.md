+++
date = '2025-02-27T12:25:13-05:00'
draft = false
title = 'On Tutorials'
+++

## Tutorials are awful

Imagine a graph of tutorials-per-capita consumption over time. For most of human history, we're blissfully free of them.
No blog posts about git rebase, no semi-official Reddit pages about where the Windows control panel is hiding, no
desperate smartphone-rendered YouTube videos on how to light a pilot light two hours before service starts. Alright
that last one might be a little specific. Regardless, suddenly in the 20th century, it's hundreds or maybe thousands of tutorials per year.

And they never work!

Okay, that's not true of course. I think the frustration I feel from them though is instructive. Because, while of course
there are actually bad tutorials, mostly I think tutorials are pretty carefully constructed. But they're frozen in time.
And the most needed tutorials are technical tutorials, and are you even programming if you're not using the absolute
most-bleeding edge Javascript framework?

We have to sweat the details with technical work. The compiler cares if you forget a semicolon, and those technical details
change all too quickly for technical tutorials to have much staying power. While ancient historians are allowed lengthy digressions
on the nature of humanity and power that may ring true a thousand years later, a technical tutorial won't even know what text
editor you'll be using in two decades.

But also, wouldn't it be great if the tutorials were a compiled language? Obsolete references getting automatically flagged for review?
Code examples runnable within the text itself?

Actually, that's thinking too small. The tutorial *itself* should solve the problem! A computer can be made to always interpret the text
the same way, so these tutorials could be exchanged between writers to solve all sorts of problems!

Oops, I re-invented programming languages again.

This kind of thinking, however, is what leads to my interest in Nix. The kinds of problems we solve tend to need to be solved over and
over, and it is my hope the Nix's emphasis on reproducibility will make these not-very-new new problems easier to address.

So this Hugo website is running on a NixOs computer in my room. Nix handles the installation and configuration of the software. So,
I write Nix files that tell the computer where to get the blog, the Hugo theme, the NGINX reverse proxy, the Let's Encrypt certificate,
and maybe some other stuff that I forgot about.

Was this the easiest way to get a website up and running? Absolutely not. But it was the most interesting. So big shout out to
Janne Pulkkinen, aka Matoking, whose tutorial [Deploying Hugo site using NixOS and nginx](https://matoking.com/blog/2023/07/08/deploying-hugo-site-using-nixos-and-nginx/)
was extremely helpful! And my advice to myself when I'm feeling frustrated with a technical problem and a tutorial is: It's
probably not the tutorials fault.

