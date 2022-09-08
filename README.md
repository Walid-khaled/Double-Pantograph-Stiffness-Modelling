[[Documentation]](https://drive.google.com/file/d/1kJkWLKQVz44wYvOEMuEN74OpXt39nmQ4/view?usp=sharing)
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
  <img src="https://user-images.githubusercontent.com/90580636/176676885-1cb6c737-12a9-49cd-8afd-511c9d349e76.png" width="400" height="250" />
  <img src="https://user-images.githubusercontent.com/90580636/176676916-4856fb85-d982-45fa-9f77-1089f8f877db.png" width="400" height="250" />
</p>

<p float="left">
  <img src="https://user-images.githubusercontent.com/90580636/176676943-2ef87d9b-189e-4c79-b72b-194a908520d9.png" width="400" height="250" />
  <img src="https://user-images.githubusercontent.com/90580636/176676970-d50fa379-6116-4b5d-85a0-7a8ded6ca529.png" width="400" height="250" />
</p>

<p float="left">
  <img src="https://user-images.githubusercontent.com/90580636/176676992-6dfa6891-9acb-40af-ae77-cea5e1bdcb32.png" width="400" height="250" />
  <img src="https://user-images.githubusercontent.com/90580636/176677019-6cd0ca53-a9f4-424b-97c9-cd8529f17501.png" width="400" height="250" />
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

