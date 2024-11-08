# ff_ad5m_klipper_config  
## Useful shell commands  
  
ps -ef | grep KlipperScreen | grep -v grep | awk '{print $1}' | xargs kill -15  
/etc/init.d/S80klipperscreen start  

## Useful gcode commands
### Calibrating PID
PID_CALIBRATE HEATER=heater_bed TARGET=60    
PID_CALIBRATE HEATER=extruder TARGET=255  
SAVE_CONFIG  