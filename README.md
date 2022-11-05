# python-uni-t-ut353-bt
Read noise/sound levels measured by the UNI-T UT353 BT device via python

This is a simple, quick and dirty, python script that reads the UNI-T UT353 BT
sound meter via bluetooth low energy and sends the values to an OpenTSDB database.

If you want to make it nice (i.e. by refactoring it into a library), please make a pull request !

# HomeAssistant integration

HomeAssistant MQTT device discovery is supported, the device should automatically appears in your MTQQ devices.

HomeAssistant do not support yet "sound level" device, the icon will show a Wifi kind of signal.

Launch with 
```
pip3 install paho-mqtt
DEVICE_MAC=E8:D0:3C:51:D9:01 MQTT_BROKER=127.0.0.1 python3 read.py
```
