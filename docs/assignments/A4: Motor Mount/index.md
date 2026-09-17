# A4 – Motor Mount

## Objective

The goal of this project was to gain experience designing a basic motor mount by calculating the minimum cross sectional area using the yield strength and maximum deflection.

## Analyze

<img width="162" height="137" alt="image" src="https://github.com/user-attachments/assets/3402c593-4ad4-4ebc-81f8-1ff172007595" />

Description from the professor: Design a motor mount using the (Brushed 24V DC Gear Motor 3.6Kg.cm/46RPM w/ 99.5:1 Planetary Gearbox) HERE which attaches to the rigid wall A. For both features, first design for yield strength and then design for a maximum deflection of .30 mm at the free end. You may select ABS, PETG,  or PLA as a motor mount material.  When designing the motor mount take into account a safety factor of 3 and neglect the weight of the motor. For steps 1 and 2 draw a FBD of the forces and a concept of your design. Research the design of different motor mounts and place the links in an appendix on your page. Make justifiable approximations in your design to simplify your analysis. (ie. use the beam calculations) Follow Appendix B for the initial approach to set up the design analysis.

P=3



## Decide

First, a material had to be chosen for the design. I decided to use high impact ABS because of its increased ductility and toughness compared to PETG and PLA. Although its yield strength is relatively lower than the other two materials, 45 MPa was not far off, and the material would hold up well to impacts, shock, and heat from the motor. 

<img width="1645" height="445" alt="image" src="https://github.com/user-attachments/assets/a42239d7-da00-4deb-8c13-d0e5e1fc1dae" />

Next, I had to decide how to solve for the cross sectional area of the 2 features. Given the thickness and width were unconstrained, one had to be chosen while the other was calculated. I decided to set the width (variable "b" in my work) because I wanted to ensure the mount was the correct size for the motor. I chose 28 mm for this dimension to account for the diameter of the motor casing. Similarly, I chose an overall length of 32 mm for each feature so that motor could fit properly without too much extra material being used.

## Feature 1

**Designed for Yield Strength**

<img width="657" height="862" alt="image" src="https://github.com/user-attachments/assets/170b32bc-ee3a-44b4-b69a-16907a8c5aa6" />

First the knowns and unknowns were listed for the problem.

Knowns: Yield strength (Sy), force (P), motor shaft length (Lshaft), and safety factor (SF).

Unknowns: Length (L), moment of inertia (I), centroidal distance (c), thickness (h), and width (b).

I then drew a free body diagram and then algebraically solved for h given a b of 28 mm (mentioned earlier in "Decide" section). The result was a thickness of 8.8 mm. Note that I made the assumption that the feature would react like a cantilever beam hence the equation used here (from the *Machinery's Handbook*).

**Designed for Maximum Deflection**

<img width="657" height="717" alt="image" src="https://github.com/user-attachments/assets/9a19a727-999d-49c9-893f-fe7ad1b44cb2" />

## Feature 2

**Designed for Yield Strength**

<img width="656" height="622" alt="image" src="https://github.com/user-attachments/assets/5eb584a9-52ea-4a78-9d9d-156899fad38f" />

**Designed for Maximum Deflection**

<img width="657" height="627" alt="image" src="https://github.com/user-attachments/assets/a85d8138-ac12-40e6-aff5-c2e972643341" />
