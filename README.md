# IonTech's Modular Systems

Modular Systems and Logic for use in the MythicMobs plugin. The original intent of this project was to centralize commonly used gameplay logic for minecraft servers into modules, minimizing technical debt and providing a scalable foundation for MythicMobs enthusiasts to build upon. I cannot say if I succeeded or failed in that regard. 

Likely a bit of both. This pack contains "modules" that act as which take in inputs via Skill Parameters to handle complex behavior. Every Module is designed to integrate with all other Modules, allowing for complex behaviour by nesting modules within each other.

### Disclaimers:
 Requires at basic understanding of MythicMobs for effective use. 
 Very little documentation is provided, with some comments. Working examples and applications are provided. 
 Primer to advanced MythicMobs usage. Welcome to Wonderland. 

## Input Handlers

  ### Weapon Movesets 
  - Create flowing attack comboes that integrate perfectly into vanilla
  - Can read vanilla hit types and perform the associated skill bound
  - Practical examples provided for reference

  ### Click Comboes
  - Logic for Wynncraft-style click combination casting
  - e.g. LLL, RRR, SWAP+DROP, etc. Bind any skill you want to each combination
  - Easy to use, with examples provided

  ### Spell Cycling
  - Attaches a Cycling system to items, to bind up to 9 skills for usage
  - Cycle through slots 1-9 with Right-Click / Shift + Right Click
  - Basic example provided
 
  ### Hit Evaluation
  - Component skill to Weapon Movesets.
  - Checks what kind of vanilla hit you have performed, e.g. CRIT, SPRINT, WEAK, etc

## Skill Handlers

  ### Spell Casting Handler 
  - The core of the Modular Skills system. Most logic in this pack integrates directly into this system
  - Handles Spell Casting, Cooldowns, Spell Charges, Casting VFX, Stats / Damage handling and more
  - Plenty of examples provided within Demo Skills

  ### Modifier Handler
  - You can save logic to be called between Skill Trees, and this logic is then executed in a stack upon being triggered
  - This enables the creation of custom Buffs, Debuffs, Modular Skills, stacking stat bonuses and much, much more
  - Most I will say is that Risk of Rain's item system is now feasible to implement in Minecraft
  - Note: Do make sure not to call a modifier within a modifier, you will nuke your server
  
  ### Set Random ID
  - Component Skill for Damage Core
  - Sets a random ID that the Damage Core checks against when dealing damage
  - Setting a new ID for the skill will count as a seperate damage instance instead
  
  ### Damage Core
  - Custom core used for percentage-scaling damage
  - Define damage as percentages of Base Damage, Risk of Rain style
  - Displays Damage Indicators and handles unique damage instances dealt

  ### Knockback Core
  - System for doing consistent, deterministic knockback
  - Unaffected by distance from player -> target
  - Directional knockback can be defined by setting an Origin and a target location before calling this skill (- setvarloc{var=knockback_direction;val=...} )
  - When not defined, this system acts similarly to the Throw mechanic, doing radial knockback.

  ### Melee Core
  - System for simulating Vanilla Melee Mechanics.
  - Acts nearly 1to1 with vanilla in terms of knockback and damage dealt
  - Can be further customized to entirely handle all attacks.

  + Some more things that aren't really used by me, such as Summon handling and Custom Mana.

## Skill Mechanics

  ### Advanced Slashes
  - Handler for creating advanced slash effects
  - Includes option for VFX configuration such as Tapering ends
  - Hitboxes are accurate to the slash VFX, and options are provided to customize the hitbox behaviour.

  ### Projectile Skills
  - Fire multiple projectiles at once in Arcing Spreads, Wide radial barrages and random spreads.
  - Handler included for handling custom projectile piercing / maximum hit count before despawn
    
  ### Custom Stuns
  - While targets afflicted are stunned, they cannot cast abilities through the Spell Handler system.
  - Ongoing casts / channeling are also interrupted 

  ### Vector Mechanics
  - Useful skills for dealing with vectors, such as getting distances, direction, velocity, etc.
  - Best used as reference for creating your own vector handler, rather than being used out of the box. 

  ### Particle Spiral / Shockwave
  - Custom VFX handlers. Useful if you want to enhance your skill casts and add some flair.
  - Very basic examples provided within the skill config. Documentation... not provided. 
  
  ### Custom Healing
  - Definable healing-over-time with an damage taken threshold for interruption
  - Honestly didn't update this much

  ### Insertion Sort
  - It's insertion sort.
  - Don't ask me why I made this, but it's a good reference for the new Meta Variables.

  + More. 

Do have fun, and behold my works. 

