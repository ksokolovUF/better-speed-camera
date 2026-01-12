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

### radar

- high speed alert triggers saving of video footage from camera until there
  is a low range alert
- second camera captures the licence plate on the back of the car
- the speed over time graph is saved (the start and end times are exactly the same
  as on the video)
- max speed, speed limit, difference between two values, along with other helpful
  data are saved in a separate plain text file
  - vehicle length
  - vehicle position/lane?

### access box

- how to make it secure?
- how to protect against lockpicking?
- how to make it impossible to hide tracks of breaking into the box?
- if secure enough:
  - provide a port for accessing the system in order to edit and
    update software
  - ability to install extra batteries in the access box in case of solar plate failure

### problems

- cosine error by the radar
- night conditions for the camera

## alternative approach

- broadcast all data wirelessly to simplify policemen work and promote public shaming
