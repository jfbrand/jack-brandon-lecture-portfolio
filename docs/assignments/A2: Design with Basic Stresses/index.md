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

Above is the CAD model of my truss design. The material used for the material properties was "steel" as Fusion does not have A500 steel in its material library. However, it is worth noting that their densities are exactly the same at 7850 kg/m^3. The predicted mass of the truss was 7.337 kg compared to my prediction of 8.13 kg. The link to download it is here: https://a360.co/3Un2BsV

<img width="370" height="447" alt="image" src="https://github.com/user-attachments/assets/1740406a-a4f6-4d40-9fc5-e5b0bc224dc0" />

The pin design. The diameter is 10.21 mm and the length is 35.32 mm.

**Lesson Learned**

The main lessons from this assignment were to take an engineering problem, produce a conceptual design, and do the calculations in order to produce a workable prototype in CAD. I found that the whole process is time consuming but highly rewarding and helped me brush up on older concepts that I may need later in my career.

# A2: Likelihood of Failure Modes in Truss Components

For this part of the assignment I decided to use Claude AI to present me with research on this topic. The prompt was simply the PDF of my work from earlier and the questions from the assignment.

**Truss:** Loading P = 30 kN at joints C and D, a = 0.4 m, b = 0.3 m, B = roller, A = pin
**Governing member force:** 24.00 kN (members CE and ED)
**Member material:** A500 steel, assumed yield strength σ_y = 269 MPa, FoS = 3.5
**Pin material:** Hardened tool steel, assumed shear yield strength τ_y = 170 ksi (1172 MPa), FoS = 4

---

## Part 1 – Truss Members

### Summary of member forces (from static analysis)

| Member | Force (kN) | Tension/Compression |
|---|---|---|
| BC | 16.67 | C |
| BE | 13.33 | T |
| CE | 24.00 | C |
| CD | 0.00 | — (zero-force member) |
| EA | 13.33 | C |
| ED | 24.00 | T |
| DA | 16.67 | T |

The cross-sectional area (A_min ≈ 312 mm²) was sized off the single largest member force (24.00 kN) using a factor of safety of 3.5. Because the same section is being used for every member (a common practical simplification so the truss can be built from one stock size), every other member runs at a lower stress and therefore carries a *higher* effective safety margin than the design FoS of 3.5:

| Member force | σ = F/A_min | Effective FoS (σ_y/σ) |
|---|---|---|
| 24.00 kN (CE, ED) | 76.9 MPa | 3.5 (design case) |
| 16.67 kN (BC, DA) | 53.4 MPa | ~5.0 |
| 13.33 kN (BE, EA) | 42.7 MPa | ~6.3 |
| 0 kN (CD) | 0 MPa | n/a |

### Material ductility

A500 is a cold-formed, welded or seamless carbon-steel structural tube. Elongation for Grade B is typically on the order of 21–23% over a standard gauge length, and the specification limits carbon (~0.26%) and phosphorus/sulfur content specifically to preserve weldability and avoid embrittlement, both signs of an intentionally **ductile** material [1][2]. Reported yield strengths for A500 range roughly from 230–345 MPa depending on grade and shape, so the assumed 269 MPa used in this design falls within the documented range for the standard [3]. Ductile steels give visible warning (yielding/necking) before final fracture, which is the basis for using a "yielding" limit state rather than a brittle-fracture limit state for these members [1].

### 1. Tension members (BE, ED, DA)

- **Expected failure mode:** Yielding of the gross cross-section, followed at higher load by ductile fracture (necking and tensile rupture). Because these members are pinned at both ends and see no compressive load reversal, buckling is not a concern for them.
- **Ductile/brittle:** Ductile (A500 steel, per above).
- **Reasoning:** All three members operate below σ_y (269 MPa) by the FoS shown in the table above, so yielding is not expected under the design load; the members are intentionally sized so first yield — not fracture — is the controlling limit state, consistent with standard ductile-material design practice. The real point of local concern for a tension member is not the gross section but the **net section at the pin hole**, where the hole removes area and creates a stress concentration; net-section rupture and block-shear are recognized failure modes at pinned tension connections in bolted/pinned steel joints [4][5].
- **Design modification:** Increase the pin-hole edge distance and/or locally widen the member (a "pad" around the hole) so the net section at the pin is not the controlling area — this shifts the critical section away from the hole and back toward the gross-section yield check, which is the more predictable, ductile failure mode.

### 2. Compression members (BC, CE, EA)

