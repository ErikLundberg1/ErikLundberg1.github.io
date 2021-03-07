---
layout: post
---

### Making all the parts come together

In the previous updates, I worked more so on the different individual parts. The next stage, I felt, was to get everything to work well together.
This required me to set all parameters of the basic functionality, such that everything worked smoothly. The first thing that I did was to get the separation force and the spring force to work in a manner such that each car would break instead of colliding. After this, I implemented some criterion that would have to be fullfilled for the car to change lane, which was rather hard to make it function as I wanted it to do, and something I feel can be improved, though it has the basic functionality required for the project. Furthermore, I implemented the lane changing to the left lane if the car behind was going faster. This ended up working, but there are still some bugs related to this that I am unsure if I will be able to fix before the deadline. 
  
With regards to the traffic light, Its basic functionality works well. The current implementation only allows for the traffic light to be red the first run of the simulation. This is something that I will try to improve if I have time. Ideally, the light should be able to be enabled for every run of the simulation. 

A reflection that I have had when working with the project is that it is very difficult to make the simulation appear realistic. It feels like there are too many different 
parameters that you have to take into account to come up with something that is similar to reality. Furthermore, when modifying each of these parameters, they also seem to affect
each other, which means that as the number of parameters increase, it will also get harder to get the desired result by only changing the value of a single parameter. This means 
that it will be a lot easier to get a minimal functional simulation than it would be to get it to appear realistic. This should be something to take into account when trying to 
make a simulation more complex, without having all the basic functionality of the simulation implemented.
