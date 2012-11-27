libHecato
=========

libHecato is an easy-to-use framework to quickly set up depth-imaging-enabled (e.g. "Kinect") multi-user 
interaction applications. It is able to process touch events, gestural movements and to track the presence of 
users. Got a big projection you've always wanted to use multi-touch? Grab a depth cam and libHecato is your 
solution.
The framework hereby expects the camera to be placed above the interaction area to minimize occlusion while 
maximizing the amount of possible simultaneous users. libHecato's key strengths lie in the following:

    Multi Aspect
Whether it's point-to-click or gestures you want to process, libHecato has a tracking component that 
robustly correlates the framewise detection to kalman-filtered tracks. Besides a defineable area for any hand 
actions it is also possible to set a space in the camera image in which persons are to be detected.
    
Scalability
The software can handle consistent tracking over a tracking space of arbitrary length. This means that 
multiple depth cameras can be inconcatenated to form larger installations. This renders it highly usable for 
big projections.

    Output / Extendability
Hecato uses the TUIO-Protocol, a for tangible user interfaces widely used protocol, for standard output.
All the classes along the processing chain - from image acquisition to output are easily extendable to 
allow for modifications in every step. See HTBlobInterpreter to modify the handling of detections or to change 
how tracks should be handled.

    Platform Independence
Using only platform-independend libraries such as opencv and OpenNI itself, libHecato is able to be 
compiled for Linux, Windows and Mac (in this order of support :) )

    Toolset
The framework includes two applications for calibrating (HTCalibration) and for operation (HTApp) which 
usually suffice for not too specific tasks. In this case, no programming experience is needed to use 
libHecato.
