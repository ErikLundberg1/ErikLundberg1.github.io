---
layout: post
---

### Group Members
Erik Lundberg (erilundb@kth.se)
### Grade
I am aiming to get a passing grade on the project.
### Specification Details

##### **BACKGROUND**
There are several ways to simulate how traffic flows. One way to do this is to use the intelligent driving model (IDM). IDM provides a mathematical model of what the acceleration is for every individual car on a road based on real driving behaviour in a single-lane traffic situation. The model roughly does this by taking into account the speed and the distance of the car infront of it, the minimum distance allowed between cars, the ideal speed of the car, and then uses this to derive the acceleration for each car at the current moment. After this has been done, the new speed for each car is updated, and a new position is calculated for each car. Boids is an artifical life simulation developed by Craig Reynolds in 1986. The aim of that simulation was to replicate the behaviour of birds. The simulation works by specifying certain rules, or behaviours, that each boid must follow, and then creates clones of those, and they are able to generate a result that is complete and realistic. It has been used primarly for simulating natural life, but it has also been used to simulate other emergent behvaiour that emanates from indiviual actors interacting with one another.

##### **IMPLEMENTATION SPECIFICS**

The main purpose of the project is to be able to create a model that can somewhat accurately simulate how real traffic could look on a highway with two lanes. To be able to achieve this, I will try to get my model to take into account some of the factors that are included in the IDM, but instead use physical formulas and boids to get a similar result. The project will be done by using Unity. The more formalized goals of the project are:

- Allow the cars to change lane to the left if they want a higher speed, without colliding with other cars.
- In order to implement collision protection, the cars should decelerate to the speed of the car forward if they get close enough.
- The lane changing should be done in a smooth manner, perhaps by using linear interpolation.
- Spawn cars with a random velocity at the start of a lane.
- Make the cars keep appropriate distance to the cars around it, such that no collisions occur.
- Spawn a new car once an old car has reached the end of the road, and destroy the old one.
- Allow each car to have its own ideal speed that it always should try to reach by accelerating at a specified comfortable acceleration rate.
- Find an efficient way to spawn the cars so that they appear to be spawning naturally.
- Use a 3D model of a highway and of a car in the simulation.
- Implement a camera script that allows the camera to be moved during runtime of the simulation.

If I find that I have time left after completing the basic functionality, I will consider adding the following extensions:
- Implement so that cars going slower than the cars behind in the left lane should try to switch to the right lane.
- Add traffic lights that will force the cars to come to a stand still until the light becomes green.
- Add one more lane to the road, and implement the lane changing so that it works with this.

##### **Minimum viable product**
As time might become scarce, it would be desirable to figure out how a resonable minimum viable product could look. I think it would be resonable that it should include the basic functionality, and not include things that are related to apperance or performance. Some possible criterion for the mvp are stated below:

- Cars should spawn at a lane with a random velocity.
- Cars should decelerate in order to prevent collision with the car infront of it.
- Each car should have an ideal speed that they try to reach by accelerating with a comfortable acceleration.
- The cars should keep a minimum distance to one another at all times.
- A car should change lane to the other lane if it can better reach its ideal speed in that lane, without in the process colliding with other cars.

##### **SPECIFICS OF WHAT THE FINAL SYSTEM WILL LOOK LIKE AND DO**

[This Youtube link](https://www.youtube.com/watch?v=W_kYXpAEnd8&ab_channel=DerPhysiker) shows something akin to what I am looking to achieve. The result should look something like the video, but I have decided to restrict the road to consist of two lanes instead of three, initially. Furthermore, I am looking to do the simulation in 3D, with a camera that provides a third person view of the simulation. The camera should be able to be moved around freely, in order to get different views of the simulation. In addition, the simulation should appear fluent and realistic.

#### POTENTIAL RISKS/CHALLENGES

With regards to risk, since the scope of the project is rather limited, as by choice, I do not excpect there to be any major unmanagable difficultues during the project. There could, however, be some issues with the simulation not working as well as I would like it to do, which could be my biggest concern at this stage. For instance, getting the formulas and forces together might be more difficult than I anticipated, and might not work as well as I would like them to do. To solve this, I will opt to use fewer formulas initially, since it would seem that getting them to work together would be easier, and then add more on to make the simulation more complex and more realistic. Moreover, I have created specific criterion for what is needed to produce a minimum viable product, which should be what I am aiming to achieve before adding on more complex tasks as well as visual improvements. If some other unforeseen diffuculties were to emerge, I would likely be able to solve them by going to a project session and asking for help.

####  DEGREE OF SIMULATION
To achieve the result I want, I believe that it will be sufficient to utilize the physics that was provided in Lab 1. The particular physics formulas that I am looking at are: Hooke's Law, the Separation Force, the Cohesion Force, the speed constraints used in Lab 1, and perhaps some acceleration formulas. I might also want to be able to have air restistance, which then would allow for a better control over the simulation. All of the above can be implemented directly into the built-in physics in Unity, and thus requires no additional physics library.

##### [LINK TO BLOG](https://eriklundberg1.github.io/)

#### REFRENCES
Kesting, A, Treiber, M. (2013). Traffic Flow Dynamics. 1 ed. Chapter 11. Springer-Verlag Berlin Heidelberg.

https://cs.stanford.edu/people/eroberts/courses/soco/projects/2008-09/modeling-natural-systems/boids.html
