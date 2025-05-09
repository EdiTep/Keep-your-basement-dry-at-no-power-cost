<p align="center">
  <img src="pictures/Edis-Blog-Logo.png" alt="Logo edi.teppert.com Blog" width="600"/>
</p>  

# Keep your basement dry - WITHOUT electricity costs
If you have the problem that a room in your basement is damp, this project might help you.  
Keep your basement dry - WITHOUT electricity costs with an "Digital 2-in-1 Dehumidifier" (Sichler electric dehumidifier, dehumidifier & air purifier model: LFT-200 or any other dehumidifier of your choice thas can be switched on / off via the powercord)  
=> Control the dehumidifier trough a Tasmota socket and Node-Red, Mosquitto via MQTT on a Raspberry Pi. Switching times are based on adjustable thresholds for battery charge and PV feed-in.

## Requirements:  
- Raspberrypi with Node-Red with Dashboard and Mosquitto MQTT Broker installed
- PV system with batteries: home power station E3/DC  
- RSCP2MQTT installed on the Raspi [(https://github.com/pvtom/rscp2mqtt)] to get Values from the Station  
- Tasmota socket with MQTT switched on and configured for the Mosquitto Broker  
- "Digital 2-in-1 Dehumidifier" or any other Dehumidifier which can be controlled with the Tasmota plug  

## The Dehumidifier i´m using:

<p align="center">
  <img src="pictures/Dehumidifier LFT-200.jpg" alt="Picture of the Dehumidifier" width="400"/>
</p>  

[Shop where you can buy the Dehumidifier](https://www.pearl.de/a-ZX6621-3037.shtml;jsessionid=eB8477A950441CEC8498534AE405685FD?vid=953&curr=DEM)  

## Installation
Verify that the above Requirements are met.    
Import the flow into Node-RED.  
Make corrections in the Nodes for your System:  
Activate and test the flow.  

## Usage
The flow runs automatically in the background and monitors the incoming values form the PV System.  
If the adjusted Values are reached, the Dehumidifier will start working and drying the Air. If the values are not met it will stop.  

## License
This project is licensed under the MIT License.

## Contact
For questions or improvements, feel free to open an issue on GitHub or submit a pull request.  
