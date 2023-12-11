# 2D-Platformer-Teleporter
Tutorial on how to create teleporters for 2D platformer


1. Create 2 empty sprites and name them teleporter 1 and 2, add a 2D box collider (make sure 'is trigger' is ticked) and create a new script and name it Teleporter (make sure to select both empty sprites so the script applies to them both). Apply a sqaure sprite to the sprite renderer and position both squares on either side of the platform.

![image](https://github.com/MartTQ/2D-Platformer-Teleporter/assets/123513842/6243257d-ce2c-4fdb-8963-ef5fe304aa5e)

![image](https://github.com/MartTQ/2D-Platformer-Teleporter/assets/123513842/99feb86c-2069-45fa-a8db-47148e863c99)
![image](https://github.com/MartTQ/2D-Platformer-Teleporter/assets/123513842/c3549ed3-0209-4b3f-812d-4f75d271321b)
![image](https://github.com/MartTQ/2D-Platformer-Teleporter/assets/123513842/48f581ab-0bf4-495d-8982-92f9af53ba22)

2. Open the Teleporter script and create serializefield to get the 'destination' of the teleporters. Then apply the script to both teleporters as well as the destination to both. 

![image](https://github.com/MartTQ/2D-Platformer-Teleporter/assets/123513842/01f9d504-7dba-453b-9a49-78ee8dc957c2)
![image](https://github.com/MartTQ/2D-Platformer-Teleporter/assets/123513842/fcb17537-6c8b-424a-a050-e342f0057c6c)
![image](https://github.com/MartTQ/2D-Platformer-Teleporter/assets/123513842/cc059e1c-db7d-4194-94ee-87f3b6c735c7)

3. Next create a new script called 'Player Teleporter', open it and we're going ot create a key input in order to use the teleporter (for this instance I am using the 'E' key to activate the teleporter) create an input.GetKeyDown and set it to E, make it so if the player presses down E on a currnent telporter it will transforms the players position.

![image](https://github.com/MartTQ/2D-Platformer-Teleporter/assets/123513842/bde99c73-a6bb-46f7-be10-beda69b479cc)

4. add a OnTriggerEnter2D colloder2D tag to the 'teleporter' so that when applying the 'E' key it will execute the 'transform position'.

![image](https://github.com/MartTQ/2D-Platformer-Teleporter/assets/123513842/83f12400-0913-4a19-a292-b131d624894a)

5. Add OnTriggerExist2D so that the 'gameObject' (the player) will be executed to the final position.
   
![image](https://github.com/MartTQ/2D-Platformer-Teleporter/assets/123513842/2ca6dff0-c1ef-401d-857e-bfff0f03923d)

The complete code for the 'PlayerTeleporter' should be like this:

![image](https://github.com/MartTQ/2D-Platformer-Teleporter/assets/123513842/01f30cef-e703-4202-9d24-f191f277ded3)

6. Finally apply the 'PlayerTeleporter' Script to our player
   
![image](https://github.com/MartTQ/2D-Platformer-Teleporter/assets/123513842/2a82b05c-889f-4533-b3f4-ee7045602d5a)

![image](https://github.com/MartTQ/2D-Platformer-Teleporter/assets/123513842/315c46e9-5c5b-45c5-b981-1d1d87eb2b06)

7. End result should be like this.

https://github.com/MartTQ/2D-Platformer-Teleporter/assets/123513842/abc671b3-37d3-49f7-bff4-cd6f6a7da8f4


