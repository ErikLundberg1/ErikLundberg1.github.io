---
layout: post
---

### Implementing a traffic light

Prior to starting this, I achieved all the criterion that I set for the minimum viable product. The next step, as I felt that I had some additional time to spend on the project, was to create a functional traffic light that the cars responded to. To achieve this was an ardorous task. The basics of my current implementation relies on collision detection between the car and the area in front of the traffic light, so as to notify the car that a traffic light exists. If it is red, the cars will decelerate according to the following formula:  
  
![Image](https://mathformulas.in/wp-content/uploads/mathsformulas/cms/images/83/formula-for-the-deceleration.png)
  
This will ensure that each car comes to a standstill at the traffic light. After the light then becomes green, the cars will start accelerating again. As of now, I will continue to work on the project, with the emphasis being on fine-tuning such that the simulation appears natural. I had prior stated that I might opt to add an additional lane, but as I feel like there is still work to be done, I will most likely not have sufficient time to implement that. Moreover, I intend to enhance the lane changing to also allow cars to change to the right lane if they are going to slow for the left lane.

<div style="height: 0; padding-bottom: calc(56.25%); position:relative; width: 100%;"><iframe allow="autoplay; gyroscope;" allowfullscreen height="100%" referrerpolicy="strict-origin" src="https://www.kapwing.com/e/6042a0d771cbf000cc8b01c0" style="border:0; height:100%; left:0; overflow:hidden; position:absolute; top:0; width:100%" title="Embedded content made on Kapwing" width="100%"></iframe></div><p style="font-size: 12px; text-align: right;"><a href="https://www.kapwing.com/videos/6042a0d771cbf000cc8b01c0" target="_blank" rel="noopener noreferrer"></a></p>  
