**--- Sensor Profiles for FPV ---**


1.  Copy file to `/etc/sensors`
  
3.  Edit `/etc/majestic.yaml`, change sensorConfig path to the new file
  
5.  Restart


**--- Commandline Installation ---**

**imx335**
```
curl -L -o /etc/sensors/imx335_greg15.bin https://github.com/sickgreg/OpenIPC-bin-files/releases/download/greg15/imx335_greg15.bin
cli -s .isp.sensorConfig /etc/sensors/imx335_greg15.bin
killall -HUP majestic
```

**imx415**
```
curl -L -o /etc/sensors/imx415_greg15.bin https://github.com/sickgreg/OpenIPC-bin-files/releases/download/greg15/imx415_greg15.bin
cli -s .isp.sensorConfig /etc/sensors/imx415_greg15.bin
killall -HUP majestic
```
