---
layout: single
permalink: /specification/
title: "Specification"
toc: true
toc_sticky: true
toc_label: "On this page"
toc_icon: "cog"
---

# Introduction

The NORM ROAST protocol allows the standardized assesment of the levels of pollutants, CO<sub>2</sub> emissions and energy consumption of small to mid-size batch coffee roasting machines.

# Abbrevations

Abbrevation  | Definition
------------- | -------------
BT | Bean Temperature
FCs | First Crack start
DROP | Drop at the end of a roast
|
CF | Correction Factor
CV | Calorific Value
|
LPG  | Propane Gas
NG   | Natural Gas
Elec | Electricity
|
CO  | Carbon Monoxide
CO<sub>2</sub> | Carbon Dioxide
NO<sub>x</sub> | Nitrogen Oxides
SO<sub>2</sub> | Sulfur Dioxide
PM  | Particulate Matter


# Principle

The total energy consumption and average pollutant concentration in the exhaust air of a roasting machine are measured over a measurement cycle including the pre-heating of the machine from room temperature and 4 roast batches. 

## Consumption & CO<sub>2</sub> Emissions

From the total energy consumed and the amount of green coffee roasted, the energy used to roast one kg of beans is computed. 

From the energy consumption per energy type (LPG, NG or Elec) the total CO<sub>2</sub> emissions used to roast one kg of unroasted beans are calculated. 

The batch size and other process parameters have to be choosen to minimize the energy consumption and CO<sub>2</sub> emission per kg unroasted beans.

## Pollutants
 
The concentrations of pollutants measured in the exhaust air and are averaged over the complete test cycle. Calibrated, validated and well maintained instruments have to be applied according to the instructions of their manufacture and the relevant ISO norms.

Pollutant  | ISO NORM
---------- | -------------
CO<sub>2</sub> | ISO 12039
CO  | ISO 12039
NO<sub>x</sub> | ISO 10849
SO<sub>2</sub> | ISO 7935
PM  | ISO 9096


# Pre-Conditions

## Ambient Conditions

During the execution of the test cycle the air in the test room has to fullfill the following limits.

Parameter   | Range
----------- | -----
temperature | 20 – 30°C
pressure    | 950 – 1050 hPa

## Beans

The raw coffee beans used in the test cycle have to be washed arabica with the following properties

Property | Range
-------- | -----
moisture | 10.5 – 11.5%
bulk density | 670 – 730 g/l
screen size | 17/18 1/64"
temperature | 20 – 30°C

# Profile

The test roasts have to heat up the coffee beans such that the audible popping sound of first-crack (FCs) occurs 10:00min into the roast and the roast ends (DROP) after 12:30min at a bean temperature by 10°C higher than that at FCs.

Event | Roast Time | Bean Temperature
----- | ---------- | ----------------
FCs   | 10:00min   | t<sub>FCs</sub>
DROP  | 12:30min   | t<sub>FCs</sub> + 10°C
    

# Measurement Cycle

The full measurement cycle takes about one hour and includes the pre-heating of the machine from room temperature and 4 roast patches following the profile specified in the previous section.

The batch size has to be choosen to minimize the consumption per kg green coffee with each of the 4 roast batch to follow profile defined above. 

The duration of pre-heating, as well as the time and bean temperature at FCs and DROP has to be noted for each batch.

The energy consumption and pollutants are measured over the full cycle. The consumptions are measured per energy type (LPG, NG, Elec) separately. The consumptions during pre-heating and the 4 roast batches are noted separately. The consumptions in the period between batches are fully accounted for.

The pollutants have to be measured in the exhaust according to the corresponding norm and averaged over the full period.



# Calculation

Energy consumption and CO<sub>2</sub> emissions are reported per kg of green coffee. Thus the calculated consumption and emission values are divided by the total amount of raw coffee roasted during the measurement cycle.

Gas consumption is usually measured in volume. The following formulas are used to convert the gas volume to energy consumption in kWh and energy consumption to estimated CO<sub>2</sub> emissions.

## Energy per gas volume

Given the measured gas volume, the energy consumed calculates as

<center>
Energy (kWh) = Volume (m<sup>3</sup>) x CF x CV (kWh/m<sup>3</sup>)
</center>

with

Constant | Name | Description 
-------- | ---- | -----------
CF | Correction Factor | adjusts volume for differences in temperature and pressure per supply [3]
CV | Calorific Value | gas energy content per volume



## CO<sub>2</sub> per energy

The CO<sub>2</sub> emitted per energy consumed calculates as

<center>
CO<sub>2</sub> (g) = Energy (kWh) * C (g/kWh)
</center>

with the factor C as

Type | C | Reference
----- | ---- | ----
Propane | 214.56 g/kWh | [1]
NG |      180.54 g/kWh | [1]
Elec |    500 g/kWh = 1000 g/kWh * 50% | (*)

(*) :  the CO2 emissions for electric energy depends on the clean electric energy mix. For the U.S. energy generation in 2020 we have C = 1011.51 g/kWh [2]. To get comparable numbers we take C = 1000 g/kWh and assume a clean electric energie mix of 50%.



# Report

The test cycle has to be fully documented by filling the following form.

<center>
[NORM ROAST Consumption & Emissions Form](../assets/docs/norm-roast-form.pdf)
</center>

Additionally, supporting measuring protocols, like roast, emissions and consumption logs should be provided.


# References

[1] [Carbon Dioxide Emissions Coefficients](https://www.eia.gov/environment/emissions/co2_vol_mass.php), U.S. Energy Information Administration, Nov. 18, 2021  
[2] [How much carbon dioxide is produced per kilowatthour of U.S. electricity generation?](https://www.eia.gov/tools/faqs/faq.php?id=74&t=11), U.S. Energy Information Administration, referencing data from 2020