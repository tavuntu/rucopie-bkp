# RucoPie

:warning: This is in early development stages

RucoPie aims to be a simple (yet customizable), alternative to systems like [RetroPie](https://retropie.org.uk/), [Lakka](https://www.lakka.tv/) or [Recalbox](https://www.recalbox.com/). It targets Raspberry Pi 3 and 4 devices to be used via HDMI.

## Features

* Fast environment, built on top of [DietPi](https://dietpi.com/) (highly optimized Raspbian)
* Support for pretty much every Libretro emulator
* For the UI:
    * Multi language
      * :uk: English
      * :es: Spanish
      * :fr: French
    * Flexible theme system
      * Single-static backgrounds
      * Multiple-static backgrounds
      * Multiple-dynamic backgrounds (useful to simulate depth)
      * Color palette customizer
      * Shadows/Opacity/Bounding controls
      * Custom icons per theme
      * Custom audio per theme
    * Thread-based IO (helps with performance)
    * Pixel-perfect in any resolution that is a multiple of 640x360, such as:  
      * [Standard HD](https://en.wikipedia.org/wiki/720p)
      * [Full HD](https://en.wikipedia.org/wiki/1080p)
      * [Quad HD](https://en.wikipedia.org/wiki/1440p)
      * [4K UHD](https://en.wikipedia.org/wiki/4K_resolution)
* Automatically scaled, pixel perfect games (RetroArch) in any resolution
* Extra video options for bilinear, stretching and other tweaks.
* Audio equalizer with custom profiles
* Vertical mode
* WiFi setup screen (non-terminal based)
* Thumbnail Game States

![](https://i.postimg.cc/3N1x2sGJ/1.png)
![](https://i.postimg.cc/7Pnhv2R8/2.png)
![](https://i.postimg.cc/Gh32bp0B/3.png)

## How to try this out:

* Install DietPi on your Raspberry Pi and start the system
* Connect to the Internet and enable Onboard Wifi
* Enable automatic boot
* Set OpenSSH as default SSH server with ```dietpi-software``` (this is for roms transferring)
* Run the following script and follow the steps

```bash
curl -s https://raw.githubusercontent.com/tavuntu/rucopie-bkp/main/setup.sh | bash -s
```

* Reboot, and it should be ready to go!

## Things to do/fix:

* Integer coordinates for background to behave smootly
* filesystem speed (add LFS)  (done)
* Persist optimal resolutions for cores and general preferences (done)
* Support joysticks via USB (done-ish)
* Wireless internet conexion screen (in progress)
* More video options (in progress)
* Add more themes
* Add animated boot screen
* Add background music manager
* Add audio equalizer with profiles, if possible
* Add no-copyright roms
* Bluetooth joystick support
* Locale/Country settings
* Skip button while mapping joystick for UI
* Change the terminal banner
* Add Favorites
* Recently played
* All games
* Vertical mode
* Add other languages (done, ES and FR)
* Game states with thumbnails
* Other things not in this list

---

## Notes
* RucoPie was inspired by [RGB-Pi](https://www.rgb-pi.com/)
* Not everything described in here is implemented yet
