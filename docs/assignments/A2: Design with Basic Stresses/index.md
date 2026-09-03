# A2 – Truss Stress Analysis

## Objective

The goal of this assignment was to practice designing a basic truss while accounting for stress. This involved analyzing the given problem, brainstorming a solution, and doing the necessary calculations in order to produce a design that meets the design requirements. In order to solve this problem, it was necessary to use basic statics produce free body diagrams and to calculate the internal stresses at each joint and member. Mechanics of materials was used briefly to calculate the minimum cross sectional area of the members given a specific material (A500 steel in this case) and safety factor. Finally the same was done for the pins at the joints of the truss.

## Analyze

<img width="832" height="491" alt="image" src="https://github.com/user-attachments/assets/0cd30194-4622-4a71-b6c7-6847749d8705" />

The problem description is displayed above along with the design constraints. Note the asymmetrical loading, roller on the left, and pin connection to the right. The selected load was 30kN.

## Decide

<img width="721" height="492" alt="image" src="https://github.com/user-attachments/assets/1165494a-fb8b-4a52-9ac1-0476aca7c10f" />

The selected geometry is shown above. This was the simplest and lightest design that I could come up with while still providing structural integrity. The traditional triangular truss design was selected for its desirable strength and rigidity characteristics. This is important in a problem with asymmetrical loading such at this. It has a total of 7 members and 5 pins. 

## Communicate

<img width="660" height="450" alt="image" src="https://github.com/user-attachments/assets/2eb37770-9493-451b-aa26-515dc4ea6364" />

The first step was to draw a free body diagram for each joint. Note that the direction of each force was assumed here and subject to change during the calculations of the internal forces.

<img width="476" height="712" alt="image" src="https://github.com/user-attachments/assets/cfaa827f-f6b6-4d6c-874b-49a5f6b77897" />

<img width="305" height="102" alt="image" src="https://github.com/user-attachments/assets/6c61665d-b31d-431c-9393-fa0f49254b00" />

Next, the lengths of the members were calculated using the Pythagorean theorem. Then, the sum of the moments were taken at A and B respectively. This allowed for the reaction forces at A and B to also be solved.

<img width="550" height="661" alt="image" src="https://github.com/user-attachments/assets/6055098e-a467-49e3-a4d4-b3659fcffa20" />

<img width="520" height="172" alt="image" src="https://github.com/user-attachments/assets/69d1ff56-ced8-4d28-886a-f33496b37b6b" />

Once the reaction forces were solved at A and B, the method of joints could be used to solve for the internal forces. I started with B since it had only 2 unknowns.

<img width="271" height="227" alt="image" src="https://github.com/user-attachments/assets/8001c373-053e-4367-b71f-52495b84127d" />

The above table showed the the force (kN) for each member and whether it was in tension or compression.

<img width="461" height="285" alt="image" src="https://github.com/user-attachments/assets/7efc9c40-3643-44e3-bbf7-6be0fa1e7030" />

Next, the minimum cross section had to be calculated using the given information above. The yield strength for A500 steel is a conservative value for a square rectangular section. Given a safety factor of 3.5, the minimum cross section was determined to be 312 mm^2.

<img width="537" height="92" alt="image" src="https://github.com/user-attachments/assets/b25d5ba0-0c78-4c8f-b184-19862b96c67d" />

The mass of the truss (without pins) was then predicted by finding the total volume of the members and multiplying by the density of A500 steel. The predicted mass was 8.13 kg (79.75 N).

<img width="552" height="562" alt="image" src="https://github.com/user-attachments/assets/723f41d1-3c64-4460-98c9-30c7239841b4" />

Lastly, the same was done for the pins. The minimum cross sectional area was calculated to be 81.90 mm^2 given a safety factor of 4. To determine the volume of each pin, the length was estimated to be 35.32 mm which is the width of exactly 2 square trusses together. This is not accurate to the actual design which would actually have one joint with 4 overlapping members and two joints with three overlapping members. Also, the thickness of each member was later changed from the 17.66 mm used here. However, given the instructions to calculate for a single shear and the relative low mass of the pins, this estimate was deemed "good enough". The predicted mass per pin was 22.26 g and the total was 111.3 g.

<img width="908" height="560" alt="Screenshot 2026-09-02 214748" src="https://github.com/user-attachments/assets/335fb691-ba01-453c-80cd-8a71141a16f6" />





