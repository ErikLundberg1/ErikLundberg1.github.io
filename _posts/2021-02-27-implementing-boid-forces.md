---
layout: post
---
### Making cars not collide
The next step of the project was to make sure that cars would not collide during the simulation. As stated in the specification for the project, the cars should have a random velocity. This could potentially allow for the car behind to crash into the on that is infront of it. To prevent this, I implemented all the relevant boid forces for this project. These were separation force and alignment force. The purpose of the separation force is to affect the acceleration of the car behind, such that it would brake if going to fast. Similarily, the alignment force could be used to make the acceleration of the car behind become the same as the car infront, which is exactly what we want. The radius and the magnitude of these forces can then be modified in order for the simulation to run smoothly. Furthermore, I also intend to use [Hooke's law](https://en.wikipedia.org/wiki/Hooke%27s_law) in order to decelerate the car by a magnitude depending on how far it is away from the car infront. This will be used to break when further away, and the separation force will be more proximate, and prevent precarious situations to bring about collisions.

### Gif of progress

<div style="height: 0; padding-bottom: calc(56.25%); position:relative; width: 100%;"><iframe allow="autoplay; gyroscope;" allowfullscreen height="100%" referrerpolicy="strict-origin" src="https://www.kapwing.com/e/603a9399e3ff1b0029e92bda" style="border:0; height:100%; left:0; overflow:hidden; position:absolute; top:0; width:100%" title="Embedded content made on Kapwing" width="100%"></iframe></div><p style="font-size: 12px; text-align: right;"> <a href="https://www.kapwing.com/videos/603a9399e3ff1b0029e92bda" target="_blank" rel="noopener noreferrer"></a></p>
