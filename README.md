# iRacing Sequence Director

An editing tool for iRacing replays. Create a sequence of 'nodes' consisting of a time, driver and camera and the application will play back the sequence of shots for recording or viewing. Includes support for recording in iRacing itself using the built-in capture facility (no need for any external software) or can be used with capture software (OBS, etc.) if you have overlays you want to use.

Each replay has its own save file so no need to edit everything in one session.

![App screenshot](https://i.ibb.co/D1czQ68/image.png)

## Installation

- Download the latest version from the [Releases](https://github.com/GetUpKidAK/iRacingSequenceDirector/releases) page. 
- Extract to your preferred location and run iRacingSequenceDirector.exe with a replay open

## How to use

- With a replay and Sequence Director open, use the playback controls to get to the desired time, select a driver and camera, and click 'Store Node'.

![Create a node](https://i.ibb.co/LPyxyjR/image.png)

This adds the node to the list for playback:

![Node list](https://i.ibb.co/bb3YJv8/image.png)

And that's pretty much it! Repeat the process, adding nodes where desired. You can edit or delete existing nodes by selecting them and picking a new car/camera combination, or pressing 'Delete Node'.

Once you've finished 'editing' rewind back to where you'd like the replay to start and press Play to view what you've created, or Record to capture it using the in-sim capture or OBS. Guides for setting that up are below...

Here's a quick video showing the basic features in an early release version.

[![How to Use](http://img.youtube.com/vi/7DBsk7VQ1dU/0.jpg)](https://www.youtube.com/watch?v=7DBsk7VQ1dU)

## Guides

### Setting up iRacing in-sim capture

- To use the in-sim recording the 'Enable video and screen capture' setting must be enabled in iRacing.
You'll need to restart the sim if this wasn't already enabled.

![Misc Settings](https://i.ibb.co/Rppt27d/Misc-Settings.jpg)

- Enable the 'iRacing Capture' setting in Sequence Director under the Options -> Recording Capure Method menu:

![Capture settings](https://i.ibb.co/Z20sYnV/i-Racing-Capture.png)

**Notes:**
The videos are saved in My Documents/iRacing/videos.

You can adjust the output quality and file format of the recordings in the app.ini file. The default is 720p30fps.
This is found under My Documents/iRacing. The lines are commented but look like this:

![app.ini](https://i.ibb.co/92cbP7M/appIni.png)

### Setting up OBS recording

To use OBS recording without manually starting the recording process, you'll need to configure a hotkey for it.

- Via the Settings -> Hotkeys menu in OBS set 'Ctrl+Shift+R' as the hotkey for both Start and Stop Recording:

![Hotkeys](https://i.ibb.co/89hcks2/image.png)

- Enable the 'OBS' setting in Sequence Director under the Options -> Recording Capure Method menu:

![Capture settings](https://i.ibb.co/DwTFbKn/image.png)

**Note:** Only [OBS Studio](https://obsproject.com/) is supported at this time. The hotkey required can't be changed at this time.

## Support

You can ask any questions or get support for the app over at the [iRacing Forums](https://forums.iracing.com/discussion/605/iracing-sequence-director-editing-tool-for-replays).

If you *really* like the app, you can make a donation via [PayPal](https://paypal.me/GetUpKidAK?locale.x=en_GB). Thanks!
