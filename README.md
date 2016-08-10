# UHF-digital-wireless-microphone

UHF digital wireless microphone based on the arduino DUE and cheap SI446x modules with 26mhz oscillator.

The project is using DIY shields;
2 x Audio CODEC (WM8731) Mikroe 506 Proto Boards
3 x SI446x shields ( 1 on TX shield and 2 on true diversity RX shield )

The project includes a true diversity reciever setup and will hopfuly support embeded LTC timcode TX RX.

This Code depends on;

Radio modules driver , 
RadioHead RH_rf24  http://www.airspayce.com/mikem/arduino/RadioHead/classRH__RF24.html
including Custom 200khz RF mask GFSK connfig file fir 26mhz oscilator based modules made with free WDS software

http://www.silabs.com/products/wireless/EZRadio/Pages/WirelessDevelopmentSuite.aspx

I2S SSC driver for ARduino Due  
ArduinoDueHIFI ,  https://github.com/delsauce/ArduinoDueHiFi

LTC Timcode decoding / encoding, libLTC, 
https://github.com/x42/libltc

IMA_ADPCM audio compression library , 
http://yxit.co.uk/source/documentation/classIMA__ADPCM.html

It early days, don't expect this code to work at all !!

Fo now the example code is just about working in 8 bit only sending 1 sample every 4.

I will update this readme when IMA_PCM is working shortly and post radio config file.






