RTMBookmarklet
==============

Enhanced version of the Remember The Milk Bookmarklet for music sites.

Currently supports adding a task for the currently playing song on [Songza](http://songza.com).

You can use this bookmarklet by dragging the "Add to RTM!" link below to your browser's bookmarks toolbar.

[Add to RTM](javascript:(function(){h="www.rememberthemilk.com";p="/services/ext/addtask.rtm";a=$(".szi-current-song .szi-artist").text();s=$(".szi-current-song .szi-song").text();sa=s+a;cp="http://"+h+p+"?t="+encodeURIComponent(sa)+"&tx=test";w=window.open(cp,"addwindow","status=no,toolbar=no,width=475,height=260,resizable=yes");setTimeout(function(){w.focus()},500)})();)