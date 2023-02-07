# 28BYJ-48-DRV8825

To connect stepper motor 28BYJ-48 with DRV8825 stepper driver, the following need to be done:

1. Connect RST and SLP to +5v
2. STEP and DIR to microcontroller to control direction and speed via PWM pulse
3. VMOT should be above 7.5v otherwise DRV8825 undervoltage protection will shut down the driver. 8v seem to be OK.
4. Toggling STEP pin with 1ms delay between Lo and Hi will seemingly produce 60rpm. 
