Leapmotion For Max
===========================================

![Project unmaintained](https://img.shields.io/badge/project-unmaintained-red.svg)

> This project is no longer under active development and will not be maintained. Feel free to get in touch if you wish to take over.

This is a simple Max external for Leap Motion Skeletal Tracking.

The object is inspired by aka.leapmotion, developed by Masayuki Akamatsu, but was re-written for the new tracking API. The object has separate outlets for gestures, hands, fingers, and frame information. Most of the features of the SDK are dumped as prefixed messages in Max.

The object was developed for research or experimental applications. Therefore, the object is in beta, and we do not guarantee any sustained development and support. The source code is available on Ircam-Forge.

## Compatibility
- Max 6+ 
- macOS 10.6 - 11.x (Intel 64 bit / Apple Silicon)
- Windows 32 / 64 bit

### macOS users on Monterey (macOS 12) or higher `EXPERIMENTAL`
Follow [these archived instructions](https://archive.vn/b6T0g) to get the LeapSDK to recognise their device. Included below for ease: 
1. Connect the LMC to the Mac
2. Open the "Recalibrate Device" window, and leave it open
3. Reboot your Mac
4. LMC should now show as connected!

### macOS users with Apple Silicon CPUs `EXPERIMENTAL`
Run Max 8 using the [Rosetta Translation Environment](https://developer.apple.com/documentation/apple-silicon/about-the-rosetta-translation-environment). 


## Features
- Full Skeletal Tracking
- Automatic left/right hand routing
- Automatic finger routing
- Build-in Leap Motion gesture recognition
- Simple record/replay based on MuBu

## Contact

Jules Françoise: <jules.francoise@ircam.fr>

## Author

This code has been initially authored by <a href="http://julesfrancoise.com">Jules Françoise</a> during his PhD thesis, supervised by <a href="frederic-bevilacqua.net">Frederic Bevilacqua</a>, in the <a href="http://ismm.ircam.fr">Sound Music Movement Interaction</a> team of the <a href="http://www.ircam.fr/stms.html?&L=1">STMS Lab</a> - IRCAM - CNRS - UPMC (2011-2015).

## Compiling

### Mac OS X

__requirements:__
- Max SDK
- Leap Motion SDK

Place the "LeapSDK" folder from Leapmotion SDK v2 to the root directory of the project and modify paths to the Max SDK in "build/xcode/leapmotion.xcconfig".

### Windows

__requirements:__
- Max SDK
- Leap Motion SDK

Modify paths to SDKs in the project settings (header path & library path)
