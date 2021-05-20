## I'm feralcoder!
f********r@g***l.com

## Interests
Any form of mechanical or material hackery:  Wood, auto, textiles, agricultural...

In IT, everything between the wall outlet and user.
Sysops, netops, SRE are all in my professional toolbox.
More recent proficiencies in API, frontend, and GUI development.
Some work in electronics: power supply, microcrontrollers for sensing and control apps...


## Learning
Remediating my system skills by diving into BPF and performance / tracing tools (a la B Gregg).
Hardening my Python chops with guided exercises and readings (Fluent Python - L Ramalho; Hitchiker's Guide to Python - Reitz & Schlusser).
Self-guided projects deploying and using data stores (Cassandra, MariaDB Column Store, HBase).
OpenStack - Fully HA deployment on Ceph, with Octavia load balancing, Magnum container orchestrator, many more bells and whistles.


## Collaborate?
I have 2 open-ended projects which might be of interest to others, and which definitely have need for more brains:

Agricultural automation.  The ag world needs a major technology refresh.  Wealthy areas are still using very expensive hardware
and underdeploying sensors and control hardware.  These devices are often networked over outdated RS-485 protocol, with max 32 devices
in many cases.  Poor areas aren't deploying basic technologies that would allow a leap in control, quality, and resource conservation.
Sensing devices which could be implemented on Arduino with cheap components are instead still being sold as expensive industrial
devices.  At 1/50 the price, one could afford to deploy a sea of unreliable devices, increasing coverage, granularity, and reliability.

Playlister.  Remember iTunes?  That was the last useful playlist / device manager.  It supported more ratings than just "love".  It had smart playlists.  
My goal is to build a collection manager which manages metadata and allows smart playlist generation based on metadata or text matching.
Of course static playlists would be also supported.  Trees of lists and conditionals could be composed for generating well-tuned dynamic lists.
Initial version in development is limited to local music, and manages syncing of songs to playback device / storage, alongside xspf playlist files.
Future versions could manage multiple sources, multiple destination devices, 3rd party collection integration, non-xspf device lists,
transcode management, etc.

    _Bonnaroo-2022-Day-1: (a dynamic list including music by all artists in Day 1 lineup)
    - Artist (OR):
        - ~= 'Aesop Rock'
        - ~= 'MGMT'
        ...

    _Bonnaroo-2022-Review: (a dynamic list to help me discover everything on offer at the festival)
    - Song in list (OR):
        - _Bonnaroo-2022-Day-1
        - _Bonnaroo-2022-Day-2
        - _Bonnaroo-2022-Day-3
    - AND Rating == None
    - AND Not in list (OR):
        - Bonnaroo-2022-Selected
        - Bonnaroo-2022-Ignore

    Bonnaroo-2022-Ignore: (a static list collecting songs I'm no longer interested in seeing in my other lists)
    
    _Bonnaroo-2022-Share: (a dynamic list to surface good or noteworthy music)
        - Song in lists (OR):
            - _Bonnaroo-2022-Day-1
            - _Bonnaroo-2022-Day-2
            - _Bonnaroo-2022-Day-3
        - AND
            - Song in list:
                - Bonnaroo-2022-Selected
            - OR Rating >= 4
