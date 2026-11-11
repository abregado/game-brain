---
title: "Stardrive-Universe Generation"
source: "Game Stuff/Game Ideas/Stardrive-Universe Generation"
modified: 2013-06-12
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Stardrive]]"]
concepts: ["Stardrive", "Design: Procedural Galaxy Generation"]
words: 856
summary: "Spec for procedural galaxy generation: input parameters, ring/arm mass allocation formulas, star creation, lifetime and stellar phase calculations, and discussion of spiral twisting and stellar populations."
tags: ["area/game-idea", "project/stardrive", "type/design-doc"]
---

Universe Generation and Exploration



In the beginning, an algorithm should be used to generate the placement of stars in the galaxy. A vast majority of stars generated should be either new stars, or have no planets. Stars closer to the galactic centre should be older (Population I) stars.

Larger stars move through their phases a lot faster.

Outer rings have less mass assigned to them and the stars there would be of higher Population (II and III mainly).

Input Screen

Galactic Mass – measured in 1000s of solar masses

Age of galaxy – Measured in billions of years

Smallest Orbit – measured in light years

Maximum Orbit - measured in light years

Number of rings – integer input

Number of arms – integer input

Width of arms – measured in light years

Create Galaxy

1.  Select total Mass (Number Input, Solar masses)

2.  Select Galactic Radius (Number input, Light years)

3.  Select Galaxy Age (Number input, billions of years)

4.  Allocate Mass to Rings

    1.  Determine smallest orbit size (number input)

    2.  Determine number of rings (Number input)

    3.  Distribute Mass (60% of remaining mass in each ring)

5.  Select number of Arms (number input)

6.  Select width of arms (Number input, light years)

7.  Allocate Mass to Arms (even distribution between arms.)

Create Star

1.  Select Ring

2.  Select Arm

3.  Randomly determine distance from centre (orbit)

4.  Determine sun mass (randomly, deduct from total mass)

5.  Determine birth date (randomly)

6.  Randomly determine distance from arm

7.  Calculate actual position (relative to arm)

Calculations

((Max Orbit-Min Orbit)/#ofRings) = Amount of base orbit to add per ring (RingWidth)

Declare ring variables (Ring Number, Mass Remaining, First Orbit)

Ring 1 gets 60% of total mass and the “minimum orbit” value

Ring 2 gets 60% of remaining mass and Ringwidth-Min Orbit

Ring 3 gets 60% of remaining mass and 2\*Ringwidth-Min Orbit

Final Ring gets remaining mass and Ring#\*Ringwidth-Min Orbit

Declare Arm variables (Arm Number, Mass Remaining, Arm angle)

360/#ofArms = Angle

TotalMass/#ofarms = Mass

Arm# \* Angle = Arms Angle

Arm# \* Mass = Arms Mass

MaxDist = ArmWidth/2

Place a star

Select Ring and Arm: This is not random. Should be done one Ring at a time

Randomise distance from centre of galaxy:

Random number between First Orbit and FirstOrbit+RingWidth

Randomise distance from arm:

Random number from –Maxdist to Maxdist

Create star entry

Give star co-ordinates

Give star Mass: Mass = Random (0.1 – 120)

Luminosity = Mass^3.5

Time before Birth = 0.1-2 bil years = TBB

Protostar = 0.1-0.3 bil years = PSL

Main sequence lifetime = (1/Mass)^2.5x10 (billions of years) = MSL

If Galaxy Age is less than TBB + PSL + MSL then star is on the main sequence

If Galaxy Age is less than TBB + PSL then star is a protostar

If Galaxy Age is less than TBB then star is a nebula

If Galaxy Age is greater than TBB + PSL + MSL then:

Time Till Present (TTP) = Galaxy Age – (TBB+PSL+MSL)

If Mass is greater than 8 then Supergiant

If Mass is less than or equal to 8 then Red Giant

Discussion (feel free to add stuff)

Arms are “twisted” into a spiral. When the systems are being displayed their position takes this into account. This should allow for “on the fly” aging.

If the “distance from arm” calculation is written so that stars are placed in a normal distribution, then the galaxy will take on a spiral look when it is twisted. The area between arms will still be populated with stars however these areas will be visibly less dense.

Maximum and minimum star size should be a function of the total mass of the ring in which the star is found. Since the outer rings have less mass in total, the stars in these rings should be smaller from the outset, and thus will burn for longer before becoming stars of higher population. Im unsure exactly what the relationship should be in order to achieve the desired effects which are:

*Inner Ring stars will be mostly Population I stars, the oldest generation of stars. The Middle Ring stars should be comprised of a combination of Population I and II, Pop I being the dominant group. Outer ring stars should mainly be Pop II stars with only very few Pop I stars. Pop III stars should be completely extinct by the start of the game.*

To achieve the desired effect cosmetically, orbit distance from the galactic centre will have to be factored into the equations so that the mix of Pop I and II stars is gradual (The percentage of higher population stars will increase towards the outside of the ring).

The **Stefan–Boltzmann law** also known as **Stefan's law**, states that the total [*energy*](http://en.wikipedia.org/wiki/Energy) radiated per unit surface [*area*](http://en.wikipedia.org/wiki/Area) of a [*black body*](http://body) in unit [*time*](http://en.wikipedia.org/wiki/Time) (known variously as the black-body [***irradiance***](http://en.wikipedia.org/wiki/Irradiance), **energy flux density**, **radiant flux**, or the **emissive power**), *j*^(\*), is directly *proportional* to the fourth power of the black body's [*thermodynamic temperature*](http://temperature) *T* (also called **absolute temperature**):

Mainsequence – giant star = 30-40% mass loss

Speed of nebulae after supernova = 10% of c
