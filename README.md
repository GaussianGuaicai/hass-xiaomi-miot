This fork is to resolve compatibility issues when using HomeKit
- Workaround when running Homekit automation or scene to turn off thermostat, but Homekit will send command like this:
  ```HomeKit send command set_temperature to TargetHeatingCoolingState to 0, TargetTemperature to 25°C for Air Conditioner```
  but these commands will trigger it to turn off and set target temperature which is two commands, and the second command will trigger AC to turn on to set the target temperature.