- **Expected failure mode:** Two competing modes must be checked — yielding (crushing) of the cross-section, and elastic/inelastic **buckling**. Which one governs depends on the slenderness ratio (KL/r) of the member, not on force alone. Short, stocky compression members (low L/r) fail by yielding at a stress close to σ_y; long, slender members (high L/r) fail by buckling at a stress well below σ_y [6][7]. Buckling is considered a failure mode in its own right even when it happens with no material yielding, because the member loses its ability to carry load once it deflects laterally [8].
- **Ductile/brittle:** Ductile (same A500 material), but note buckling itself is a **geometric/stability** failure, not a material-strength failure — a member can buckle while the material is still fully elastic, so ductility does not protect against it the way it does against yielding [6][9].
- **Reasoning:** The area was sized purely from a normal-stress (yield) check (σ = F/A), which is correct for tension members but is only half the check for compression members. Because A500 members are supplied as hollow structural sections (tube), they naturally have a larger radius of gyration for a given cross-sectional area than a solid bar of the same area — this is favorable for buckling resistance, since Euler's critical load is proportional to EI/L² and a tubular shape maximizes I for a given material quantity [9][10]. However, without checking the actual slenderness ratio (KL/r) of BC, CE, and EA against the material's critical slenderness ratio, it cannot be confirmed that yielding — rather than buckling — is actually the governing failure mode for these members.
- **Design modification:** Perform a slenderness check (KL/r) for each compression member and compare the resulting critical buckling stress to σ_y; if buckling governs, increase the tube's outer diameter (which increases r more efficiently than increasing wall thickness) or shorten the unbraced length with additional bracing, rather than simply adding cross-sectional area, since adding area to a compact bar shape helps yielding capacity but does relatively little for buckling capacity.

### 3. Zero-force member (CD)

- **Expected failure mode:** None under the stated design load (F = 0), so a strength-based failure mode does not apply.
- **Design modification:** Even though it carries no calculated force under this specific loading, CD should not be removed — zero-force members maintain the joint geometry and provide buckling restraint/redundancy for adjacent compression diagonals under secondary loads (self-weight, minor load eccentricities, or an alternate load case not shown here). It should be sized to at least a practical minimum member size rather than to zero area.

---

## Part 2 – Pin Connections

### Governing pin data

- Largest force transferred through a pin: 24 kN (at the CE/ED joints)
- Computed minimum pin area: 81.90 mm² → approximate pin diameter ≈ 10.2 mm
- Material: hardened tool steel, τ_y = 170 ksi (1172 MPa), FoS = 4

### 1. Expected failure mode

The pin was explicitly sized using a **shear stress** check (τ = F/A), which is the correct primary check for a pin in a truss joint — the pin is loaded transversely by the members framing into it and is cut by shear across its cross-section, exactly like the shank of a bolt in a lap joint. Direct shank shear is described as "the most direct mechanism" for a pin or bolt acting as a shear connector under transverse load [11]. However, shear of the pin itself is only one of several recognized failure modes at a pinned/bolted connection. The others act on the *members* (lugs) around the pin, and design codes require **all** of them to be checked, not just pin shear:

- **Bearing failure** — the pin crushes/ovalizes the hole in the surrounding member before the pin itself shears [12][13].
- **Tear-out (shear-out) failure** — if the edge distance from the hole to the member's edge is too small, the material ahead of the pin shears out in two planes and the pin pulls free; this is generally avoided by keeping the edge margin at or above about 1.5 times the pin diameter [14].
- **Net-section/hoop-tension failure** of the lug material itself around the hole [15].

A pin connection is only as strong as its weakest failure mode, so shear alone does not guarantee the joint's safety — the surrounding member geometry has to be checked too [14].

### 2. Supporting data / reasoning

The problem's assumed shear yield strength of 170 ksi (≈1172 MPa) is consistent with the pin being made from a fully hardened, high-carbon tool steel (e.g., an air-hardening grade like A2 or D2). Reported *tensile* yield strengths for hardened tool steels of this class run roughly 105,000–111,000 psi, with maximum attainable hardness around Rockwell C59–C65 [16][17]. Using the typical shear-to-tensile yield relationship from the Tresca/von Mises criteria (τ_y ≈ 0.5–0.58 σ_y), a 170 ksi shear yield implies a tensile yield on the order of 290–340 ksi, which is plausible only at very high hardness — and that hardness is exactly what makes the material behave in a **quasi-brittle** manner rather than a ductile one. Sources on hardened tool steels are explicit that as yield strength/hardness increases through quenching, ductility and impact toughness drop sharply, and fully hardened, high-carbon steels are described as prone to brittle, sudden fracture, particularly under impact or complex stress states [18][19][20].

This is an important contrast with Part 1: the truss members themselves are ductile A500 steel and are expected to yield (deform visibly) before they fail, giving a warning. The pin, by contrast, is a hardened, comparatively brittle component — if it does fail, it is more likely to fail suddenly by fracture with little or no visible warning, which is a materially different (and less forgiving) failure characteristic than the members it connects.

### 3. Design modification

