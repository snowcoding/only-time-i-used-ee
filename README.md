# The only time EE came in handy

So today the power went out _while_ I was on an interview! Good thing I had a battery back up (EC650LCD reco by Avi). It gave me enough time to plan to get on to an alternate network and continue. The battery back up did eventually die, but it provided critical time frame: ~ 15 mins.

Out of curiosity I tried to calculate how long the router would last off of a fully charged battery. This is the first time I've ever used any of my knowledge from my EE degree IRL. So sad [said in trump's voice]

Given:
- Battery Power (in watts) = Power <sub>batt</sub> = P <sub>batt</sub> = 390 W
- Battery AC voltage (in volts) = Voltage <sub>batt</sub> = V <sub>batt</sub> = 120 V<sub>AC</sub>
- Router AC voltage ( in volts) = Voltage <sub>router</sub> = V <sub>router</sub> = 115 V<sub>AC</sub>
- Router AC current (in amps) = Current <sub>router</sub> =  I <sub>router</sub>= 1 A<sub>AC</sub>

On to the math:

### Step 1: Get Battery's Energy
Energy is power (watts) over time (hrs). So energy will be in terms of Watt-hrs. This couldn't be easier than 
- Energy in Watt-hrs = Power * time => Watts * hours, therefore:
- Energy <sub>batt</sub> = P <sub>batt</sub> * 1 unit time => 390 W * 1hr = 390 watt-hrs


### Step 2: Convert Energy to Amp-hours

The final formula is in Amp-hours so to convert we'll use this:
- Amp-hr = Watt-hr/Voltage =>
- Energy <sub>batt-A-h</sub> = Energy <sub>batt-W-h</sub> / V <sub>batt</sub> =>
- 390 W-h / 120 V <sub>AC</sub> => 3.25 A-h

### Step 3: Calculate the router's Power:
- Power (Watts) = Voltage (Volts) * Current (Amps)
- Power <sub>router</sub> = P <sub>router</sub> = V <sub>router</sub> * I <sub>router</sub>
- P <sub>router</sub> = 115 V<sub>AC</sub> * 1 A<sub>AC</sub> = 115 Watts

### Step 4: Calculate the discharge time of the battery:
- Discharge Time (hrs) = 10 * (Energy <sub>batt-A-h</sub>) / Power <sub>router</sub>
- Discharge Time = 10 * (3.25) / 115 = .263 hrs or 15.7 minutes!!!

This is ideal. So in actuality it will be less due to heat loss and stuff!
