<h2 style="color: red;">
    "SMART INTEGRATED WIRE/ WIRELESS CHARGING SYSTEM FOR ELECTRIC VEHICLES WITH SOLAR AND GRID ENERGY USING IOT"
</h2>

<h2>INTRODUCTION:</h2>
<p>The government of India has launched “MISSION EV” to make all the vehicles electric as soon as possible. However, the major drawback faced by the Automobile manufacturers and government is the hurdle of battery life and setting up of charging stations. The battery range and the inability to setup charging stations at all the places is a major challenge faced by electric vehicles. Increasing in the number of travelling vehicles has increasing the problems such as air pollution and to the use of petroleum.Improved quality of life and increased mobility lead to greater consumption of energy resources and implied greenhouse gas emissions. This increased power consumption involves more quality and reliability to regulate electricity flows, less mismatching between electricity generation and demand, and more integrated renewable energies. Thus, the concept of smart grid is born in recent years. A smart grid could be easily defined as the electricity delivery system, which transports, converts and distributes the power efficiently (from producers to consumers), integrated with communications and information technology. In fact, plug-in hybrid electric vehicles (PHEVs) and electric vehicles (EVs) represent an important step in solving environmental problems and are being developed around the world.</p>

<h2>OVERVIEW:</h2>
<p>The increased power consumption involves more quality and reliability to regulate electricity flows, less mismatching between electricity generation and demand, and more integrated renewable energies. Thus, the system consists of two charging sources available one is implemented on solar energy system and another is grid based on requirement and availability it automatically swtiches. The wireless system is implemented which will charge the vehicle wirelessly and send the SMS notification to the user regarding the cost of the charge when the charging is complete. The same is displayed on LCD. The second part is Vehicle consisting of RFID reader abd wireless charge reciver. Once charging is completed total cost of charging is calculated and sent to owner using GSM modem. The IOT based application to track different locations of charging stations.</p>


# Component required with Bill of Material:

