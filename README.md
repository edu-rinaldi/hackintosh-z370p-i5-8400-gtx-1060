# Hackintosh High Sierra 10.13.6 Coffee-Lake 

### Main Specs:
	* Asus z370-p Motherboard
	* Intel core i5-8400 Coffee-Lake
	* EVGA GTX 1060 3GB
	* 8GB DDR4 2400mhz

**Note:**
1. If you have my same motherboard, cpu _(or similar cpu)_ and GPU you can directly copy and paste my `efi ssd` folder in your efi partition.
2. If you have my same motherboard and cpu _(or similar cpu)_, you can copy my `efi ssd` folder, but you should:
	* remove `WhateverGreen.kext` from *EFI/CLOVER/kexts/other/*
	* regenerate `SSDT.aml` ( you can follow [this](https://www.tonymacx86.com/threads/guide-generate-ssdt-for-coffee-lake-cpu.238311/) guide )
	* change config.plist :
		- untick `System parameters->NvidiaWeb`
		- use another ig-platform-id and enable intel gpu ( google is your friend )

If you're **NOT** in one of those two cases, you should **NOT** use my efi folder.

## Enable Nvidia Card
Checkout [this](https://www.tonymacx86.com/threads/fix-for-failure-nvidia-web-driver-on-high-sierra-black-screen-panics.234390/) guide from tonymacx86.com , it's easy to follow and it works like a charm :+1:

## Final results
**What works?**: 
> everything except for HDMI Audio from Nvidia GPU (it can be fixed using *VooDooHDA.kext* but it's not good to have 2 "drivers" that do the same thing. (If you can find a fix you can suggest it to me i will add it to the repo with credits :sunglasses:
