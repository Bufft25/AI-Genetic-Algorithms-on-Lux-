# AI-Genetic-Algorithms-on-Lux-
#Artificial Intelligence: Project Proposal
#Group Members: Adam Tucker, Travis Buff, Peter Cipolone 

#Project Goal: 
To use a genetic algorithm on the board game Lux (same game play as risk) in order to create an artificially intelligent computer player. 

#Project Language and Platform: 
This genetic algorithm will use the Java programming language and will run on Microsoft Windows. As for the entire project, the languages used will be the languages which the SDK uses, which will be mostly Java. 

#User Interface:
The user interface which came with the game will be used, and this interface will reflect the genetic algorithm changes made in the SDK. 

#Proposal: 
The objective of this project is to create and implement a genetic algorithm on an already made Lux (risk) board game. The lux delux game is an open-sourced SDK called SillySoft. A genetic algorithm will be used, which can find the quickest way to winning the game (taking control of all the territories on the board). This project will involve a lot of rankings such as where to place armies, which country to attack, and how fortifications will be done. Over many generations, these rankings will be more and more precise and will eventually help the AI bot to win the game. 

To use the genetic algorithms effectively, efficient data structures will be selected. There will be two data structures used; a binary string for each individual gene in a chromosome and a priority queue based on a heap sort for the population in each generation. There will be a weighted number calculated to represent fitness, and the individuals in the priority queue will be placed based on their fitness number. 

Fitness will be calculated in three different ranks based upon the three phases of a single turn in the game. The three ranks are named after the three phases: reinforcement rank, attack rank and fortification rank. For example, the reinforcement rank will be computed by a few factors such as army advantage, territories held, and cards currently in your hand. Each phase shares information, but is not necessarily dependent on the rank of each phase because each phase has its own individual goal. The ranks will be calculated by using an algorithm which produces the probability of a successful solution.

Mutations will occur with one or more of the bits of the binary string that is randomly flipped. The algorithm will implement a function which gives a small probability that one of the bits will be flipped. The exact probability is currently unknown, but it will mostly likely be a hundredth or thousandth of a percent. Crossovers in our algorithm will occur when two individuals split at a random point and those pieces come together to form a new individual for the next generation. They will then receive a fitness number and be placed in the heap. Two binary strings will be randomly split in half and inter combined to produce new solutions along with their calculated fitnesses.
