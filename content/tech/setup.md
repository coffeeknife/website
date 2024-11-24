+++
date = '2024-11-23T20:39:56-06:00'
title = 'Tech Setup'
+++
a quick rundown of my main tech equipment. pictures will be added someday

## personal

- **workstation:** custom budget build. intel i5-12400, intel arc a380, 16gb ddr4. arch linux. i game on here
- **laptop:** salvaged thinkpad t510. 6gb ram, original hard drive replaced with a 500gb ssd. arch linux. has a stripped screw, needs new thermal paste and a better wifi card, but otherwise runs very well.
    - can go up to 8gb ram, which would be nice.
    - eventually i want to swap the 1366x768 display out for a 1920x1080. i'm fairly confident there's a compatible display.
    - currently has an i5 processor in it, but can go up to i7. if i ever have to go without a desktop, i'll get an egpu enclosure for the expresscard slot and get an i7.
- **phone:** refurb'd galaxy note20. picked specifically because it's the last and best phone with an SD card slot. flashed from carrier firmware to stock, but not currently rooted. can be used as a mobile workstation in a pinch via a usbc dock + DeX.

## homelab

3 raspberry pis, a network switch and an imac with the display internally disconnected. they all sit on a rack built with an ikea LACK table.
- **etheirys:** the imac. sits on top of the rack. runs proxmox with a bunch of lxcs/vms for my services
    - vyos (virtual router), macos vm, ansible, mqtt server, caddy reverse proxy, jellyfin, homeassistant, kavita, vaultwarden, paperless-ngx, hydrus, immich
- **vulcan:** rpi 4, 4gb ram. usb hdd w/ 8tb storage on zfs, served over nfs. also runs nextcloud.
- **gunsmoke:** rpi3 model b. exclusively runs iot stuff. has a ConBee2 to talk to zigbee devices.
- **gallifrey:** rpi4, 2gb ram. runs a wireguard vpn for remote access.