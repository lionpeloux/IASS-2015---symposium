# Formulation of a 4-DoF torsion/bending element for the formfinding of elastic gridshells


##Abstract

Elastic gridshells offer an efficient way to build freeform shapes from an initially flat structure. This capacity to “form the form” efficiently is of peculiar importance in the current context where morphology is a predominant component of modern architecture (F. Gehry, Z. Hadid, ...) and envelopes appear to be the neuralgic point for the environmental performance of buildings.
The “proof of concept” was made by Frei Otto in 1974 when he built the emblematic Multihall of Mannheim – a wooden elastic gridshell of 7500m2 – thanks to the expert knowledge he had developed on physical models and photogrammetry. More recently, the development of numerical models has encouraged the emergence of few projects made of cardboard (Hanovre 2000), timber (Downland 2004, Savill 2006) or composite material (Solidays 2011, Créteil 2013).

The major difficulty in the design of such structures is to compute the deformed geometry of the initially flat grid and the corresponding stresses due to beams bending and twisting. 3-DOF elements have yet been formulated to achieve such computations using dynamic relaxation integration scheme [1] but they don’t account for torsional effects, anisotropic sections or complex joint cinematic, which could be very limiting. 6-DOF elements have also been formulated but they suffer from ill-conditioning problems and convergence instabilities (Adriaenssens, Knippers, D’Amico).

The paper presents a completely novel approach to model elastic gridshells with a 4- DOF element based on recent advances in the field of hair modelling [2]. The reduction from 6 to 4 DOF is achieved with an appropriate curve framing introduce by R. Bishop. The resulting model is fast and efficient. Its accuracy has been validated on test cases.


## 1 - Introduction (1p)
Résumé punchy avec une belle photo sur half page


## 2 - Related Work (1p)
Biblio + critique des modèles passés 3DoF -> 6DoF => 4DoF


## 3 - Elastic gridshells (1p)

### Overview
Explain here what is an elastic gridshell : structure + materiel + erection process

### The work of Frei Otto
- Photogrametrie + hanging net
- IL13
- Mannheim

### Recent Projects
- Japan Pavilion 2000
- Downland 2002
- Savill 2006
- others ??

### Recent Developpements
- composites
- numerical methodes
- Solidays 2011
- Creteil 2013


## 4 - A novel 4-DoF torsion/bending element (3p)
Ici on développe le nouveau modèle en continue

### Kirchhoff rod
- introducing curvatures and twist
- adapted frame
- Darboux vector

### Kinematic
- centerline
- angle representation
- bishop frame as a reference (compare to frenet frame)

### Inextensibility
- explain why inextensibility is a reasonable assumption
- explain briefly how it will be ensured in the model

### Elastic energy
- Strecthing
- Bending
- Twisting

### Gradients
- Moments acting on theta
- Forces acting on the center line

## 5 - Numerical model (2p)
Ici on développe la discrétisation + la connexion

### Discret Bishop frame and parallel transport

### Inextensibility

### Moments

### Forces

### Joints

### Boundary conditions

### Dynamic Relaxation algorithm


## 6 - Test case (1p)
Ici on présente une application

## 7 - Conclusion
limitations and futur works
- Passage par Kirchhoff
- Raideur axiale adaptative
- Mesh refining
- Formulation avancée de l'algoroithm de relaxations dynamique
- Modélisation avancée de la connexion (méthode de projection / excentricité)
- Résolution implicite vs. explicite

## Acknowledgements

## References (1p)
