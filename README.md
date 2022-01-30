# Hack the QMap

Guess the terrain of the quantum map!

## Team

Sumit Suresh Kale, Rishabh Gupta, Shree Hari Sureshbabu, Shah Ishmam Mohtashim

## What is 'Hack the QMap'? 
Hack the QMap is a game powered by quantum computing where the players of the game have to build quantum circuits, gate by gate in each move of the game, to generate terrain which is as close to the original terrain generated by our quantum game engine!(circuits).

This game is the marriage between the two of the challenge ideas of the IonQ + Microsoft Joint Challenge @ MIT iQuHACK 2022:
* Using a quantum computer to procedurally generate maps
* Using quantum logic itself as a gaming mechanism for both fun **AND** education!


### Qunatum Game Engine for Map Generation
Random map generation is an important part of game design. Map generation can not be completely random as it is subject to the constraints of being aesthetic, having some sort of symetry yet unique, being relevant to the experince of the game and solvable as well. Meeting all these contraints means repeatation of some set models, which undermines the uniqueness of the game content. Hence, satisfying all these and constraints and still providing a fresh experience everytime is a mammoth task. For our game, we have used the power of quantum computing to help us with this 'seemingly impossible' task.

The generated map is simply a form of representation of the probabilty distributions of the basis states. Each block in the lattice represents a basis state and the colour of the blocks are determined by the probabilty of getting that state. The blocks will be darker for states whose probability is low, and lighter for high probability states. The lowest probabilities are made black, the highest are white and the scaling of the shading is logarithmic.

The probabilites of the states are generated by our quantum game engine i.e set of quantum ciruits where we have included randomness during parameter selection of the rotation gates but ensured that the final wavefunction generated is in the entangled regime. 

![map1](map1.png)


### Playing the game




