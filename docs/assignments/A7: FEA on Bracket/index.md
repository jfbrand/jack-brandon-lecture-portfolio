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

Before the outer loop could begin, each model had to go through the inner loop to determine the optimal mesh. This required test runs with coarse and medium meshes first to determine if they converged or not. This was determined by using the percent difference equation:

<img width="350" height="183" alt="image" src="https://github.com/user-attachments/assets/79b17576-4939-4366-8bab-26685f73a216" />

Where a and b represented values for two different simulations, each with a different mesh. The difference had to be below 7% in order for the results to converge. If the data did not converge, then the fine mesh had to be used.

## Preprocessing

<img width="1175" height="662" alt="Screenshot 2026-10-20 211301" src="https://github.com/user-attachments/assets/e601c9d2-6e0c-4042-9d7f-5d989abd27e8" />

The setup for the constraints and applied load on the model. I used frictionless constraints underneath the top beams to best simulate the sliding fit of the bracket and not over constrain the bracket, which could lead to inaccurate simulations.

<img width="1055" height="577" alt="Screenshot 2026-10-21 221833" src="https://github.com/user-attachments/assets/fc4a9c53-2680-4cff-912f-cd1bfca8d6c0" />

## Inner Loop

**Coarse Mesh**

<img width="1081" height="605" alt="Screenshot 2026-10-20 212443" src="https://github.com/user-attachments/assets/4b41e31b-972b-4237-8f47-e33ec1523312" />

<img width="1121" height="550" alt="Screenshot 2026-10-20 221843" src="https://github.com/user-attachments/assets/7be94a9d-14f8-4c8f-a360-1091c2c0facc" />

<img width="1102" height="545" alt="Screenshot 2026-10-20 221902" src="https://github.com/user-attachments/assets/50b4a36f-2825-4e7a-87d6-7441d10e9f28" />

<img width="782" height="562" alt="image" src="https://github.com/user-attachments/assets/a3ecdd05-2f79-4fd1-910a-90bc2d8ff3ca" />

<img width="780" height="561" alt="image" src="https://github.com/user-attachments/assets/5bb8f03d-a35a-4e96-b511-0e64a88a9e7e" />

<img width="792" height="555" alt="image" src="https://github.com/user-attachments/assets/0ed83f6f-3bb5-4386-a253-c37024f18f32" />

**Medium Mesh**

<img width="1133" height="552" alt="Screenshot 2026-10-20 220940" src="https://github.com/user-attachments/assets/7214f0e4-9007-4599-8115-a287bcb2f383" />

<img width="1170" height="548" alt="Screenshot 2026-10-20 221254" src="https://github.com/user-attachments/assets/53483747-9d1f-4550-9e4c-ab4b74919f47" />

<img width="1158" height="558" alt="Screenshot 2026-10-20 221322" src="https://github.com/user-attachments/assets/ef1e21d9-749e-4240-b7fd-67efe033c623" />

The displacement with the medium mesh was greater than 7% different than the course mesh. Due to there not being convergence, I moved on to the fine mesh.

<img width="790" height="567" alt="image" src="https://github.com/user-attachments/assets/3905c1cf-1b64-4d07-904b-fb562be060a1" />

The safety factor for the link with the medium mesh also failed to converge with the course mesh. This meant that it would also require the fine mesh.

<img width="797" height="572" alt="image" src="https://github.com/user-attachments/assets/545bc281-9abe-410c-85c6-e9688ef82f9d" />

<img width="775" height="555" alt="image" src="https://github.com/user-attachments/assets/b9b72438-0106-46d7-84c5-5ae406508d04" />

**Fine Mesh**

<img width="1087" height="605" alt="image" src="https://github.com/user-attachments/assets/47734cf6-883c-4987-a750-7eedefccedd0" />

<img width="1062" height="602" alt="image" src="https://github.com/user-attachments/assets/a210ef56-5c26-445e-bc1d-555160b9c186" />

<img width="1066" height="605" alt="image" src="https://github.com/user-attachments/assets/2bae5b5d-31aa-4943-a875-8ed4abf5b0f5" />

