# better speed camera

## hardware

- raspberry pi
- radar
- camera
- waterproof enclosure
- storage for system
- long usb c cable
- secure box with secure lock
- multi sd card hub with mirroring
- sd cards
- solar plate
- battery

## how it's gonna work

- radar continuously measures speed of every vehicle
- iff vehicle is above speed limit record it on camera (and read it's licence plate?)
- store these recordings along with corresponding radar measurements on all sd cards
  -- this is the evidence for police to deal with dangerous drivers
- removing and adding sd cards does not affect the program and can be done any time
- before mounting a new sd card, erase and format it, then rsync the data to it
- delete all data every 100 days
