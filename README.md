# 4028 High Flow Duct for EVA toolhead

This is a modified duct for the EVA 4028 Fan Duct.
It optimizes the fan flow to achieve higher flow at the exit point at the nozzle.

This is comparison between the current EVA 4028 duct design and the new modified duct.
In the tests I redirect the flow of one of the horns of the nozzle duct, so as to only measure the flow from one side.

**Duct A** - The current design shows a range flow velocity range between 3.4 to 3.9 m/s.   
**Duct B** - The new design shows a range or flow velocity between 4.2 to sometims up to 4.8 m/s at some spots.

I am aware that the flow measurement is not consistent and varies since I'm not holding the anemometer in exactly the same spot every time.     
Chaging the average flow speed from 3.65 m/s to 4.5 m/s would certanly benefit some users.
If nothing else, you can run the fan at a lowe rpm and hence lower noise.   

https://github.com/0ut5ider/EVA_4028_High_Flow_Duct/assets/88666133/834bde17-1405-4503-b53a-58a323b9f26b

## Visual comparison of the differences

This is the duct you're familiar with from the EVA project
https://main.eva-3d.page/heat_insert/cooling_inlet/40mm/

![image](https://github.com/0ut5ider/EVA_4028_High_Flow_Duct/assets/88666133/cf9946fe-da1c-4520-a527-a8cef17b9a9a)

The modifications are the addition of a central piece behind the 4028 fan (and a few air splitters which also hold the central part in place). 

![image](https://github.com/0ut5ider/EVA_4028_High_Flow_Duct/assets/88666133/8c99bcb2-5731-486d-a148-b0581aac280b)

For the purposes of the testing I printed a Two-Horn nozzle duct as well as part of the EVA back piece which connects the fan duct to the nozzle duct.

https://github.com/0ut5ider/EVA_4028_High_Flow_Duct/assets/88666133/c6780624-e585-49d4-9ce4-8a394958fdb8

## Theory

The effective fan cross section area is area over which the blades move the air. For the 4028 fan this area is 681 mm^2.   
This comes from the full fan area created by duct the inner diameter of 38mm (which equals 1134mm^2), and from that we subtract the inner hub area created by the 24mm inner hub (which equals 452 mm^2)   
After the airflow is passes thgrough the fan, it expands in the large volume behind the fan. This causes a lot of turbulance back there since expansion happens suddenly. 
When the area increases, the pressure increases and more importantly flow velocity decreases ([Bernoulli's principle at work](https://en.wikipedia.org/wiki/Bernoulli%27s_principle) ). At the exit of the fan duct, the area restricts to 543 mm^2 (the two rectangular openings combined) so the pressure drops and velocity increases again. All these changes in pressure and velocity in one duct adds up to significant inefficiencies. 

The duct mod tries to reduce the amount of pressure and velocity changes throughout the duct. This results in better airflow.   
In order to good laminar flow, we must retain the fan area (681 mm^2) throughout the duct. That is where this internal piece comes into effect. It maintains the airflow area to roughtly 700 mm^2 cross sectional area.   
This increased laminar flow (with less turbulance) results in better flow at the nozzle.

## CAD

The STP file is available in the github repo.
This duct is a mod to the Heat Insert version of the EVA duct.

## Future Work

This is the first stab at improving the airflow through the duct. There may be further optimizations taht can be made to the design. 
- 
