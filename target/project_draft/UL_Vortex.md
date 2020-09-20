# UL Vortex (Unlight Zwei)


## Scope / Aimming (for resolving phase 1 project)

1. resolve data / class structure 
    1. do the review
    2. user / player structure 
      ```protoc
      enum    PlayerSide  {
          HOST                        = 0;
          DUELER                      = 1;
          // watcher                  = 2;
          // add 'watcher' defination, instead of if-else to make me confuse
      }
      ``` 
    3. Event-phase / action-phase
        - still claos for understanding

<!-- slide -->
2. Unity System
   1. Use Job-scheduling, instead of mono-game-object 
      1. hard for central controlling
      2. performance, e.g. Action-Card rendering 
   2. complete skill-calculation part
      1. rewrite calculator into Unity ??
      2. keep it in nodejs??
   3. complete game-phase?
<!-- slide -->

3. Redefine the system arch
   1. define
      1. no more centralize design
      2. consider client-side PC minimum ability
      3. both-side pc need trust,
      4. submit log.
   2. auth and personal data
      1. firebase ?
      2. discord auth ?
         1. personal data storage : discord.com/developers/docs/game-sdk/storage
         2. signal , get player ip 

   3. story system (RPG mode)
      1. need someone to write new story log
      2. AVG game UI!
      3. 