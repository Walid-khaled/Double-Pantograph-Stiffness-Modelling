## Double-Pantograph-Stiffness-Modelling
This repository contains the implementation of the stiffness analysis of the double pantograph transmission system. It is implemented using VJM and MSA techniques to fnd the EE deﬂection at different points in the workspace. After deﬂection calculations, deﬂection scatter plots are built to analyse the maximum deﬂection due to 100N force along x, y, z directions respectively. It was found that VJM method has some limitations to model this structure, which prevent evaluating the deﬂection with an external load in x, z directions. A comparative analysis is performed to compare both MSA and VJM computation complexity and deﬂection deference. It was noticeable that MSA has less computation cost and no limitations to model the double pantograph structure compared to VJM approach.

---

### Results

<p float="left">
  <img src="https://user-images.githubusercontent.com/90580636/169873194-ea15a37a-d2e2-4bec-bfb1-4e32b9dd0623.png" width="300" height="200" />
  <img src="https://user-images.githubusercontent.com/90580636/169873289-08462128-badd-47d2-9840-1145acda43a5.png" width="300" height="200" />
</p>
<p float="left">
  <img src="https://user-images.githubusercontent.com/90580636/169873344-9bb2a158-917e-4118-bca3-f2c1a90b6b0f.png" width="300" height="200" />
  <img src="https://user-images.githubusercontent.com/90580636/169873392-eb278311-cac1-42f3-9881-36da38ed2366.png" width="300" height="200" />
</p>
