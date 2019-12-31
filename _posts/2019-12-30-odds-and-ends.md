---
layout: post
title: Odds and Ends
subtitle: Tidbits of technical teachings 
---

#### Before I start reading... what is this page?
There are so many learnings that I would like to share via this blog, but not 
all of them warrant a fully fleshed out blog post. Instead of leaving these 
golden nuggets of information out, I figured that I would consolidate them to 
this page. I'll be continually adding useful information as I learn more.



### What's the difference between `.profile,` `.bashrc`, and `.bash_profile`?
 If you've recently gotten a new laptop and you're looking at setting your 
 whole environment up from scratch again, you might have wondered what the difference
 is between`.profile`, `.bash_profile`, and `.bashrc`. 
 
#### `.profile`: the non-bash specific stuff
  *    It is run whenever you start an interactive session (if it exists)
  *    Since it is run after /etc/profile, it takes precedence 
  *    Put your environment variables + things relevant to non-bash shells in here
  *    Must be compatible with non-bash shells
 
#### `.bashrc`: the bash specific stuff
  *    It's run whenever you start an _interactive_ non-login bash session
  *    Put any bash specific setup commands in here
 
#### `.bash_profile`: surprise, you don't really need one of these
  *    If for some reason there are environment variables you _need_ for bash
       but you don't want them to get loaded when you are using other shells, 
       you could put them here
 
To be honest, I feel like I'm only scratching the surface of this topic since there's
also information about `/etc/profile.d` and how sftp (and the like) are handled
that I'm skipping over. But hopefully this information will hold you over (or 
pique your interests).