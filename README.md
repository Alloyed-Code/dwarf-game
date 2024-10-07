# Dwarf Game (Dwarf's Reclamation)
Delve into the depths of an abandoned dwarven stronghold to find the greatest treasure of all: the Heart of the Mountain. Navigate caverns and collapsed halls while fighting the dungeon's new inhabitants to grab the treasured gemstone and then to escape back to the surface.

Dwarf Game is a top-down tilemap-based 2D Unity game with z-levels. Instead of representing different floors of the map with different scenes or disabling and enabling different tilemaps, each depth level is a separate tilemap that is always active. They are physically at different z-levels in the Unity scene. This allows lower levels to be visible while on higher level.

This does, however, introduce complications of its own. Unity's 2D physics engine does not recognize depth in a scene. Levels the character is not on will still cause collisions and enemies will move and attack as if they were all on the same depth level as the character. To avoid this, almost everything needs a script to manage whether its current floor should be active or have a collider based on what level the player character is on.

## Controls

Movement is controlled by **WASD** or the **Arrow Keys**.

**Tab** lets the Dwarf interact with objects.

**Left-click** will cause the Dwarf to punch in the direction of the mouse cursor.

**Escape** opens the pause menu.
