---
layout: page 
title: endless seashore 
---

FFmpeg gained several audio filters recently, including [sinusoidal amplitude modulation](http://git.videolan.org/?p=ffmpeg.git;a=blob;f=libavfilter/af_tremolo.c;h=572e9e3b56082e474ec4480addeb19d512b1b2b3;hb=HEAD) and a [colored noise source](http://git.videolan.org/?p=ffmpeg.git;a=blob;f=libavfilter/asrc_anoisesrc.c;h=e4d4013749225ae2f0321f8a7c6e082fd98d55e5;hb=HEAD).
I guess that means that everyone with FFmpeg installed on their system can now generate endless seashore sounds. This is important work.

<code>
ffplay -f lavfi -i anoisesrc=colour=brown -af tremolo=f=0.1:d=0.9
</code>
