---
layout: post
---
### Implementing basic lane changing functionality

The next step in the project was to enable cars to change lane if they could get closer to their ideal speed by doing so. To achieve this, I created a method that checks the other lane such that there are no cars within a certain range, and that the speed of the car that is changing lane is larger, by some amount, than the car behind in the new lane. This should be somewhat realistic, since the car behind should not be slowed significanlty when a car changes lane in real life. Furthermore, the previously implemented separation force can come in handy, as it will always make sure that no collisions can occur, so at the right values, this should also improve the lane changing functionality. 

<div style="height: 0; padding-bottom: calc(48.58%); position:relative; width: 100%;"><iframe allow="autoplay; gyroscope;" allowfullscreen height="100%" referrerpolicy="strict-origin" src="https://www.kapwing.com/e/603a9d90f7d0d90103b46c11" style="border:0; height:100%; left:0; overflow:hidden; position:absolute; top:0; width:100%" title="Embedded content made on Kapwing" width="100%"></iframe></div><p style="font-size: 12px; text-align: right;"> <a href="https://www.kapwing.com/videos/603a9d90f7d0d90103b46c11" target="_blank" rel="noopener noreferrer"></a></p>
