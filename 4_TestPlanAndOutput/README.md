# High Level Test Plan
| Test ID  | Description | Exp I/P | Exp O/P | Actual O/P | Type of Test |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- 
| H_01  | System Testing  | LED - ON when all the doors and windows closed  | Pass  | Pass  | Requirement Based  |
| H_02  | System Testing  | Convert the analog signal from the temperature sensor to the digital value | Pass  | Pass  | Boundary Based  |
| H_03  | System Testing  | Generate the PWM signal according to the converted digital value  | Pass  | Pass  | Scenario Based  |
| H_04  | System Testing  | Send the temperature value to the serial monitor using UART protocol  | Pass  | Pass  | Boundary Based  |

# Low Level Test Plan
| Test ID  | Description | I/P | O/P | Status |
| ------------- | ------------- | ------------- | ------------- | -------------
| H_01  | If server room closed   | Push button=1  | Push button=1  | Pass  |
| H_02  | If server room opened  | Push button=0  | Push button=0  | Pass  |
| H_03  | Temperature Request  | Temp=0  | Heater=Off  | Pass  |
| H_04  | Temperature Request  | Temp=20  | Heater=20 degree generation | Pass  |
| H_05  | Temperature Request  | Temp=25  | Heater=25 degree generation  | Pass  |
| H_06  | Temperature Request  | Temp=29  | Heater=29 degree generation  | Pass  |
| H_07  | Temperature Request  | Temp=33  | Heater=33 degree generation  | Pass  |
| H_08  | LED ON | Buttons=1 && Heater=1 | LED=1  | Pass  |
| H_08  | LED OFF | Buttons=0 && Heater=0  | LED=0  | Pass  |
| H_08  | Display | Temperature :- 20 deg Cel  | Temperature :- 20 deg Cel  | Pass  |
