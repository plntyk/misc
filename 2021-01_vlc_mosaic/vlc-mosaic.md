# VLC Mosaic 2021-01

SD:
vlc --color --vlm-conf mosaic1.vlm.conf --mosaic-width=720 --mosaic-height=576 --mosaic-keep-picture --mosaic-rows=2 --mosaic-cols=2 --mosaic-position=1 --mosaic-order=1,2,3,4
HD
vlc --color --vlm-conf mosaic2.vlm.conf --mosaic-width=1920 --mosaic-height=1080 --mosaic-keep-picture --mosaic-rows=2 --mosaic-cols=2 --mosaic-position=1 --mosaic-order=1,2,3,4
vlc --color --vlm-conf mosaic3.vlm.conf --mosaic-width=1920 --mosaic-height=1200 --mosaic-keep-picture --mosaic-rows=2 --mosaic-cols=2 --mosaic-position=1 --mosaic-order=1,2,3,4
vlc --color --vlm-conf mosaic4.vlm.conf --mosaic-width=1920 --mosaic-height=1200 --mosaic-keep-picture --mosaic-rows=2 --mosaic-cols=2 --mosaic-position=1 --mosaic-order=1,2,3,4
vlc --color --vlm-conf mosaic-tvh.vlm.conf --mosaic-width=1920 --mosaic-height=1200 --mosaic-keep-picture --mosaic-rows=2 --mosaic-cols=2 --mosaic-position=1 --mosaic-order=1,2,3,4 --no-video-deco --qt-start-minimized
HD++
vlc --color --vlm-conf mosaic5.vlm.conf --mosaic-width=1440 --mosaic-height=808 --mosaic-keep-picture --mosaic-rows=2 --mosaic-cols=2 --mosaic-position=1 --mosaic-order=1,2,3,4


 vlc file:///mnt/pictures/bg/wallpaper_1920x1200.jpg --image-duration=1 --image-fps=10
 --http-host host
 --http-port port
  --http-password
  -I http
 ./vlc --color -I http  --http-host localhost  --http-port 9999 --http-password vlc


 
## Sources 
https://wiki.videolan.org/VLC_HowTo/Make_a_mosaic/
https://wiki.videolan.org/MosaicExampleSetup/
https://wiki.videolan.org/Documentation:Streaming_HowTo/VLM/
https://forum.videolan.org/viewtopic.php?t=58646
https://www.vlc-forum.de/thread/2484-mosaik-outputs-flackern/
https://forum.videolan.org/viewtopic.php?t=147932

## Issues 

- mosaic widt+height wie hintergrundbild
- vlc does not support multiple streams per transponder; vlc blocks dvbadapter with one stream
- use Linux: tvheadend, vdr; Windows: dvbviewer for non-blocking-streaming
- too many open files error 

### cmdlines

Debug: -vvv 2> vlc_$(date +%Y-%m-%d-%H-%M-%S).log

--no-video-deco --no-embedded-video --video-x=1 --video-y=1 --qt-start-minimized --no-video-title-show --zoom=0.75 --noaudio

## Misc

cvlc --video-x=1 --video-y=1 --zoom=0.75 <file1>
--video-x=1 --video-y=1 --zoom=0.75 
--video-x=961 --video-y=1 --zoom=0.75
--video-x=1 --video-y=541  --zoom=0.75
--video-x=961 --video-y=541 --zoom=0.75

#setup channel4 option dshow-fps=25
setup channel4 option dshow-size="720x405"


