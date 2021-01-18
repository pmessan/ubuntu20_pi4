# Ubuntu 20.04.1 Image for Raspberry Pi 4
This image is based on the unofficial arm64 Ubuntu 18.04.4 Server image for raspi 4B's available [here](https://github.com/TheRemote/Ubuntu-Server-raspi4-unofficial/releases). I tweaked it an upgraded it to Ubuntu 20.04 to produce the image in this repo. If you're looking for an Ubuntu 18.04 image, you're in luck. Head over [here](https://github.com/pmessan/ubuntu18_raspi4) to download it.

I added the following feature so you don't need a usb keyboard and mouse to setup your pi4.

## Tweaks

* [Pifi](https://github.com/rohbotics/pifi) : This was added so that the raspi comes up as a wifi access point on first boot. Connect using password `robotseverywhere`. From there you can run `ssh ubuntu@ubuntu.local` with password `ubuntu18` to access the pi via ssh, then add your own network using `sudo pifi add NETWORKNAME NETWORKPASSWORD`. Next, `sudo reboot` and within a few minutes, your pi should connnect to your own network.

## Misc. 

If you found any bugs, let me know by issuing a pull request.

For more information on how this image was created, and how you too can create your own custom image for your raspi, check out [this GitHub gist! - to be published]()


Clone this repo to download this image and flash it to your pi4 with [etcher](https://www.balena.io/etcher/). Happy Coding!
