
# micropython-driver


This is a collection of MicroPython drivers for various sensors and devices. Each driver is designed to be simple to use and compatible with MicroPython's I2C and SPI interfaces.

## The collection from following code repositories:


### sensors 

#### BMP280 

[dafvid/micropython-bmp280](https://github.com/dafvid/micropython-bmp280)

#### SSD1306

[TimHanewich/MicroPython-SSD1306](https://github.com/TimHanewich/MicroPython-SSD1306)


### I2S 

https://github.com/maspetsberger/esp32-i2s-mems/blob/master/examples/NoiseLevel/NoiseLevel.ino


### OV2640 

https://github.com/lemariva/micropython-camera-driver

### OV2640-SPI

https://github.com/namato/micropython-ov2640




## basic operations 

esptool --port COM6 erase_flash

esptool --port COM6 --baud 460800 write-flash 0x1000 micropython_camera_feeeb5ea3_esp32_idf4_4.bin


mpremote connect COM6 fs cp ssd1306.py :
mpremote connect COM6 fs cp bmp280.py :
mpremote connect COM6 run mp-i2c-dat.py