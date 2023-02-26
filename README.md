# HP-ProBook-450-G3-Hackintosh
My HP ProBook 450 G3 Hackintosh laptop configuration.

(NO MORE UPDATES FOR THE CONFIG ONLY BECAUSE A COWORKER SPILLED LIQUID ON THE LAPTOP AND FRIED IT LOL)

I NOW OWN A HP PROBOOK 450 G6 I5 VARIANT AS OF 3-2-22

I put these commands at the top so everyone would see them :)

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


This Config uses Clover as the bootloader (but its the version 5144 which uses open core runtime) and I am currently running macOS BigSur 11.6.3 as OS

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

    macOS BigSur 11.3
    UEFI booting via Clover with Openruntime.
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
    SD Card Reader (as of release 1.0.4 it now works thaks to user, "robi62"

Thanks to:
The entire internet.

only 1% is my actual doing. this config is the result of many other config fixes and tips. I just combined them into a working config.

Most other guides were designed for the i5 version of this laptop, not the i7.

this is designed for the i7 variant.

(I rebuilt the config manually with the same settings so it wouldn't be corrupt)

Below is a link to my configuation

if anyone wants to make this config better for everyone let me know your fixes and ill include them and give you credit :)
