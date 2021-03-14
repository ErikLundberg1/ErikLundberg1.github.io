---
layout: post
---


### Creating a road and making cars move

To start of with the project, I created a road out of a rectangle with appropriate dimensions, and then found a texture of a road online, that I applied to the road.
To get a car object to spawn and then get destroyed once it has traveled to the end of the road, I implemented some code that spawned clones of a prefab that I could select, by using [instantiate in unity](https://docs.unity3d.com/ScriptReference/Object.Instantiate.html). The prefab I choose to represent the car was a rectangle, which will serve as a placeholder that I can change to something else at a later stage. After this, I created a script that moved the *Rigidbody* of the car with a fixed value, which later will be changed to the actual velocity, which made the car travel forward on the road. In order to get the car destroyed after a fixed coordinate position, I created a method that takes a parameter with a coordinate and that destroyes the current gameObject once it reaches that value. Once it was destroyed, I set the method to spawn a new clone at the start of the road.

&nbsp;
sada
    
<div style="height: 0; padding-bottom: calc(48.58%); position:relative; width: 100%;"><iframe allow="autoplay; gyroscope;" allowfullscreen height="100%" referrerpolicy="strict-origin" src="https://www.kapwing.com/e/603a9e95a20c420119a91fb0" style="border:0; height:100%; left:0; overflow:hidden; position:absolute; top:0; width:100%" title="Embedded content made on Kapwing" width="100%"></iframe></div><p style="font-size: 12px; text-align: right;"><a href="https://www.kapwing.com/videos/603a9e95a20c420119a91fb0" target="_blank" rel="noopener noreferrer"></a></p>
