# A7 – FEA on Bracket

## Objective

The goal of this assignment was to modify the bracket from A5 and A6 using FEA analysis to gain understanding of how FEM can be used in the design process.

The objectives from the professor:

1. Use Finite Element Analysis (FEA) to improve the bracket design from previous assignments.
2. Ensure high stiffness, strength, and lightweight optimization through iterative design.
3. Conduct multiple FEA simulations, refining geometry based on results.
4. Perform static stress analysis, including constraints, loading, and meshing selection.
5. Interpret data by identifying max stress, displacement, and safety factors.
6. Optimize the design by modifying geometry to enhance performance.
7. Document the entire process with images, calculations, and insights.
8. Reflect on key engineering lessons learned and time spent.

## Analyze

<img width="590" height="437" alt="image" src="https://github.com/user-attachments/assets/3d1998cc-9587-4c95-92f1-314515b7d584" />

<img width="477" height="515" alt="image" src="https://github.com/user-attachments/assets/535959c7-4077-460b-b668-1a50876752d7" />

## Preprocessing

<img width="382" height="552" alt="Screenshot 2026-10-20 215202" src="https://github.com/user-attachments/assets/c2d69e52-ff51-48d8-8a94-d38d8603968f" />

<img width="1175" height="662" alt="Screenshot 2026-10-20 211301" src="https://github.com/user-attachments/assets/e601c9d2-6e0c-4042-9d7f-5d989abd27e8" />

## Inner Loop

**Coarse Mesh**

<img width="1081" height="605" alt="Screenshot 2026-10-20 212443" src="https://github.com/user-attachments/assets/4b41e31b-972b-4237-8f47-e33ec1523312" />

<img width="1121" height="550" alt="Screenshot 2026-10-20 221843" src="https://github.com/user-attachments/assets/7be94a9d-14f8-4c8f-a360-1091c2c0facc" />

<img width="1102" height="545" alt="Screenshot 2026-10-20 221902" src="https://github.com/user-attachments/assets/50b4a36f-2825-4e7a-87d6-7441d10e9f28" />

**Medium Mesh**

<img width="1133" height="552" alt="Screenshot 2026-10-20 220940" src="https://github.com/user-attachments/assets/7214f0e4-9007-4599-8115-a287bcb2f383" />

<img width="1170" height="548" alt="Screenshot 2026-10-20 221254" src="https://github.com/user-attachments/assets/53483747-9d1f-4550-9e4c-ab4b74919f47" />

<img width="1158" height="558" alt="Screenshot 2026-10-20 221322" src="https://github.com/user-attachments/assets/ef1e21d9-749e-4240-b7fd-67efe033c623" />

**Fine Mesh**

<img width="1087" height="605" alt="image" src="https://github.com/user-attachments/assets/47734cf6-883c-4987-a750-7eedefccedd0" />

<img width="1062" height="602" alt="image" src="https://github.com/user-attachments/assets/a210ef56-5c26-445e-bc1d-555160b9c186" />

<img width="1066" height="605" alt="image" src="https://github.com/user-attachments/assets/2bae5b5d-31aa-4943-a875-8ed4abf5b0f5" />

## Outer Loop

**Design II**

**Design III**

|          | Design I | Design II | Design III |
| -------- | -------- | -------- | -------- |
| Max Stress & Location | 234,472.509 psi - bottom beam |    |     |
| Max Deflection & Location  | 6.144 in - left beam |    |     |
| Mass | 0.889 lbm |    |     |
| Safety Factor |    |     |     |
| Number of Elements |    |    |    |

## Communicate

