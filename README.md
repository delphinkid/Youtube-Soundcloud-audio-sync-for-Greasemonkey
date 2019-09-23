# Youtube-Soundcloud-audio-sync-for-Greasemonkey
Greasemonkey script that embeds a soundcloud link in the description section of youtube videos and syncs the audio track with the video.

  This is an experimental script meant to embed an audio track from a soundcloud link in the description section of a youtube video. To use it, go to the soundcloud track you wish to embed and click 'share', then 'embed', and copy the code provided into a text editor. From this, copy the number right after where it says "api.soundcloud.com/tracks/", usually it is nine digits long. Finally, in the description of your youtube video, put "soundcloudsync(#########)", with the number you copied where the # symbols are.
  When you load the page for the video, the soundcloud track should be embedded in the description section of the video. Pausing and un-pausing the video will pause and un-pause the soundcloud audio, and changing your playback position on the video will update the soundcloud playback to the same timestamp. If the video and audio become desynced, just pause and un-pause the video to synchronize the tracks. If the video starts playing while the soundcloud audio is still paused, just click play on the soundcloud track and then pause and unpause the video to resync the tracks.

 Some known bugs:
 -occasionally, the soundcloud player does not load. Refreshing the page should fix this.
 -sometimes, following a link to another youtube page causes the video player to to persist on top of the new page. Refreshing the page should fix this.

This is still in its early phases, so there are likely more bugs I haven't found yet. Most bugs seem to be fixed by refreshing the page. If you encounter any issues that refreshing does not fix, you can disable the script in the greasemonkey menu.

TO INSTALL:
Make sure you have greasemonkey installed. Go to the youtube_soundcloud_sync.user.js file page and click 'raw'. A window should open allowing you to install the userscript.
