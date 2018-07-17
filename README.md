# Finite-State-Machine-Simulation
A text based game using non-deterministic finite state machine without outputs. Developed with JFLAP.

Game Title: Evil Robots Are Outside

Description:
Evil robots are outside your home rampaging the entire city! Being a hero, your job is to go outside to search and destroy robots as soon as possible. Be careful, however, as the terryfying robots are capable of shooting deadly laser beams that will vaporize any human being within seconds. You must successfully hide from their laser beams, or you will die.

Picture of NDFA
![NDFA](https://image.ibb.co/n1Wdyd/JFLAP.png)

Game Test
![NDFA_TEST](https://image.ibb.co/hdkhPJ/JFLAP_2.png)


In the screenshot above, the first three inputs are valid game state changes. For example, the first is the sequence of the player going outside, encountering robots and then destroying robots. The second is the sequence of the player going outside, encountering robots and getting killed with the laser beams from robots. The third is the sequnce of the player going outside but getting killed by robots shooting laser beams without encountering any robots. 

The last three inputs are not supposed to happen. The input “Go_OutsideRobot_Kills” means the player goes outside but gets killed by robots right away. Moroever, the input “Go_OutsideEncounter_RobotRobot_Kills” means the player goes outside, encounters robots, and gets killed by robots. These two inputs are illegal moves because robots have to first shoot laser beams in order to kill the player. The last input means the player goes outside, hides, and gets killed by robots. This is illegal since robots cannot kill the player when the player is hidden.
