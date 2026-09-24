# A5 – Bracket Design

## Objective

The goal of this project was to design a component by assigning dimensions to features using equations for stress and stiffness.

## Analyze

<img width="817" height="380" alt="image" src="https://github.com/user-attachments/assets/f12ca92d-dd45-4d17-9373-d0cf8f2d3521" />

<img width="480" height="450" alt="image" src="https://github.com/user-attachments/assets/e11108d0-7f21-47cd-b65b-d7a3dc14227a" />

## Calculating Dimensions

**Designing for Stress**

<img width="482" height="702" alt="image" src="https://github.com/user-attachments/assets/13053609-e6d0-457c-bfa2-6776e9ecc10c" />

First, an intial sketch was drawn of the different features and the dimensions of the T bar. For each feature, the knowns and unknowns were listed, as well as the assumptions.

<img width="460" height="757" alt="image" src="https://github.com/user-attachments/assets/569d135d-9877-4d3f-8a02-b345a391fbaa" />

Feature A was solved for stress first by treating it as a cantilever beam with a distributed load, the dimension being solved for was the radius (r). The result was 0.38 in.

<img width="456" height="605" alt="image" src="https://github.com/user-attachments/assets/79a482c2-9479-48f3-a859-4456854e7529" />

Similarly feature B was solved for stress by treating it as an axially loaded beam, the dimension being solved for was the thickness (t). The result was 0.15 in. 

<img width="462" height="752" alt="image" src="https://github.com/user-attachments/assets/2a8dc636-2459-42ff-98b1-8eda0cfb50b3" />

Feature C was solved for stress by treating it as a simply supported beam with a central load. The dimension being solved for was the height (d). The result was 0.68 in.

<img width="492" height="777" alt="image" src="https://github.com/user-attachments/assets/0588e6bb-a974-4a19-a260-206797a4315b" />

Feature D was also treated as an axially loaded beam. The dimension being solved for was the width (w). The result was 0.082 in.

<img width="465" height="757" alt="image" src="https://github.com/user-attachments/assets/af876546-e6d3-4330-b6e3-f3bcd9f1b781" />

Feature E was solved for stress by treating it as a cantilever beam with a distributed load. The dimension being solved for was the height (d). The result was 0.43 in. 

**Designing for Stiffness**

<img width="460" height="662" alt="image" src="https://github.com/user-attachments/assets/89fb1fa4-0f7e-4978-915f-26d84fe0e60d" />

Following the stress calculations, the same features were analyzed again for stiffness. The knowns and unknowns were written for each problem once again. The assumptions were not restated as they did not change and neither did the dimensions being solved for. The result for feature A was a radius of 0.15. 0.38 in. from the stress analysis remained the governing dimension.

<img width="462" height="670" alt="image" src="https://github.com/user-attachments/assets/856c7adc-18e0-4ba7-9791-60af9799a8f8" />

The result for feature B was a thickness of 0.014 in. 0.15 in. from the stress analysis remained the governing dimension.

<img width="470" height="697" alt="image" src="https://github.com/user-attachments/assets/46942638-d20e-4696-a186-b02529cff75e" />

The result for feature C was a height of 0.31 in. 0.68 in. from the stress analysis remained the governing dimension. 

<img width="462" height="637" alt="image" src="https://github.com/user-attachments/assets/cc5def1b-bb4f-466b-b677-447e811c38a5" />

The result for feature D was a width of 0.006 in. 0.082 in. from the stress analysis remained the governing dimension.

<img width="491" height="702" alt="image" src="https://github.com/user-attachments/assets/80c7c38b-3b84-43f3-b0fc-f2589eefc072" />

The result for feature E was a height of 0.18 in. 0.43 in. from the stress analysis remained the governing dimension.

## Drawings

<img width="1086" height="725" alt="image" src="https://github.com/user-attachments/assets/b6293c49-1a9c-4ab6-bd2a-2b015851cae4" />

<img width="1117" height="685" alt="image" src="https://github.com/user-attachments/assets/db1efb7e-b39d-485e-9df3-8024c6f46664" />

## Lessons Learned

The dimensions were fully governed by the stress analysis in this project. I was surprised that not a single dimension solved for using max deflection was larger than the one using yield strength. I assume this is because of the effect of the safety factor and the relatively large max deflection of 0.005 (5 thou). One mistake I made early on was solving for the depth of feature C instead of letting it equal a set length and then solving for the height. The first attempt lead to an extremely thin overall geometry that I think would have not been as stable in practical use. This highlighted to me the importance of strategically choosing which variables to solve for and which ones to constrain. In the instance where the height of C mattered, it would have made sense to do it the way I did originally, but that wasn't the case here. Also, I forgot to account for the tolerances for a,b,c. Luckily, these would have very little effect, if at all on the results in my calculations, but for the modeling stage of the design process, it will be necessary to go back and double check that those dimensions will have the correct clearances. Lastly, the assumption of feature B and feature D being axially loaded cause the geometry of those features to have relatively small cross sections. In reality, due to the moments acting on those two features, the cross sectional area would have had to be larger to account for this. 

## Fits

<img width="457" height="782" alt="image" src="https://github.com/user-attachments/assets/d9ecd32d-6b1a-4bb9-9fc0-b47a359cafad" />

<img width="465" height="652" alt="image" src="https://github.com/user-attachments/assets/53820688-ceec-4de4-bf1a-38dad0225447" />

After deciding the length and width of the link, the thickness (t) could be computed. The result was 0.07 in for the stress analysis and 0.01 in for the stiffness analysis respectively. Once again, the stress analysis produced the governing dimension. 

**Fit for Feature A shaft**

For feature A, an ISO H7 hole with a g6 shaft is ideal. The tolerances are 0.76 - 0.7608".

**Fit for 1 in. Diameter Shaft**

For the 1 inch diameter shaft, an ISO H7 hole with a k6 shaft would be ideal. The tolerances are 1 - 1.0008".

Sources: 

1. https://www.simplybearings.com/pages/faq-iso-286-limits-and-fits-reference?srsltid=AU7gw4UFfB1q_tH_Fb7ubHIMuCYa8_jFdkdc9cx4ZHT7mC-9t_upf2Dx&shpxid=36617a5b-4e01-4357-be69-a3f6ce14769b
2. https://www.machiningdoctor.com/calculators/tolerances/
