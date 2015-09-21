audioplayer
===========

Simple WinRT component for playing sound effects using XAudio2. Based on the [MSDN XAudio2 sample](https://code.msdn.microsoft.com/windowsapps/Basic-Audio-Sample-9a5bb0b7) but makes it easier to use. Supports Windows 8.1+ and Windows Phone 8.1+.

#### Features
* Extremely easy to use
* Supports playing multiple sounds at the same time (unlike MediaElement)
* Abstracts away the complexities of DirectX

#### Usage

**C#**

    Em.Media.Playback.AudioPlayer player = new Em.Media.Playback.AudioPlayer();
    player.PlaySound(new Uri("ms-appx:///Assets/your-sound.wav"));

**WinJS**

    var player = new Em.Media.Playback.AudioPlayer();
    player.playSound(new Windows.Foundation.Uri("ms-appx:///Assets/your-sound.wav"));

Make sure you make player a glogal variable.

When player goes out of scope music will stop.

Comments and pull requests are more than welcome.
