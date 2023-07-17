# aircraft_icing
Product: Icing Flight Test Instrumentation System simulator
Technical Production of the master's thesis: Preliminary design of an in-flight icing condition measurement system for flight test instrumentation
Available in the Unifesp repository (https://repositorio.unifesp.br/handle/11600/65316). This content is public.

Product Objective:
The simulator is useful for testing system configurations, presenting results, implementing control algorithms, and evaluating possible integration problems discovered only in installing equipment on the aircraft. The research also delivers the specific development objectives of the SLR, increasing knowledge of variables
related to ice parameters, the list of standards and sensors, and ice instrumentation equipment,
in addition to the modularized simulator for the entire system. The simulator will help in the maturity of the system development because knowing each test’s characteristics will make it possible to test the sensor configurations necessary for purchase and integration.

 Description (Item 5.2 of Master thesis):
The simulator was developed with Matlab/Simulink in version 2021b. Next Figure shows the
main page of the simulator, which is divided into subsystems:
• Cloud
• Sensors
• Aircraft
• Data Acquisition
• Data Processing
• Dashboard

![image](https://github.com/julianomdomingos/aircraft_icing/assets/139662040/a13d0582-4023-4dfb-8702-e9933436b34a)


The Cloud subsystem generates random values for the LWC and MVD parameters. The indicated boxes must be programmed with the values of the various ranges. The Air Temperature box generates a fixed temperature value for the simulation. The aircraft provides Airspeed, AOA (Angle of Attack), and Pressure Altitude values for Data Acquisition. The Ice Accretion sensor has as its structure a fixed value of impingement ratio in millimeters per second (mm/s) that can be programmed for each simulation. This is a sensor that needs to be developed for an aircraft installation. 
Data Processing is a subsystem with a few logical boxes: Equivalent time, Ice Envelope Conditions, and Data Recorder. The Equivalent Timebox is responsible for counting the test time that the aircraft was within the Startiform clouds test envelope of Appendix C - FAR 25.