<img width="782" height="545" alt="image" src="https://github.com/user-attachments/assets/b4a9f8e7-6804-4430-88e0-1bf05587108d" />

<img width="782" height="555" alt="image" src="https://github.com/user-attachments/assets/84a5f400-4b16-4fe0-a1b0-441ea0f22a75" />

<img width="772" height="565" alt="image" src="https://github.com/user-attachments/assets/1ac989fd-3841-48a8-87dc-92f92b9dfed5" />

## Outer Loop

**Design I**

<img width="540" height="677" alt="image" src="https://github.com/user-attachments/assets/39e7d656-0578-41f3-b537-4275585bc692" />

<img width="326" height="550" alt="image" src="https://github.com/user-attachments/assets/041f8ce3-ca7c-4189-a908-a4f964e3c1a9" />

The initial designs, with dimensions calculated in A5.

**Design II**

<img width="555" height="652" alt="image" src="https://github.com/user-attachments/assets/4b61abf3-c530-4b5d-a647-308594ac8764" />

Increased the thickness of the L/R vertical beams to 0.5 in. Added another beam to simply support the cylinder. Used half the original thickness of the single beam for both.

<img width="352" height="610" alt="image" src="https://github.com/user-attachments/assets/13aab5b5-109c-4442-8833-8080854b5b3e" />

Increased the thickness to 0.3 in.

**Design III**

<img width="485" height="655" alt="image" src="https://github.com/user-attachments/assets/5048eb91-d44a-4b60-aa72-2d447d06aeb1" />

Added fillets with radius 0.5 in. to corners with the highest stress, where possible. Increased thickness of beams supporting the cylinder to 0.125 in.

**Bracket**

|          | Design I | Design II | Design III |
| -------- | -------- | -------- | -------- |
| Max Stress & Location | 234,472.509 psi - beam w/ cylinder | 34,482.717 psi - corners | 13,781.745 psi - corners |
| Max Deflection & Location  | 6.144 in - outside of L vertical beam | 4.461 in - outside of vertical beams | 4.345 in - outside of vertical beams|
| Mass | 0.889 lbm | 1.47 lbm | 1.504 lbm |
| Safety Factor | 0.128 | 0.871 | 2.178 |
| Number of Elements | 159,818 | 264,911 | 270,335 |

<img width="957" height="647" alt="image" src="https://github.com/user-attachments/assets/8d8fe8ec-b1f7-4e39-8e93-d77d46ddd58c" />

The safety factor map for design III. Although the model was almost entirely blue (above a safety factor of 4), some green was still visible around the radii, leading to the minimum safety factor of 2.178. This was unavoidable due to how fine the mesh was.

<img width="950" height="657" alt="image" src="https://github.com/user-attachments/assets/a2250685-fd80-403f-952a-46591c2b966a" />

<img width="937" height="647" alt="image" src="https://github.com/user-attachments/assets/910fbf84-1162-4412-904f-29b815d61442" />

**Link**

|          | Design I | Design II |
| -------- | -------- | -------- |
| Max Stress & Location | 15,355.26 psi - inside face of large hole | 11,294.614 psi - inside face of large hole |
| Max Deflection & Location  | 0.006 in - inside face of large hole | 0.018 in - inside face of large hole |
| Mass | 0.128 lbm | 0.173 lbm |
| Safety Factor | 1.955 | 2.658 |
| Number of Elements | 135,702 | 232,632 |

<img width="807" height="621" alt="image" src="https://github.com/user-attachments/assets/f95eb63b-616b-4daa-a50e-4dde0c09644b" />

For the link, I did not move onto design III, as it met the minimum safety factor at Design II. 

<img width="802" height="635" alt="image" src="https://github.com/user-attachments/assets/537c36d6-a9cc-45fa-baa5-e2215c6132cd" />

<img width="797" height="642" alt="image" src="https://github.com/user-attachments/assets/23829f83-311d-475d-9de3-dfc96504a6da" />



