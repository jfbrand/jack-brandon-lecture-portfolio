# A2 – Truss Stress Analysis

## Objective

The goal of this assignment was to practice designing a basic truss while accounting for stress. This involved analyzing the given problem, brainstorming a solution, and doing the necessary calculations in order to produce a design that meets the design requirements. In order to solve this problem, it was necessary to use basic statics produce free body diagrams and to calculate the internal stresses at each joint and member. Mechanics of materials was used briefly to calculate the minimum cross sectional area of the members given a specific material (A500 steel in this case) and safety factor. Finally the same was done for the pins at the joints of the truss.

## Analyze

<img width="832" height="491" alt="image" src="https://github.com/user-attachments/assets/0cd30194-4622-4a71-b6c7-6847749d8705" />

The problem description is displayed above along with the design constraints. Note the asymmetrical loading, roller on the left, and pin connection to the right. The selected load was 30kN for both.

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