- **Check bearing and tear-out, not just shear.** Confirm the member thickness at the hole and the edge distance around each pin (≥1.5× pin diameter, per typical pin-joint guidance) so that bearing/tear-out of the *member* does not govern before the pin itself would shear [14].
- **Add margin for the brittle failure mode.** Because a fully hardened tool-steel pin fails in a brittle, low-warning manner, consider either (a) increasing the pin's FoS beyond 4, or (b) specifying a quenched-and-tempered alloy steel pin at a slightly lower hardness in exchange for greater fracture toughness and a more ductile (yield-before-fracture) failure mode, similar in spirit to the ductile members it connects.
- **Distribute bearing load.** Where the connected member is thin relative to the pin diameter, add a bushing or reinforcing plate around the hole to spread the bearing stress over a larger area and reduce the local bearing/tear-out risk.

---

## Sources

1. Alibaba Product Insights, "Exploring ASTM A500 Yield Strength: Material Grades, Properties, and Uses" — https://www.alibaba.com/product-insights/astm-a500-yield-strength.html
2. PandaPipe, "A500 Steel Properties Full Analysis" — https://pandapipe.com/blog/a500-steel-properties/
3. BeamDimensions, "ASTM A500 Material Properties" — https://beamdimensions.com/materials/Steel/ASTM/ASTM_A500/
4. ScienceDirect, "Machine learning-based failure mode identification of double shear bolted connections" — https://www.sciencedirect.com/science/article/abs/pii/S1350630722004459
5. NCBI/PMC, "Failure Mode Analysis of Aluminium Alloy 2024-T3 in Double-Lap Bolted Joints" — https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5455755/
6. MechaniCalc, "Column Buckling" — https://mechanicalc.com/reference/column-buckling
7. EngineeringToolbox, "Euler Column Buckling: Formula, Theory & Calculator" — https://www.engineeringtoolbox.com/euler-column-formula-d_1813.html
8. The Efficient Engineer, "Understanding Buckling" — https://efficientengineer.com/buckling/
9. EngineeringHulk, "Column Buckling — Euler's Formula" — https://engineeringhulk.com/mechanical/strength-of-materials/column-buckling/
10. FicientDesign, "Column Buckling Explained" — https://ficientdesign.com/column-buckling-explained-eulers-critical-load-and-slenderness-worked-example/
11. Cosmobc, "Common Bolt Shear Failures Engineers Should Consider in Design" — https://cosmobc.com/common-bolt-shear-failures/
12. Machine Design, "What's the Difference Between Bearing, Shear and Tear-Out Stress?" — https://www.machinedesign.com/fastening-joining/article/21834800/whats-the-difference-between-bearing-shear-and-tear-out-stress
13. ScienceDirect, "Bearing-strength of high strength steel plates in two-bolt connections" — https://www.sciencedirect.com/science/article/abs/pii/S0143974X18309787
14. Tool Croze, "Pin Shear Stress Calculator | Pin Joint Check" — https://toolcroze.com/pin-shear-stress-calculator/
15. MechaniCalc, "Lug Analysis" — https://mechanicalc.com/reference/lug-analysis
16. Huyett, "Grades of Tool Steel: An Introduction" — https://www.huyett.com/blog/tool-steel
17. Huyett, "Steel Grading, Hardness, Yield Strength, and Alloys" — https://www.huyett.com/resources/production-and-design/materials-and-attributes
18. Rapid Protos, "Yield Strength of Steel: Carbon, HSLA, Stainless & Tool" — https://www.rapid-protos.com/yield-strength-of-steel/
19. Nuclear-power.com, "Tool Steel - Characteristics and Uses" — https://www.nuclear-power.com/nuclear-engineering/metals-what-are-metals/steels-properties-of-steels/tool-steel/
20. MFG Shop, "Understanding the Shear Strength of Steel: A Comprehensive Guide" — https://shop.machinemfg.com/understanding-the-shear-strength-of-steel-a-comprehensive-guide/

---

## AI Use Disclosure

An AI assistant (Claude) was used as a research and drafting aid for this assignment, in the following way:

- **Prompt given:** The student's handwritten static analysis, member-force table, member sizing calculation (A500 steel, σ_y = 269 MPa, FoS 3.5), and pin sizing calculation (hardened tool steel, τ_y = 170 ksi, FoS 4) were provided, along with the assignment instructions to identify likely failure modes (yielding, fracture, buckling) for the truss members and pin, state ductility/brittleness, support the reasoning with stress comparisons and credible sources, and propose design modifications.
- **What the AI did:** The assistant ran web searches to find credible sources on (1) ASTM A500 mechanical properties and ductility, (2) buckling/slenderness criteria for compression members (Euler and Johnson formulas), and (3) pin/bolt failure modes (shear, bearing, tear-out) and typical hardened-tool-steel properties, then used those sources to organize and support the failure-mode reasoning above.
- **What remained the student's own work:** The static analysis, member force values, cross-sectional area sizing, and pin sizing calculations shown at the top of this document are the student's own hand calculations (from the uploaded work) and were not generated or altered by the AI. The AI was not used to perform or check the numerical engineering analysis — only to research supporting literature and help structure the written explanation of failure modes.
