[[Paper]](http://nd.ics.org.ru/nd221208/) [[Documentation]](https://drive.google.com/file/d/1mzSFjXsLGNrE1SjGGM3FPeQPK2IoKhK4/view?usp=sharing) [[NIR 2022 Conference Presentation]](https://drive.google.com/file/d/1jKnN-oI8are-T6YKvFMAqkvB3s6L5WAM/view?usp=sharing)
## Double-Pantograph-Stiffness-Modelling
This repository contains the implementation of the stiffness analysis of the double pantograph transmission system. The importance of stiffness modelling is to improve the overall accuracy of the robot by calculating the difference between the desired pose and the actual pose of the robot due to the applied load.
It is implemented using VJM and MSA techniques to fnd the EE deﬂection at different points in the workspace. After deﬂection calculations, deﬂection scatter plots are built to analyse the maximum deﬂection due to 100N force along x, y, z directions respectively. It was found that VJM method has some limitations to model this structure, which prevent evaluating the deﬂection with an external load in x, z directions. A comparative analysis is performed to compare both MSA and VJM computation complexity and deﬂection deference. It was noticeable that MSA has less computation cost and no limitations to model the double pantograph structure compared to VJM approach.

## Double Pantograph
- Double Pantograph includes two sets of vertically stacked scissors which are pinned directly together, stabilized, and raised simultaneously.
- The design creates a stable structure for high travel applications and consumes less floor space, so it can easily fit among other work equipment.
- Common applications include parts assembly and disassembly, personnel work platforms, mezzanine, and multiple landing access. 
<img src="https://user-images.githubusercontent.com/90580636/176668254-663de557-9418-44ee-83e4-c21c1ffb9459.png" width="300" height="300" />

## Kinematics 
<p float="left">
  <img src="https://user-images.githubusercontent.com/90580636/189139491-e488be91-3fde-45ac-b423-277a1ec6dd7f.png" width="400" height="250" />
  <img src="https://user-images.githubusercontent.com/90580636/189139604-d24336a5-a929-4690-b6f8-7ba8fa2f6c89.png" width="400" height="250" />
</p>

## Matrix Structural Analysis
<p float="left">
  <img src="https://user-images.githubusercontent.com/90580636/189139906-3b07366d-d055-43dd-92d1-ba898b301946.png" width="400" height="250" />
  <img src="https://user-images.githubusercontent.com/90580636/189139923-d65527dc-ae1c-4308-8902-0ae94371fd87.png" width="400" height="250" />
</p>

<p float="left">
  <img src="https://user-images.githubusercontent.com/90580636/189140063-b1152aab-93d6-43ab-9658-7fc214408a5a.png" width="400" height="250" />
  <img src="https://user-images.githubusercontent.com/90580636/189140085-3cb232d8-4ef4-40c1-9976-4328df99e4c8.png" width="400" height="250" />
</p>

<p float="left">
  <img src="https://user-images.githubusercontent.com/90580636/189140252-7025f0de-f86e-4173-b261-7b362140a46a.png" width="400" height="250" />
  <img src="https://user-images.githubusercontent.com/90580636/189140278-9f219789-3385-4bcf-9072-6cf7aee18c25.png" width="400" height="250" />
</p>

![image](https://user-images.githubusercontent.com/90580636/189140303-1f6b199e-e057-4fed-9a65-5b49b9d72d7d.png)

### Virtual Joint Modelling
<p float="left">
  <img src="https://user-images.githubusercontent.com/90580636/189140685-bba3d2aa-b92b-4112-9413-d3aeef0daa9a.png" width="400" height="250" />
  <img src="https://user-images.githubusercontent.com/90580636/189140704-562312e0-1fe1-4617-8201-509f5abe74b0.png" width="400" height="250" />
</p>

<p float="left">
  <img src="https://user-images.githubusercontent.com/90580636/189140734-8f9c698e-dc29-4eae-973b-5a3f418ff3a1.png" width="400" height="250" />
  <img src="https://user-images.githubusercontent.com/90580636/189140763-e663fc6d-972f-4131-afd7-773dfed5082a.png" width="400" height="250" />
</p>

![image](https://user-images.githubusercontent.com/90580636/189140779-fc10ef4f-c73e-404f-9655-494d6dc45cb2.png)

## Results
<p float="left">
  <img src="https://user-images.githubusercontent.com/90580636/189141123-bde122c2-a20f-477a-87da-2550dce0ce44.png" width="400" height="250" />
  <img src="https://user-images.githubusercontent.com/90580636/189141142-88932980-4783-45c0-ae62-f8e4eb2be3d7.png" width="400" height="250" />
</p>

<p float="left">
  <img src="https://user-images.githubusercontent.com/90580636/189141155-e920ae5e-b873-45a3-b62f-c3d1ae39e0b6.png" width="400" height="250" />
  <img src="https://user-images.githubusercontent.com/90580636/189141177-234388f4-2afc-4aba-866e-75c8e367cd7f.png" width="400" height="250" />
</p>

## MSA - VJM Comparison  
As VJM limitations do not allows us to compare the deflections due to forces in x and z directions with the corresponding deflections from MSA, deflections are compared by applying forces in y-axis.

<p float="left">
  <img src="https://user-images.githubusercontent.com/90580636/169873194-ea15a37a-d2e2-4bec-bfb1-4e32b9dd0623.png" width="300" height="200" />
  <img src="https://user-images.githubusercontent.com/90580636/169873289-08462128-badd-47d2-9840-1145acda43a5.png" width="300" height="200" />
</p>
<p float="left">
  <img src="https://user-images.githubusercontent.com/90580636/169873493-26ce0f1e-5775-407e-92a3-377c9cfdfd92.png" width="300" height="200" />
  <img src="https://user-images.githubusercontent.com/90580636/169873392-eb278311-cac1-42f3-9881-36da38ed2366.png" width="300" height="200" />
</p>

