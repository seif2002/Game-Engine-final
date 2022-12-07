# Game-Engine-final

Final Midterm

I apologize my UNITY is not functioning as it should I've tried fixing it over the last few days but had no luck, so I apologize for not being able to add implementations but I hope the explanation is worth a few marks.


Implement object pooling to increase the number of ducks in a scene.

you need to create and destroy objects frequently. Objects are similar in size.
allocating objects on the heap is slow or could lead to memory loss. These are the reason why people who know how will usually go with object pooling. 
 
I first need to create an empty game object and that will be the pool manager, then we will also need to make a pool manager script, and we'll add that to that empty game object. I would add a singleton to the pooling script so that when it's being called on it's easier for the system. I would make a list to hold the prefabs and a variable to tell the game how many prefabs there are I will create a method that will return as a list. This method will take an integer parameter, loop through, and create a prefab based on the integer given. This will let the system know how many ducks there should be at a time and what the conditions to create or destroy an old duck are. Next, I will set the list equal to the method. And the last part would be to state when the pool is active and when it's not, what all the conditions are, and basically where all information will be added to clarify what the pooling will do and when.
 
Implement the command design pattern for rebinding and controller when missing two ducks in a row by inverting the up and down aiming movement.
 
	The Command Pattern is a design pattern that holds all of the information about a specific action or event and sets it up so it can be called at a later time by other scripts.

	The command design pattern will be used here to invert the controls for the up and down aiming movement. First, we will have to declare bullets as well as ducks, we will also declare that every time a bullet hits a target a point is awarded to the player, using the pooling system we made earlier, as soon as a bullet is destroyed it's announced to the system. After that, we must make an if statement stating this, if the bullet does not make contact twice in a row, set the y-axis to -y else if points are being awarded between shoots keep axis as is.
 	
