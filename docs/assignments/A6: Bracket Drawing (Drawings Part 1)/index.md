# A6 – Bracket Drawing (Drawings Part 1)

## Objective

The goal of this project is to generate a CAD model and drawing of the bracket that I designed last week.

## Parametric Design

<img width="1615" height="795" alt="image" src="https://github.com/user-attachments/assets/988a7355-4f7d-46ff-a0bf-d3fb57d9eea6" />

Here was the parameters used in the model for the bracket. Every value was either provided for in the problem or calculated using the formulas (expressions). Note that the governing dimensions for this model were all obtained by designing for strength. Due to the assumptions made in that assignment, the geometry may look odd/poorly designed.

<img width="850" height="641" alt="image" src="https://github.com/user-attachments/assets/8aa19c70-3b93-4b65-85ec-182dcb6dcbdd" />

Here was the overall geometry of the bracket. Note the "fx:" before each value, showing that a parameter was being referred to in the sketch. Clearly, the sides are too thin due to the assumption that they were experiencing axial stress only.

<img width="765" height="640" alt="image" src="https://github.com/user-attachments/assets/8bf5d3ef-9292-42f1-b7fe-30060c392fa4" />

The extrusion using the depth, d, parameter.

<img width="1102" height="542" alt="image" src="https://github.com/user-attachments/assets/a139d8ae-6c04-4c3e-90dc-1c86e9376cd7" />

Using the parameters for the diameter of feature A, d_A, and the thickness of feature B, t_B, I sketched feature B.

<img width="611" height="565" alt="image" src="https://github.com/user-attachments/assets/38abb783-911c-4e35-9de8-9cf328614f41" />

Feature B was extruded to 1.5 in (not a calculated value/parameter since it was designed for strength not stiffness).

<img width="792" height="501" alt="image" src="https://github.com/user-attachments/assets/dec34bb4-34fe-48c0-928a-84bcd0ece532" />

Feature A was sketched using the parameter for the diameter of feature A, d_A.

<img width="642" height="637" alt="image" src="https://github.com/user-attachments/assets/69de361e-20f1-4d1e-9c69-fe2f6844bae8" />

Feature A was then extruded to the depth of the bracket, d.

<img width="540" height="677" alt="image" src="https://github.com/user-attachments/assets/8170b3b2-1b7c-4fd5-8d43-d46d69be7a36" />

The completed model of the bracket.

[Download the Model Here](https://a360.co/4hWGmmI)

## Drawing

<img width="1115" height="722" alt="image" src="https://github.com/user-attachments/assets/d7d61fbd-2b0e-4bf6-91ff-eca94dde752d" />

## Reflections

As mentioned earlier, all of the governing dimensions for this model were obtained by designing for strength. One example of of this was the dimension for the width of feature D. The feature was assumed to be axially loaded and so the equation to solve for the width was simply yield strength/safety factor = force/area. I then isolated the width variable and entered that equation into CAD. The result was 0.0617 in. This dimension is mathematically correct when solving for the cross sectional area of the feature while its only axially loaded. However, it is clear that in reality this feature (and a couple others in this design) would undergo bending moments as well. The Calculated width would simply be far too narrow for a 1000 lbf load on the bracket. For the purpose of this assignment, I decided to not change the dimension manually as I believed that would go against the intent.

Only one of the features, A, required a tighter tolerance due to interfacing with the link. The desired fit was a running sliding fit. The only other features that maintained tight tolerances were the internal dimensions that would interact with the T-beam. The dimensions were intentionally kept loose throughout the rest of the bracket to make it more manufacturable and because there were no other fits needing tighter tolerances.

## 2157

**Parametric Design**

<img width="1622" height="800" alt="image" src="https://github.com/user-attachments/assets/ab15186c-d951-4830-8e92-f4df0bec70a4" />

The parameters for the model of the link. Note that the length and width were chosen to accommodate the two diameters. The governing dimension for the thickness of the link was obtained by designing for strength. The diameter of the largest hole was included in the equation to account for the part of the link with the least cross sectional area.

<img width="617" height="600" alt="image" src="https://github.com/user-attachments/assets/88fd471c-774f-4d47-99bc-09a6fab5bfd3" />

The sketch of the geometry of the link. Holes were placed strategically to ensure .25 in of material between the top and bottom edges of the link and the circumference of the holes.

<img width="607" height="657" alt="image" src="https://github.com/user-attachments/assets/b5cd7429-dc11-4399-a414-22db1f3f1bcb" />

The link was extruded to the thickness, t, calculated earlier.

<img width="532" height="637" alt="image" src="https://github.com/user-attachments/assets/6ffc2c50-4c9d-47db-9197-62b57cb3f2a9" />

The edges were filleted to match the design concept.

<img width="582" height="632" alt="image" src="https://github.com/user-attachments/assets/0e0dd5aa-4746-48f5-883a-866e510fd0a6" />

The completed model of the link.

[Download the Model Here](https://a360.co/4hG3wwx)

**Drawing**

<img width="1097" height="712" alt="image" src="https://github.com/user-attachments/assets/9e039c04-21fa-41bc-80e6-5dbb55c6440e" />

**Reflections**

The important takeaway is determining the desired fit before choosing tolerances of both of the parts. This requires careful attention to both the tolerances themselves but also the direction of the deviation. For example, the deviation should be +.000x for a hole and -.000x for a shaft in order to ensure that there is no interference (unless desired).

Lastly dimensions communicate design intent by showing where manufacturers need to prioritize their accuracy/precision. If a part has an intended function that requires a tight or loose fit, manufacturers can discern this by reading the drawing and seeing the tolerances.
