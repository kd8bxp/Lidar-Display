# Lidar (Radar Like) Display

Based on the Arduino Radar Project found:  
https://howtomechatronics.com/projects/arduino-radar-project/  
By Dejan Nedelkovski (date unknown)  
This has been updated to use the TFMini Lidar sensor, which is a low cost high range lidar. The range is between 30cm to 12m (about 12 inches to 36+ feet).  
The processing sketch was modified for greater range display, and could be improved for a selectable range display.  
Because the servo library and softwareserial cause problems together, a PCA9685 PWM/Servo board was used. The library for that can be found here:  
https://github.com/adafruit/Adafruit-PWM-Servo-Driver-Library  
The Lidar is a serial device, and the Softwareserial library is used.  
A library is not needed, sections of the code are based on the work of Juan Jose Luna Espinosa 2018 for the TFMini and the ESP32  
https://github.com/yomboprime/TFMiniArduinoTest  
Under public domain.  
 This sketch was tested on the Arduino UNO.  
I used a couple of 9G servos, with a pan and tilt mount.  Tilt isn't used other than to put the sensor at 90 degrees.  
This means that only one servo is need, two are pictured.  

## Installation

There are two sketches for the Arduino, The TFMini_Lidar_30cm_to_12m_sensor_test_code.ino is just that, is sketch was written by Juan Jose Luna Espinosa (2018) see the link above.  
It will just display the reading of the lidar sensor in the serial console.  
The 2nd sketch lidar_radar_with_processing2.ino works with the processing IDE and processing sketch (lidar_processing_code) and will display a radar like sweep.  
The processing sketch is a modified version of the Arduino Radar Project Sketch. With key changes to max range of the Lidar, and changing the original display from a line to a point.  

## Things To Do

## Usage

The processing sketch will need to have line 40 or 41 changed to the serial port your Arduino is using, otherwise, there shouldn't be much more that needs to be setup.  

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## Support Me

If you find this or any of my projects useful or enjoyable please support me.  
Anything I do get goes to buy more parts and make more/better projects.  
https://www.patreon.com/kd8bxp  
https://ko-fi.com/lfmiller  
https://www.paypal.me/KD8BXP  

## Other Projects

https://www.youtube.com/channel/UCP6Vh4hfyJF288MTaRAF36w  
https://kd8bxp.blogspot.com/  


## Credits

Copyright (c) 2018 LeRoy Miller

## License

This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses>

### 1.8.9 June 2019
