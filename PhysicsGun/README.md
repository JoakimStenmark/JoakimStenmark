![title](Resources/Titel.png)

This was a game I had incredible fun making while learning the ins and outs of Unreal 4. 




## Gun Handling

For this project I started with the first person shooter template and modified it to suit my game idea of shooting to push objects around.

I wanted to to be able to charge up how hard the shots would push objects so I made these on the playercharacter blueprint:
![fire](Resources/ProjectileFire.png)
![spawn](Resources/ProjectileSpawn.png)

The power value is the most important value here. When the mouse is pressed a timeline plays which increases the power value over time. I then use that value to set the projectiles velocity, and the gunfire sound´s volume and duration as it plays.  

On the projectile blueprint I set it up like this:
![projectile](Resources/ProjectileHit.png)

I added an Impulse multiplier here because the velocity needed to move the objects otherwise was way too high (so fast that one barely had time to see them).

Here I also use a cast to check if it's a key object. This game doesnt explore that design space at all but if I could, I would play around with this idea that you can't move other objects with the gun so you have to push a keyobject onto the other object, like Pool meets Half life 2.

Late in the game the overload mode on the gun is unlocked which is used to move the big ball into the final goal. 

