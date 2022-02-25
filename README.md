# joystick-features
MIDI-Joystick via Wekinator 
Max MSP Joystick feature extractor README file

This feature extractor is going to get three continuous controller values from an device like a joystick, gamepad etc.

-You can change the device via the menu in Max MSP

-You may have to change the "route" numbers according to the device

-you may add further features of any gaming-device

This extractor works with the Wekinator software via OSC-Messages.

The max-patch sends three features via OSC to Wekinator (left) and receives them after the training in the neural network to generate some MIDI-Notes, whenever you move your joystick (based on the training). 

The Sounds move between two octaves in pitch, between 1 and 127 in velocity/gain. Also the decay of each note can differ while moving the stick, which results in layering of some notes over each other. I will try to match the notes with different scales in further versions and integrate some more buttons.

You can download the project at https://github.com/jantorge/joystick-features.git
