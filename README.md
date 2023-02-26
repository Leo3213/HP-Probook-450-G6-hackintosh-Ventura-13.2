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

    SD Card Reader (as of release 1.0.4 it now works thaks to user, "robi62"

Laptop Specifications:

    Intel Core i7 6200U CPU (Skylake)
    Intel HD 520 Graphics
    8GB DDR4-2133MHz RAM
    15.6 Full HD Display
    Synaptics PS2 TouchPad
    
(THIS CARD WAS REPLACED WITH THE FOLLOWING!)


    2 USB 3.0 Ports, 2 USB 2.0 Ports
    HDMI Port
    SD Card Reader
    Kingston SSD disk A400 120GB (upgraded)
    sata m2 500 gb ssd.
    
    soon i will be repacing dvd drive with 1tb hdd
    for windows backups and mac timemachine backups 
    (it will be partioned in 2)

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
    USB 3.0 Ports
    Ethernet
    Audio on internal speaker and headphone
    Sleep and Wake

What doesn't work:
    Fingerprint Reader
    Itunes movies (were using intel onboard graphics)

Thanks to:
The entire internet.

only 1% is my actual doing. this config is the result of many other config fixes and tips. I just combined them into a working config.

this is designed for the i5 variant.

(I rebuilt the config manually with the same settings so it wouldn't be corrupt)

Below is a link to my configuation

if anyone wants to make this config better for everyone let me know your fixes and ill include them and give you credit :)
