---
layout: post
title: raspberry pi fun
tag: [fractal, projects]
---
so i finally got my wireless dongle and in the span of 24 hours i have re-purposed
the pi to an cherry pi server which works but in an very weird way so i was following
an [tutorial online](http://fomori.org/blog/?p=687) and as usual something went wrong.
The first thing was that for the script that automatically starts up on boot it needed a cli
program called [gnu screen](https://www.gnu.org/software/screen/) but it didn't work for the terminal
so i tried a different start up script but then the folder which held the music wasn't found by the
script (i think it was because i was was pointing the dir to .local which messed it up somehow)so then
i spent the rest of the evening trying out different things in till i found a real simple method using
something called crontab which i found on the cherry music [wiki](https://github.com/devsnd/cherrymusic/wiki/Setup-guide#tips-and-tricks) using two simple commands

{% highlight bash %}
EDITOR=nano crontab -e
{% endhighlight %}       

then inside the editor:

{% highlight bash %}
@reboot cd /path/to/your/cherrymusic/installation ; python cherrymusic
{% endhighlight %} 

which worked once i changed the dir where the music was. Amazingly it runs pretty well
for something that is on an low spec system. Which is interesting since i always found
the mini dnla server (which i had before this) to be really glitchy and also i could
never find a good dnla client that wouldn't glitch up after a while      
![cherry music](/images/cherrymusic.gif)
