# Video Segments

Like everything else used to build Hydrogen, the video player is also open-source. By using [video.js](http://videojs.com) in a Chromium wrapper, we don't have to mess around pulling in VLC-like libraries to support our existing video content.

Theoretically we should also be able to support transcripts in the future. We could also parse these transcripts to static text so that they can be included below the video itself (which then means we benefit from the full-text-search included within the application).

{% raw %}
<video id="videoEmbed" class="video-js vjs-default-skin vjs-16-9 vjs-big-play-centered vjs-fluid" controls preload="auto" data-setup="{}">
  <source src="assets/video.mp4" type="video/mp4">
  <p class="vjs-no-js">To view this video please enable JavaScript, and consider upgrading to a web browser that supports HTML5 video</p>
</video>
{% endraw %}

This video section is from *Mastering React*.
