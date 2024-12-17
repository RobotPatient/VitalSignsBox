# VitalSignsBox

This repo provides basic implementations for the VitalSignsBox modules.

### ECGLeadDetection
- BasicFirmware

Only the basic implementation, recommended to become familiair with the board and basic code.

- FirmwareECGLeadDetect

Reads the three sensors that detect the LL/LA/RA ECG leads (10-bit resolution for each sensor). It puts their values as two bytes per sensor in an I2C buffer. The client/master can read six bytes at a time.


### Temperature Sensors

- BasicImplementation_TempSensors

Allows a SensorHub to read both channels CH1+ and CH2+ of the MCP3426 sensors.
They share the same address so it uses both A and B i2c ports.
