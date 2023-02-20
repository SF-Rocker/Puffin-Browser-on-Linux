# Puffin Browser on Linux - Unofficial instructions about installing Puffin Internet Terminal on Linux
_Note: for **Windows** the browser is called **Puffin Secure Browser** or simply **Puffin Browser**, for **Linux** the browser is called **Puffin Internet Terminal**. Initially **Puffin Internet Terminal** is intended for **Raspberry Pi** devices, but this does not prevent it from being installed on a regular Debian-based computer.
You can still use the Chromium or Firefox browsers but the performance is barely acceptable, on Raspberry Pi devices or if you have a very low Internet speed, and a very weak device._

**Puffin Internet Terminal** is a fast functional browser for low end PCs and laptops. Puffin Internet Terminal provides fast page loading with **cloud-based content compression technology** and **saves traffic**.

## Why is this repository needed?
Cloudmosa has not published instructions on how to install Puffin on Linux systems, but it does officially provide support itself. 

**Benefits**:
- Cloud-based content compression technology with saving and encrypts traffic, because of this, the browser works very quickly and does not use much RAM
- Supports working with cloud storage.
- Own ads blocker, works with 97% efficiency
- Pretty cheap price, just $2 a month, first month for free*
- ~~Support for Adobe Flash technology (no longer in demand).~~

**Disadvantages**:
- Based on old version of Chromium engine, because of this, some sites refuse to working.
- No support for DRM and browser extensions

## Installation :
### For Debian-based Linux Distributions:
Note: only for i386 and amd64 processors! armv7/aarch64 in working process
#### First method - by adding Puffin repositories to the system
- Full version (Paid)
```
sudo apt update && sudo apt install wget -y && wget -q https://raw.githubusercontent.com/ZhymabekRoman/Puffin-Browser-on-Linux/main/puffin-internet-terminal.gpg -O- | sudo apt-key add - && sudo wget https://raw.githubusercontent.com/ZhymabekRoman/Puffin-Browser-on-Linux/main/puffin-internet-terminal.list -O /etc/apt/sources.list.d/puffin-internet-terminal.list && sudo apt update && sudo apt install puffin-internet-terminal -y
```
- Demo version*
```
sudo apt update && sudo apt install wget -y && wget -q https://raw.githubusercontent.com/ZhymabekRoman/Puffin-Browser-on-Linux/main/puffin-internet-terminal.gpg -O- | sudo apt-key add - && sudo wget https://raw.githubusercontent.com/ZhymabekRoman/Puffin-Browser-on-Linux/main/puffin-internet-terminal.list -O /etc/apt/sources.list.d/puffin-internet-terminal.list && sudo apt update && sudo apt install puffin-internet-terminal-demo -y
```
#### Second method - by manual installing deb package
- Full version (Paid)
```
sudo apt update && sudo apt install wget -y && wget -O /tmp/puffin-internet-terminal_full.dpkg http://github.com/ZhymabekRoman/Puffin-Browser-on-Linux/blob/main/deb/full/puffin-internet-terminal_8.2.4.705_`dpkg --print-architecture`.deb?raw=true && sudo dpkg -i /tmp/puffin-internet-terminal_full.dpkg; sudo apt install -f  && rm /tmp/puffin-internet-terminal_full.dpkg
```
- Demo version*
```
sudo apt update && sudo apt install wget -y && wget -O /tmp/puffin-internet-terminal_demo.dpkg http://github.com/ZhymabekRoman/Puffin-Browser-on-Linux/blob/main/deb/demo/puffin-internet-terminal-demo_8.2.4.705_`dpkg --print-architecture`.deb?raw=true && sudo dpkg -i /tmp/puffin-internet-terminal_demo.dpkg; sudo apt install -f  && rm /tmp/puffin-internet-terminal_demo.dpkg
```

## Running:
- Full version (Paid)
```
puffin
```
- Demo version*
```
puffin_demo
```


\* Honestly, I didn't notice any difference between the paid version and the demo version, the demo version is fully functional as the paid version, but does not require a subscription.
