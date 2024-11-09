# ff_ad5m_klipper_config  
## Useful shell commands  
  
ps -ef | grep KlipperScreen | grep -v grep | awk '{print $1}' | xargs kill -15  
/etc/init.d/S80klipperscreen start  

## Useful gcode commands
### Calibrating PID
PID_CALIBRATE HEATER=heater_bed TARGET=60    
PID_CALIBRATE HEATER=extruder TARGET=255  
SAVE_CONFIG  

### extruder PID
HEATER=extruder TARGET=230 PID parameters: pid_Kp=32.996 pid_Ki=4.400 pid_Kd=61.868  
HEATER=extruder TARGET=240 PID parameters: pid_Kp=32.676 pid_Ki=4.357 pid_Kd=61.267  
HEATER=extruder TARGET=250 PID parameters: pid_Kp=32.517 pid_Ki=4.251 pid_Kd=62.189  
HEATER=extruder TARGET=260 PID parameters: pid_Kp=32.421 pid_Ki=4.238 pid_Kd=62.005  
Approx: pid_Kp=32.65 pid_Ki=4.31 pid_Kd=61.83



### heater_bed PID
HEATER=heater_bed TARGET=60 PID parameters: pid_Kp=73.354 pid_Ki=1.167 pid_Kd=1152.577
HEATER=heater_bed TARGET=60 PID parameters: pid_Kp=73.882 pid_Ki=1.310 pid_Kd=1041.734
HEATER=heater_bed TARGET=70 PID parameters: pid_Kp=73.598 pid_Ki=1.598 pid_Kd=847.297
HEATER=heater_bed TARGET=70 PID parameters: pid_Kp=74.843 pid_Ki=1.647 pid_Kd=850.402
Appox: pid_Kp=73.92 pid_Ki=1.43 pid_Kd=973.00


