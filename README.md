# Modbus_Comunnication_via_tcp_server

ROS Driver for Modbus to communicate between PLCs or Pis as modbus client server from a modbus master server  

# What is [Modbus](https://en.wikipedia.org/wiki/Modbus)

![687474703a2f2f7777772e636f6e74726f6c73797374656d776f726b732e636f6d2f692f46656174757265732f4d6f646275732e6a7067](https://user-images.githubusercontent.com/65698541/177214230-68b467df-2686-4163-9c25-73ae6d04ac7e.jpg)

> Modbus is a serial communications protocol originally published by Modicon (now Schneider Electric) in 1979
for use with its programmable logic controllers (PLCs). Modbus enables communication among many devices connected
to the same network, for example a system that measures temperature and humidity and communicates the results to
a computer. In simple terms, it is a method used for transmitting information over serial lines between electronic
devices. The device requesting the information is called the Modbus Master and the devices supplying information
are Modbus Slaves. In a standard Modbus network, there is one Master and up to 247 Slaves, each with a unique Slave
Address from 1 to 247. The Master can also write information to the Slaves.

## Prerequisites:

- Ubuntu [20.04/18.04/16.04](https://releases.ubuntu.com/) system 
- Ros [kinetic/Noetic](http://wiki.ros.org/ROS/Installation)
- joystick (for sending message as a modbus client)
- Windows system with [Siemens TIA PORTAL v13](https://support.industry.siemens.com/cs/document/78793685/simatic-step-7-(tia-portal)-v13-trial-download?dti=0&lc=de-WW)(for communicating with PLCs)

## How it Works?

- [ ] joystick setup ([joy_ros](http://wiki.ros.org/joy/Tutorials/ConfiguringALinuxJoystick))
- [ ] build [teleop_twist_joy node](https://github.com/Mdmorshadurrahman/Modbus_tcp/tree/main/teleop_twist_joy) to convert `joy (sensor_msgs/Joy)` from joytick to `cmd_vel (geometry_msgs/Twist)` to modbus
- [ ] 1. to communicate between Ubuntu and/or Pis [click here](https://github.com/Mdmorshadurrahman/Modbus_tcp/tree/main/modbus/modbus)
      2. to communicate between Ubuntu/Pi and PLCs [click here](https://github.com/Mdmorshadurrahman/Modbus_tcp/tree/main/modbus/modbus_plc_siemens) 


