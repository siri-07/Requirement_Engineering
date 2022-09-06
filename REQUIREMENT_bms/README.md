  # 40020868 Shreyashi Sonkar
 # Requirement for controller


## System Requirement:
### High level requirement:
| High Level Requirements |	Description |
| ------------------------ | ----------- |
|HL01|Controller should have the current and voltage of battery pack.|
|HL02|	Controller should achieve the temp measurement of the battery pack.|

### Low level requirement:


| Low Level Requirements |	Description |
| ------------------------ | ----------- |
|LR01|	If voltage >12v then then it will in over chargeable mode (OV).|
|LR02|	If the voltage <2.5v then it will in under discharge mode (UV).|
|LR03 |	If the temperature >90 degree then it will in over temperature mode (OT).|
|LR04	|If the temperature < -20 degree then it will in under temperature mode (UT).|


## Sub System Requirement:

## SOH Controller:

### HIGH LEVEL REQUIREMENT:
| High Level Requirements |	Description |
| ------------------------ | ----------- |
| HL01	|SOH should measure the rated capacity (Cr).|
|HL02	|SOH should measure the maximum charge available in battery.|


### Low level requirement:
| Low Level Requirements |	Description |
| ------------------------ | ----------- |
|LR01	|The rated capacity of the should be 100%.|
|LR02	|The maximum charge of the battery value should be 95mAh .(Qmax=95mAh)|

 ## SOC Controller:
### HIGH LEVEL REQUIREMENT:

| High Level Requirements |	Description |
| ------------------------ | ----------- |
|HL01	|SOC controller should measure the state of charge.|
|HL02|	SOC should measure the maximum capacity of battery (Qmax).|
|HL03	|SOC Should measure the initial charge of the battery (Q0).|
|HL04	|SOC should measure the quantity of electricity delivered or supplied by battery(Q).|


### LOW LEVEL REQUIREMENT:

| Low Level Requirements |	Description |
| ------------------------ | ----------- |
|LR01 |	The initial charge of the battery value should be 0.(Q0=0mAh)|
|LR02	|The maximum charge of the battery value should be 95mAh .(Qmax=95mAh)|
|LR03	|The quantity of the electricity delivered should be between in 0 to 100 mAh.|



# TEST PLAN:
## System Test plan:


 | Test ID | Description           | Expected I/P                                   | Expected O/P    | Actual O/P      | Status    |
 |---------|-----------------------|------------------------------------------------------|----------------------|-----------------|-----------|
 |TEST ID 01|	If voltage >12v then it will in over chargeable mode (OV).	|V>=12|Mater disconnector will disconnect.| |	
 |TEST ID 02|If the voltage <2.5v then it will in under discharge mode (UV)	|V<2.5|	Mater disconnector will disconnect.| |	
 |TEST ID 03|	If the temperature >90 degree, then it will in over temperature mode (OT).|	T>90 |degree	Mater disconnector will disconnect.| |	
 |TEST ID 04	|If the temperature < -20 degree, then it will in under temperature mode (UT).|	T<-20| degree	Mater disconnector will disconnect.| |
		
    
 

## Subsystem Test Plan:
 # SOH CONTROLLER:
 
 
 | Test ID | Description           | Expected I/P                                   | Expected O/P    | Actual O/P      | Status    |
 |---------|-----------------------|------------------------------------------------------|----------------------|-----------------|-----------|
 |TEST ID01|	The rated capacity of the should be 100%.|	rated capacity=100%	|rated capacity=100%| |
 |TEST ID02|The maximum charge of the battery value should be 95mAh.(Qmax=95mAh)|Qmax=95mAh|	Battery should be Fully charge.| |
 
 # SOC CONTROLLER:
  
 | Test ID | Description           | Expected I/P                                   | Expected O/P    | Actual O/P      | Status    |
 |---------|-----------------------|------------------------------------------------------|----------------------|-----------------|-----------|
 |TEST ID01|	The initial charge of the battery value should be 0.(Q0=0mAh)|	Q0=0	|The battery should be initially charge.| |		
 |TEST ID01	|The maximum charge of the battery value should be 95mAh.(Qmax =95mAh)	|Qmax=95mAh|	The battery should be fully charge.	| |	
 |TEST ID01	|The quantity of the electricity delivered should be between Q = 0 to 100 |mAh	Q= 0 to 100 mAh|	the battery must be charge and discharge properly.| |	



 
















