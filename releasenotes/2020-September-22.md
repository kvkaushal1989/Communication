# Release Notes for September 22, 2020

## Android SDK

### Features available
*   1-1 and 1-N audio/video call outgoing and incoming
*   Join group audio/video call
*   Place a call to PSTN
*   Render Video from remote participants
*   Render screenshare from remote participants
*   List audio and video devices
*   Ability to preview local video camera
*   Share local camera stream
*   Mid-call operations (mute/unmute)
*   Mid-call operations (Turn Video on/Turn Video off)
*   Mid-call operations (Add/Remove remote participant to an ongoing call)
*   Push notification support for incoming call

### Onboarding
The SDK is packaged as FAT SDK artifact with all ABIs (arm64-v8a, armeabi-v7a, x86_64) supported on the Android platform.
<br/>Please refer to the [Microsoft docs](https://review.docs.microsoft.com/en-us/azure/project-spool/quickstarts/voice-video-calling/getting-started-with-calling) of how to bootstrap a Calling sample application on android.

### Limitations
* While ability of making PSTN calls is availble in the SDK, you need a PSTN number in ACS to make the call. The ability to aquire the number comes in October
* On mobile and desktop at any given time client multiple receive video streams might result in greater number of video freezes and/or quality fluctuations. We are working on improving the experience. We recommend to limit nimber of incoming streams to one if you experience such issues
* If you specified a scope for the User Access Token (Chat, VoIP or PSTN) the scope (s) for PSTN and VoIP will not be enforced 
*  We don't support x86 simulators, arm7 support is coming soon

## iOS SDK

### Features available

*   1-1 and 1-N audio/video call outgoing and incoming
*   Join group audio/video call
*   Place a call to PSTN
*   Render Video from remote participants
*   Render screenshare from remote participants
*   List audio and video devices
*   Ability to preview local video camera
*   Share local camera stream
*   Mid-call operations (mute/unmute)
*   Mid-call operations (Turn Video on/Turn Video off)
*   Mid-call operations (Add/Remove remote participant to an ongoing call)
*   Push notification support for incoming call

### Onboarding
The SDK is released for the following platforms: arm64 and x86_64 (simulator)
<br/>Minimum supported iOS SDK version is 12.0
<br/>Please refer to the [Microsoft docs](https://review.docs.microsoft.com/en-us/azure/project-spool/quickstarts/voice-video-calling/getting-started-with-calling) of how to bootstrap a Calling sample application on iOS.

### Limitations
* While ability of making PSTN calls is availble in the SDK, you need a PSTN number in ACS to make the call. The ability to aquire the number comes in October
* On mobile and desktop at any given time client multiple receive video streams might result in greater number of video freezes and/or quality fluctuations. We are working on improving the experience. We recommend to limit nimber of incoming streams to one if you experience such issues
* If you specified a scope for the User Access Token (Chat, VoIP or PSTN) the scope (s) for PSTN and VoIP will not be enforced 

## JS (Web) SDK

### Features available
*   1-1 outgoing and incoming calling
*   Join group call
*   Allow to join call with microphone mute
*   Allow to set camera device before call and to switch camera device during call
*   Allow to enable/disable camera in-call and while call is ringing/incoming
*   DeviceManager support to list audio and video devices
*   DeviceManager support to set audio devices
*   Remote video and screen-sharing rendering
*   Screensharing support
*   Local camera device preview rendering
*   Mid-call operations (mute/unmute)
*   Mid-call operations (Turn Video on/Turn Video off)
*   Mid-call operations (Add\Remove Participant)
*   Call and RemoteParticipant states
*   Property changed and collection updated events
*   Place a call to PSTN

### Onboarding
Please refer to the [Microsoft docs](https://review.docs.microsoft.com/en-us/azure/project-spool/quickstarts/voice-video-calling/getting-started-with-calling) of how to bootstrap a Calling sample application on web.

### Limitations
* While ability of making PSTN calls is availble in the SDK, you need a PSTN number in ACS to make the call. The ability to aquire the number comes in October
* On mobile and desktop at any given time client should have only one remote video stream running, multiple receive streams will result in greater number of video freezes and/or quality fluctuations. You may still choose to have multiple streams on desktop but your experience will be degraded. We will update you when we officially support up-to 5 incoming streams (4 video+1 ss) on desktop.
* If you specified a scope for the User Access Token (Chat, VoIP or PSTN) the scope (s) for PSTN and VoIP will not be enforced 
