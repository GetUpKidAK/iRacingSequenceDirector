# iRacing Sequence Director

Create your own replay edits without any required editing knowledge. Create 'nodes' at points in your replay and choose this point to either cut to a different driver and/or camera or skip to further ahead in the replay. Sequence Director will then play this sequence of shots and time-skips back for recording or viewing.

- No need for additional editing knowledge or software
- Useful for anyone using editing software for testing cuts in iRacing and recording sequences of shots without recording multiple clips
- Support for recording using iRacing's built-in capture facility (no need for any external software)
- Support for capturing with overlays for race standings, etc. when using OBS Studio
- Each replay has its own save file so no need to edit everything in one session
- Works with custom cameras for setting up your own shots with the iRacing camera tool
- Resizeable window for users with limited screen space

![App screenshot](https://i.ibb.co/6nGVxfh/Main.png)

## Installation

- Download the latest version from the [Releases](https://github.com/GetUpKidAK/iRacingSequenceDirector/releases) page. 
- Extract to your preferred location and run iRacingSequenceDirector.exe with a replay open

## How to use
### Camera Changes
A Camera Change node will cut to the selected car and camera combination when the desired frame is reached
- Use the playback controls to get to the desired time, select a driver and camera, and click 'Add Cam Change'.

![Add Cam Change](https://i.ibb.co/6FJ9KNk/Add-Cam-Change1.png)

This adds the node to the list for playback:

![Node list](https://i.ibb.co/KrNq37Z/Add-Cam-Change2.png)

And that's pretty much it! Repeat the process, adding nodes where desired. You can edit or delete existing nodes by selecting them and picking a new car/camera combination, or pressing 'Delete Node'.

### Frame Skips
A Frame Skip node will, when the desired frame is reached, jump ahead to the next node in the list.
- Use the playback controls to get to the point in the replay where you want to skip _from_ and click 'Add Frame Skip'.

![Add Frame Skip](https://i.ibb.co/HCrcZKp/Add-Frame-Skip-P1.png)

This will add a disabled Frame Skip node to the list.

![Node list](https://i.ibb.co/9qXY14K/Add-Frame-Skip-P2.png)

- Now you can use the playback controls to find the point you want to skip _to_ and select your desired car/camera combination. Add a Camera Change node as above.

![Frame Skip Added](https://i.ibb.co/VptvZkM/Add-Frame-Skip-P3.png)

Now the Frame Skip node will update to show which frame it will skip to.
_In this example, once the replay reaches frame #49942 it will jump ahead to frame #58772 and cut to the selected camera._

**Note:** If you're making long jumps in the replay and it takes too long or doesn't skip far enough, please check the guides below.

Once you've finished 'editing' rewind back to where you'd like the replay to start and press Play to view what you've created, or Record to capture it using the in-sim capture or OBS. Guides for setting that up are below...

### Video
Here's a video explaining some of the basics in an early version (pre-frame skipping). I'll try and do a video explaining frame skips soon:

[![How to Use](https://i.ibb.co/Lpp6wTr/Thumbnail-Play.png)](https://www.youtube.com/watch?v=amghnO6rE7U)

## Guides/More Info

### Using Frame Skip Nodes

iRacing has a 'replay spooling' option which can cause issues with skipping over certain lengths of the replay. If this is enabled you may get long delays when skipping and/or it may stop before it gets to the point you want to skip to. You can stop these issues by disabling this setting under the 'Replay' section of the in-sim options:

![Spooling option](https://i.ibb.co/44nTQbf/Spooling1.png)

You need to restart the sim after changing this setting. When disabled this can also limit the size of the replay when the sim is in a live session so make sure you only disable this when editing if you run longer races.

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

### Using custom cameras

You can use your own modified cameras using the iRacing Camera Tool. I've written a basic guide on how to do that here: https://docs.google.com/document/d/1EOWFVIqH9OppcqurmR_wzZs_czvqj3_zsKU_qR6fKfo/edit?usp=sharing

## Support

You can ask any questions or get support for the app over at the [iRacing Forums](https://forums.iracing.com/discussion/605/iracing-sequence-director-editing-tool-for-replays).

If you *really* like the app, you can make a donation via [PayPal](https://paypal.me/GetUpKidAK?locale.x=en_GB). Thanks!
