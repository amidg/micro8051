# micro8051
micro8051 is the open-source implementation of the outdated Intel's architecture MCS-51 commonly known by the microcontroller 8051. 
Github contains only my last polished revision (Rev.A5). If you would like to request older versions (explained below), please, contact at dgusev@sfu.ca

Some background:
Initially I started this project around 2 years ago while taking MSE352 "Digital Logic and Microcontrollers" at Simon Fraser University, Canada. 
This project was supervised by Dr. Mohammad Narimani and Dr. Amr Marzouk. 

Main goal of the project was to reduce the cost of equipment and provide students with advanced and open-source alternative for the board designed by MikroElektronika which is costly and lacks modern functionality. 

Achieved results:
- Total cost of purchasing was reduced by half (from $90 to ~$40, even with fabrication and parts located in NA)
- Smaller breadboard-friendly form-factor
- In-built Arduino Uno R3
- 8051 can take control of the Arduino functionality (via additional UART MUX, Arduino must support SoftwareSerial @ 9600 baud)
- 8051 can communicate to the USB directly (UART<->USB)

Revision History:
- Rev.A1: FTDI232 (SMD) + Arduino Uno (DIP) + 8051 (DIP)
- Rev.A2 (breadboard only): MCP2221A (DIP) + Arduino Uno (DIP) + 8051 (DIP)
- Rev.A3: Rev.A2 + 2x MCP2221A for 8051 direct USB communication
- Rev.A4: ATmega16u2 (Hoodloader @ SMD) + ATmega2560 (extra @ SMD) + 8051 (SMD)
- Rev.A5 (current): FT231XS + MCP2221A (SMD) + ATmega328P (SMD, UART<->SPI flashing) + 8051 (SMD)

Important notes: 
When communicating to Arduino, 8051 cannot take control over Serial communication. 

Gerbers and BOMs are located in Manufacturing folder. 

Enjoy! 
