# A3 – Parametric and FEA

## Objective

The goal of this project was to decide/solve for parameters of a cylindrical bar given an applied tensile load, the change in length, and the Young's modulus of the material. Once a model of the bar was created parametrically, an FEA was used to compute the axial deflection in the bar. The values were then compared to find the percent difference between the two calculation methods.

From the professor:

1. Use axial deflection modeling to design its dimensions
2. Use parametric design to determine a bars length
3. Introduce you to FEA (Finite Element Analysis)
4. Introduce you to linking dimensions to appropriate parameters in CAD.
5. Compare and contrast the different analysis

## Analyze

<img width="736" height="452" alt="image" src="https://github.com/user-attachments/assets/a6b90bb2-d130-4245-8df6-1c066846eb7e" />

## Decide

Given the above problem statement and given values, I decided on 500 lbf for my axial load and chose a Young's Modulus of 10x10^6 psi because it is within the range for typical aluminum. For the design and dimensions of the bar I decided on a hollow cylinder/pipe because I was interested to see the affect of the reduced cross sectional area on the axial length. For the outside (OD) and inside (ID) diameters I chose .75 and .5 inches respectively. This gave the pipe a wall thickness of .125 or 1/8 in. 

## Communicate

<img width="632" height="662" alt="image" src="https://github.com/user-attachments/assets/e79405bf-630d-4184-9804-815e604f7968" />

First, I wrote down the knowns and unknowns of the problem. As previously mentioned, the max axial deflection (lowercase delta) was given: 0.009 in. The values of the axial load and Young's Modulus were selected by me. The overall length (L), ID, and OD of the bar were unknown. I started by isolating the variables in the young's modulus (stress-strain equation). Once that was done I decided to assign values for ID and OD as mentioned previously. I was then able to calculate the cross sectional area leaving me with one unknown variable left, the length of the bar. After plugging in values, I obtained a length of 44.17 inches. 

**Parametric Design**

<img width="1501" height="600" alt="Screenshot 2026-09-08 225559" src="https://github.com/user-attachments/assets/424e6d04-0892-4b85-809a-ed1a4f82969e" />

In Fusion 360, the first step to parametrically designing this beam was assigning values to parameters. This is done by selecting "modify" and then "change parameters". From here parameters could be added and modified. Note that some parameters have units and others are unitless but with a comment to the right showing the units. This was because I discovered that my version of Fusion 360 did not have units for area (in^2). The work around was creating parameters without units when possible and keeping the parameters with correct units as such when necessary. Once complete, I was able to have both the complete modulus of elasticity equation, and the ability to reference the dimension parameters crucial to the design. I will go into more detail later about this process.

<img width="475" height="392" alt="Screenshot 2026-09-08 225305" src="https://github.com/user-attachments/assets/7834d7de-9ee7-4b18-b9ed-11c308545c5e" />

<img width="443" height="410" alt="Screenshot 2026-09-08 225324" src="https://github.com/user-attachments/assets/de0b38b8-2524-4ed6-a387-238177d09097" />

<img width="397" height="385" alt="Screenshot 2026-09-08 225348" src="https://github.com/user-attachments/assets/12c768ad-6d5e-4731-9184-f9f0b668d5b0" />

<img width="396" height="385" alt="Screenshot 2026-09-08 225401" src="https://github.com/user-attachments/assets/22995cc9-6605-419a-8ea3-e58b3335d458" />

In the above photos, the base sketch for the profile of the bar was made. The parameters were typed in for the dimensions to the left, resulting in the correct dimension once entered, as seen on the right. 

<img width="962" height="642" alt="Screenshot 2026-09-08 225541" src="https://github.com/user-attachments/assets/a1480209-ca25-4167-9e47-8086a9174ce1" />

The same process as above was performed when extruding the length of the bar.

**FEA**



**Design Reflection**


