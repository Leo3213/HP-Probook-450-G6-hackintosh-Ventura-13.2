# HP-ProBook-450-G6-Hackintosh
My HP ProBook 450 G6 i5 Hackintosh laptop configuration.

You will need to add your own:
platform id information
and map your own usb ports!!!

THE SMBIOS IM USING IS MacBookPro15,2

I put these commands at the top so everyone would see them :)

*
Readable brightness keys troubleshoot:

Do a hard shutout and keep the power button down for 30 seconds
This clears the Laptops EC.



After install to get sleep/wake working run theses commands:

    "sudo pmset -a hibernatemode 0"
    "sudo pmset autopoweroff 0"
    "sudo pmset powernap 0"
    "sudo pmset standby 0"
    "sudo pmset proximitywake 0"
    "sudo pmset tcpkeepalive 0"
    "sudo pmset lidwake 0"
    
after install to enable TRIM (TO PROLONG THE LIFE OF YOUR SSD) run this command:

    Type "sudo trimforce enable" and hit return or enter.
    
    Carefully read the important notice and if you still wish to proceed, hit Y.
    
If you would like to disable TRIM, you can use the command:
    
    "sudo trimforce disable"


This Config uses OpenCore as the bootloader and I am currently running macOS Ventura 13.2.1 as OS

(everything works that I'm aware of)

Laptop Specifications:

    Intel Core i5-8265U processor (Skylake)
    Intel UHD Graphics 620
    16 GB DDR4-2400 SDRAM (8 GB x 2) RAM
    15.6 Full HD Display
    Synaptics PS2 TouchPad
    720p HD HP Camera


(1) USB 3.1 Type-C Gen 1 (Power Delivery, DisplayPort) (2) USB 3.1 Gen 1
(1) USB 2.0 (Powered port)
(1) HDMI 1.4b
(1) RJ-45/Ethernet port
(1) Headphone/microphone combo jack 
(1) AC power port
(1) SD Card reader



BIOS Setup:

    Disable Fast Boot
    Disable Power On when AC Detected
    Disable Power On when Lid is Opened
    Disable Secure Boot
    Disable Legacy Boot
    Enable Turbo Boost
    Enable Hyperthreading
    Enable Multi-Processor
    Enable VT-x
    Disable Wake on LAN
    Video Memory Size: 64MB
    Enable Runtime Power Management
    Disable Extended Idle Power States
    Enable Deep Sleep
    Disable Wake when Lid is Opened
    Disable Wake on USB
    Enable Power Control

What works:

    macOS Ventura 13.2.1
    SD CARD READER
    UEFI booting via Opencore.
    Built-in keyboard (with special function keys)
    Built-in trackpad
    Brightness Control Hotkeys
    Audio Control Hotkeys
    HDMI Video and Audio
    Integrated Camera
    Native Wifi and Ethernet
    Bluetooth and AirDrop
    Native audio with AppleALC, including headphone
    Built-in mic
    Native power management
    Battery status
    USB Ports
    Ethernet
    Audio on internal speaker and headphone
    Sleep and Wake

What doesn't work:
    Fingerprint Reader
    Itunes movies (its because were using intel onboard graphics)

(THE Wifi-bluetooth CARD WAS REPLACED WITH THE FOLLOWING!)




Thanks to:
The entire internet.

only 1% is my actual doing. this config is the result of many other config fixes and tips. I just combined them into a working config.

this is designed for the i5 variant.

(I rebuilt the config manually with the same settings so it wouldn't be corrupt)

Below is a link to my configuation

if anyone wants to make this config better for everyone let me know your fixes and ill include them and give you credit :)
