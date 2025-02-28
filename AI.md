---
name: ww-video-vimeo
description: The `ww-video-vimeo` component seamlessly embeds a Vimeo video player into a website, offering control over playback features such as autoplay, mute, loop, and specific start times, while integrating with the Vimeo player API for enhanced video management.
keywords:
  - vimeo video player
  - embed vimeo video
  - autoplay
  - video mute
  - video loop
  - video controls
  - vimeo player api
  - video playback events
  - dynamic property binding
  - video seek time
---

#### ww-video-vimeo

Renders a Vimeo video player within a website with playback control features.

Properties:
- url: string - Vimeo video URL. Default: ""
- videoStartTime: number - Start time in seconds. Default: 0
- autoplay: boolean - Auto start playback. Default: false
- muted: boolean - Initial mute state. Default: false
- loop: boolean - Loop playback. Default: false
- controls: boolean - Show video controls. Default: true

Children: none

Special Features:
- Vimeo player API integration
- Video playback control
- Dynamic property binding support

Events:
- play: {value: number} - Triggered when video starts playing. Value is current time in seconds
- pause: {value: number} - Triggered when video is paused. Value is current time in seconds
- end: {value: number} - Triggered when video reaches the end. Value is current time in seconds

Variables:
- Is Playing: boolean - Indicates if video is currently playing
- Current time: number - Current playback time in seconds

Note: Do not set element or parent element height to 0 : a combination of width to 100% & aspectRatio to 16/9 will ensure the video is displayed correctly.

Example:
<elements>
{"uid":0,"tag":"ww-video-vimeo","name":"Vimeo Player","props":{"default":{"url":"https://vimeo.com/768475858","controls":true,"autoplay":false,"loop":false,"muted":false,"videoStartTime":0}},"styles":{"default":{"width":"100%","height":"auto","aspectRatio":"16/9"}}}
</elements>

