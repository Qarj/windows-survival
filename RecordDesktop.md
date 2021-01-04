# Record Desktop

## VLC
View Menu -> Ensure Advanced Controls is ticked

CTRL-C
* Capture mode -> Desktop
* Desired frame rate -> 30 f/s
* Show more options -> check
* Edit Options - set to: ` :screen-fps=30.000000 :live-caching=300 :screen-height=1080 :screen-width=1920` or `2560` to capture left screen
  Or `:screen-fps=30.000000 :live-caching=300 :screen-height=1440 :screen-width=2560` for 1440p
* Edit Options - set to: ` :screen-fps=30.000000 :live-caching=300 :screen-height=1080  :screen-left=1920` to capture right screen
  Or `:screen-fps=30.000000 :live-caching=300 :screen-height=1440 :screen-left=2560` for 1440p
* Play Drop Down -> Convert
  * Set Profile to `Video - H.264 + MP3(MP4)`
  * Destination file -> Click Browse
    * Copy Paste this to filename `%USERPROFILE%\Videos\MyDesktopCapture.mp4`
* Click Start

Recording will start immediately - no need to click red record button!

Click the Stop button to end recording.

https://superuser.com/questions/782959/how-to-record-the-desktop-in-vlc-media-player-second-screen

## Bandicam


