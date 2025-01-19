## Mechanical Design

### Feeding Solid Ingredients
I explored several valve options for controlling the feed of solid ingredients, including rotary valves, slide valves, etc. My criteria were:
- Simplicity
- Use of available raw materials

I narrowed it down to two options:
- **Horizontal Auger Valve**
- **Vertical Auger Valve**

#### Decision:
I have chosen the **vertical auger** mainly because it is less space-consuming and easy to construct with available plumbing materials.

#### Concept:
The solid ingredient feed (SIF) needs to be easily washable and easy to store on a refrigerator’s door shelf (with a diameter of less than 50mm). Based on this, I designed and created a paper prototype of such an SIF.

#### Steps:
1. Create an **outer body cylinder**.

- **Outer Diameter (D1)** = 50 mm
- **Length (L)** = 120 mm

When you roll a rectangular piece of paper into a cylinder, the width of the paper becomes the circumference of the rolled cylinder, and the length of the paper becomes the height (or length) of the cylinder.

The outer circumference of the cylinder is given by the formula:

C = pi x D1

Where, pi is approx 3.1416

Substituting the given values,

C = 3.1416 x 50mm = 157.08mm

- **Width of the Paper (Circumference)** = 157.08 mm
- **Length of the Paper (Height of the Cylinder)** = 120 mm
---

2. Create an **auger screw**.

This involved 2 parts: 
- The center pipe that drives the auger blade
- The auger blade itself.

I created a center pipe of 8mm diameter using the **C = pi x D** formula. The difficult part was to find the formula for designing the auger blade; so that, I can design it on a flat surface and cut it to form the auger blade.

I found the following formula to calculate the inner diameter and the outer diameter of the auger blade.

##### Parameters

- **D<sub>1</sub>** : Outer cylinder diameter (50mm)
- **D<sub>2</sub>** : Inner pipe diameter (8mm)
- **Pitch** : linear distance between two flights (20mm)

##### Values to be calculated

- **D<sub>out</sub>** : Outer diameter of the flat cut auger blade
- **D<sub>in</sub>** : Inner diameter of the flat cut auger blade

- L = &radic;((D<sub>1</sub> x Pi)<sup>2</sup> + P<sup>2</sup>)
- l = &radic;((D<sub>2</sub> x Pi)<sup>2</sup> + P<sup>2</sup>)
- D<sub>in</sub> = (D<sub>1</sub> - D<sub>2</sub>) / ( (L / l) - 1 )
- D<sub>out</sub> = (D<sub>1</sub> - D<sub>2</sub>) + D<sub>in</sub>

Doing the math, gave me following values:

- D<sub>in</sub> = 6.67mm
- D<sub>out</sub> = 48.67mm

##### This is how the flat cutouts looked

<img src="https://github.com/user-attachments/assets/99294d54-ecc1-4fa9-b38e-137365ae4dc3" width="400" />
<br/>
<img src="https://github.com/user-attachments/assets/fac58683-acb1-4ad1-ae85-2fb181e7f698" width="400" />

---

3. Test and validate with mock solid ingredients.

![auger_concept](https://github.com/user-attachments/assets/b101b52e-3201-4426-9b9c-4e5206c61f87)

---

### Feeding Liquid Ingredients
My first thought is to break it into 2 types:
- High volume liquid feed (Eg: Water)
    - May use a gravity fed solenoid controller valve system
- Low volume liquid feed (Eg: Oil)
    - Looking at commercially available syringe (>100ml capacity)

### Feeding Semi-Solid Ingredients

Yet to work on it.
