Zero Tolerance level editor v0.3
(c)2009 FireWing

How to use:

At first, you need a good dump of the game ROM in a .BIN (NOT .SMD!) format.
In case you have an .SMD, you can convert it to .BIN with some utility like
"ROM Converter" (not included, but it's not a big problem to find this or any
similar tool).

Each cell has a hexadecimal value written on it, except empty cells and doors 
(those are same in any episode). Remember that there are 3 episodes in the game,
and each episode has different cell definitions, i.e. player start cell # is 8F
for first episode, but it's F3 for second.
To edit a cell, right-click it and select the cell type from the popup menu.
You can also type in the new value directly.

Another important thing: There are 16 levels in each episode, but not all
of the levels are used in game:
 - Episode 1 has 3 unused levels, for some reason called "REACTOR 2"
   similar to the last playable level.
 - Episode 2 has one unused level, "FLOOR 150".
 - Episode 3 has 4 extra levels, though they all are untitled since there's
   simply no room left in the level name list.

While you can use those to make extra levels, there are some issues:
 - When you reach such a level, a password given wouldn't be valid if you
   try to enter it later.
 - For Episode 3 levels, there's garbage instead of level name displayed
   on the map.

Beyond Zero Tolerance has no unused levels, there are 8 levels for Episode 1,
6 levels for Episode 2 and 10 levels for Episode 3.

Some other things you should know:
 - Obviously, you shouldn't place more than 99 enemies per level since
   enemy counter is only 2 symbols wide.
 - Edges of the map should always be closed with walls.
 - Stairs and elevators should always be surrounded with special walls and
   cells, if you need to place them just check how it's done in original
   levels. Wrong placement will cause rendering glitches or even a game
   crash.
 - Don't place elevators/stairs going up on the first level of any episode.
   This will result in loading an unplayable garbage when you try to use them.
   Same for last level - don't place elevators/stairs going down, place a boss
   instead.

Send feedbacks, questions, feature requests to
firewing15@gmail.com