| Item                              | Quantity    | Description                            |    links of products        | 
| :---:                             | :---:       | :---:                                  | :---:                       |
| ESP32-Devkit                      | 2           | Microcontroller board                  | [ https://amzn.in/d/06Ng27mP](https://amzn.in/d/0iFXkja9) |
| Wireless Charging Module          | 1           | TO transfer energy between two objects | [https://amzn.in/d/09fDYpCs](https://amzn.in/d/0cpaSmdk)  |
| ICC LCD                           | 2           | Output display                         | [ https://amzn.in/d/0jjuc7f8](https://amzn.in/d/085QoUza)  | 
| Li-Ion Battery Charging Module    | 1           | TP4056 C Type charging module          | [https://amzn.in/d/08mS8YMR](https://amzn.in/d/0fadjajC)  | 
| Solar panel                       | 1           | renewable energy source                | [https://amzn.in/d/0iPO9ODt ](https://amzn.in/d/005uP3qb) |
| RFID Reader                       | 1           | To read RFID card                      | [https://amzn.in/d/0351O0Iw ](https://www.amazon.in/dp/B09PZ3NB4Q?ref_=cm_sw_r_cp_ud_dp_31MHW1GD4QEBWAZJZR5X_2) |
| RFID Card                         | 1           | Wireless communication                 | [ https://amzn.in/d/06Ng27mP](https://amzn.in/d/0jb8S7oR) |
| Relay Board                       | 1           | Electrically operating switch          | [ https://amzn.in/d/09fDYpCs](https://amzn.in/d/06BRSXYJ)  |
| Adapter                           | 2           | Constant power supply                  | [ https://amzn.in/d/0jjuc7f8 ](https://www.amazon.in/dp/B0B5V42269?ref_=cm_sw_r_cp_ud_dp_80HH41CQJPGXA3W94H92) | 

#  Car Part Pin connection:

| Components                        |                           |                                      |                             
| :---:                             | :---:                     | :---:                                |
| ESP32                             | Pin16                     | se                                   | 
|                                   | Pin17                     | sc                                   | 
|                                   | Pin19                     | sd                                   |
|                                   | Pin21                     | pb2                                  | 
|                                   | Pin22                     | pb                                   | 
|                                   | Pin30:GND                 | GND                                  | 
|                                   | GPIO Pins (Digital I/O )  | Sensor,led,motor drive               | 
|                                   | Pin15:VIN                 | PW in                                |
| DEO1A-G Battery Protection IC(U2) | Pin 5:VID                 | Power Supply                         | 
|                                   | Pin 3,6 :GND              | GND                                  | 
|                                   | Pin 1                     | OC(over current)                     |
|                                   | Pin 2                     | CS(current sensing)                  | 
|                                   | Pin 4                     | TD(time delay)                       |
| Relay (J2)                        | Pin 13:GND                | GND                                  | 
|                                   | Pin 14:VCC                | Power Supply                         | 
|                                   | Pin 15:SIG                | Signal from ESP-32                   | 
|                                   | Pin 3:NC                  |                                      | 
|                                   | Pin 5:NO                  |                                      |

# EV Charging Station Pin Connection:
| Components                        |                           |                                      |                             
| :---:                             | :---:                     | :---:                                |
| ESP32 Devkit V1 (U1)              | Pin : GND                 | GND                                  | 
|                                   | Pin 21:VC                 | 5V power supply                      | 
|                                   | Pin 22:(D23)              | SD                                   |
|                                   | Pin 22:(D22)              | SC                                   | 
|                                   | Pin 23:(RXD)              | RX1 through DIP switch               | 
|                                   | Pin 24:(TXD)              | TX1 through DIP switch               | 
|                                   | Pin 25:(D21)              | Csig                                 |
|                                   | Pin 26:(D19)              | RX                                   |
|                                   | Pin 27:(D18)              | TX                                   | 
| GSM Module (GSM1)                 | Pin 1                     | Antenna                              | 
|                                   | Pin 2                     | 3.7V power input                     |
|                                   | Pin 6:(GND)               | GND                                  |
|                                   | Pin 3:(Rst)               | Reset                                |
|                                   | Pin 4:(RX1)               | To RX1 via R3(10kohm)                | 
|                                   | Pin 5:(TX1)               | To tX1 via R2(20kohm)                |
|                                   | Pin 1: VCC                | 5V power supply                      | 
| LCS Display(LCD1)                 | Pin 2:(GND)               | GND                                  |

# Pinout diagram
![WhatsApp Image 2024-07-04 at 5 57 59 PM](https://github.com/jaine-bharati/wirless-charging-system-project/assets/171180747/fea8ab8c-b55d-4f03-9d84-259d996d9fad)

![WhatsApp Image 2024-07-04 at 5 57 59 PM (1)](https://github.com/jaine-bharati/wirless-charging-system-project/assets/171180747/06758090-8704-48bf-a9a8-3eb2ffc3f9e8)

![WhatsApp Image 2024-07-04 at 5 58 17 PM](https://github.com/jaine-bharati/wirless-charging-system-project/assets/171180747/d0fbb2bf-36bc-4c24-86f0-5a208a27930d)

![WhatsApp Image 2024-07-04 at 5 58 18 PM](https://github.com/jaine-bharati/wirless-charging-system-project/assets/171180747/28914f19-a899-413d-8c34-a39567c50e4b)


# Demo Video:
https://github.com/jaine-bharati/wirless-charging-system-project/assets/171180747/b0a560fc-ba2f-4bb8-9b66-1cd2f2b08ef7

<h2>Conclusion:</h2>
<p>The project deals with the concept of smart integrated wireless charging and tracking system for elective vehicles using solar energy and IOT. From the project we can conclude that the proposed project can be useful to automatically switch over to the solar energy for the purpose of the charging. We can further conclude that the developed system can easily be scaled to the actual charging stations. The system will perform wireless charging of the electric vehicles and notify the owners the charge regarding the same. The proposed project can also help the users of the electric vehicles to track the location of charging stations nearby making it easier to find out the charging stations. The App is developed which will help the users of the electric vehicles to track the status of charging and the charge using IOT.</p>
