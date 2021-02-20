---
layout: post
---


### Creating a road and making cars move

To start of with the project, I created a road out of a rectangle with appropriate dimension, and then found a texture of a road online.
After this had been done I created a rectangle that would represent a car. To get the car to spawn and then get destroyed once it has traveled to the end
of the road, I implemented some code that spawned clones of a prefab that I could select, by using [instantiate in unity](https://docs.unity3d.com/ScriptReference/Object.Instantiate.html). The prefab I choose to represent the car was a rectangle, which will serve as a placeholder that I can change to something else at a later stage. After this, I created a script that increased the transform.position with a fixed value, which later will be changed to the actual velocity, which made the car travel forward on the road. To get the car destroyed after a fixed coordinate position, I created a method that destroyed the current gameObject that reach that value, and once it was destroyed it then spawned a new clone at the start of the road. The result of this can be seen in the video below.


### Video
