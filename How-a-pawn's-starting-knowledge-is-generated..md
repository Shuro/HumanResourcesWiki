The game will generate a pawn's expertise when it is first spawned following these rules. Two lists are generated: one of _technologies_ and another one for _weapon proficiencies_.

> _Human Resources_ generates a number of things based on data collected automatically from all available research projects and weapons, so every modded content is taken into consideration. This process is far from perfect though, and there might be inconsistencies and even errors with content that strays too far from vanilla standards. If you notice anything that could be improved, please let us know. The complete record for this data collection at startup and later use can be found in your game log, with entries marked with [HumanResources]. Turn on "verbose logging" for advanced details.

### Technology expertise
First, all technologies are classified according to their affinity with the basic skills ~~based on what kinds of things they unlock and what their descr~~ **using magic**.

The number of techs a pawn knows when he is created is based on his faction's tech level:
* Neolithic and Medieval: 3
* Industrial: 2
* Spacer or higher: 1

If his faction is undefined, the game guesses it from the pawn's background info.

If his highest skill is intelectual and at least level 7, there is a chance he gets assigned one tech that's one level higher than his own.

**If the pawn is a player's colonist, the pool of technologies for this process might also include the faction's starting technologies, those added on the scenario or even ignore the faction tech level entirely, depending on the chosen settings.**

That number is modified by the following factors:
* if the pawn's age is past half his life expectancy, +1
* if the pawn is not an adult, according to the game's classification, -1 up to -3 (for babies)
* if his highest skill is shooting or melee, -1 (because he gets on weapons)

Then, these slots are filled according to the pawn's skills: 
1. A technology related to his highest skill.
2. A technology related to his second-highest skill,
3. From there, random technologies from the selected pool until all slots are filled.

In case of a tie between skill levels, the passion levels break it.

There's usually no techs related to the _Animal_ and _Social_ skills, so pawns specialized on those get random technologies instead.

### Weapon proficiency
The weapons list is much more straightforward. Pawns get:
1. **All the commom weapons**, things like beer, elephant tusks, orbital targeters and those weapons that aren't locked behind some technology (with some exceptions, mostly Royalty and other modded weapons that were patched in)
2. **Weapons he knows how to craft**, according to his tech expertise
3. **If his highest skill is _Shooting_, all ranged weapons** from his tech level (or, for the player's colonists and according to the chosen settings, all ranged weapons included in the scenario).
4. **If his highest skill is _Melee_, all melee weapons** from his tech level (or, for the player's colonists and according to the chosen settings, all melee weapons included in the scenario).
5. If he is a player's colonist and this setting is selected, **all weapons included in the scenario** (not default).
6. If he is a NPC, the weapon he is carrying.