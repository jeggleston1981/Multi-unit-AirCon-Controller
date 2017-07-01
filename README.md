# Multi-unit-AirCon-Controller
Control multiple Heat pump units from 1 x controller, with web access and scheduling

The initial concept of this project is contructing one central control point for a building, which controls all the ducted heatpump air conditioning units in a building.  The controller will be low cost and modular. Initially it will be very simple with heating - cooling - fan modes and will not control addition functions, such as de-ice and fault monitoring.  It will require time scheduling so that the units only run during times of operation.

It will use remote thermometers such as the Sonoff TH10 based on the esp8266 to report temperatures back to the controller, and 24vac relay outputs to control the compressor relay, reversing valve, and indoor fan.

As the thermometers will use MQTT to report temps, a RPI may be used as a local broker, and a Arduino or similar microcontroller paired with a Nextion touch screen will be the main controller.  Or possibly the controller will just be the RPI.
