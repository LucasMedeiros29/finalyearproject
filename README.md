# finalyearproject
Undergraduate capstone project for the Information Engineering program at the Federal University of ABC, by Lucas de Medeiros.

Abstract: This work presents the development and validation of a computer vision-based intelligent
traffic light system prototype, motivated by the fact that traffic lights predominantly
operate with fixed timings without considering their surroundings. The proposal involves
integrating an image acquisition system, an AI-based processing module, and a programmable
logic controller capable of dynamically adjusting the traffic light cycle in a
laboratory setting. The developed architecture comprises three main modules: the visual
system, the processing system, and the traffic light controller. The visual system, based on
the ESP32-CAM microcontroller, was configured to operate as an IP camera, continuously
transmitting images via Ethernet. The processing module—implemented in Python using
the OpenCV library and the YOLOv8 neural network—detects pedestrians in the received
images and transmits the results to the controller via the Modbus/TCP protocol. The
controller, developed using Ladder Logic on the OpenPLC platform running on an ESP32
microcontroller, interprets this information to manage the traffic light cycle; it also incorporates
supervision and camera-status monitoring mechanisms to automatically switch
to a safe mode in the case of communication failures. The obtained results demonstrated
the integrated operation of the three modules, validating image transmission, pedestrian
detection, real-time communication, and automatic controller actuation. Although the
system still exhibits limitations regarding component performance and detection model
accuracy, the experiments confirmed the proposal’s viability, highlighting that integrating
computer vision, artificial intelligence, and programmable controllers offers a promising
alternative for developing intelligent urban traffic control systems.
