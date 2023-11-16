# Python-Platformer

This is a reworked version of https://github.com/techwithtim/Python-Platformer.  
I didn't have a goal to make complete game, just studing pygame library, so this code is a prototype, nothing more.  
I've found the tutorial on techwithtim youtube channel, and started to playing around it.  
The main problem I've bumped with, was the collision detection. Running animation consists of jump phase and landing phase,  
and in jumping phase sprite collision detects that he is not touching block and start falling - increase Y position.  
Then in landing phase you get a collision just by change to next sprite, and this treated by X movement as a collision,  
and code doesn't change X position. This is easy to see, if add delay when get X collision, and run left and right. 
  
I spent a few days to develop another collision algorithm which is based on vector orientation (simple check dx vs dy of two object centers), and seems it works good.  
Also I’ve created more useful class structure with methods, which allows to add user-defined objects and their behavior  
Added map load/save, and editor mode (press ‘E’ to toggle between game and edit modes)  
Added music / sound effects, HP, damage from traps and healthy fruits 😊
