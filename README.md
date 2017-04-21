# Changelog
## Crises

### General
-Enabled multiple crises to occur. Multiple instances of the same crisis are still disabled.

### Prethoryn Swarm
-Removed 25% chance of swarm not spawning.

-Rescaled crisis start time from 10/20/30/15% for 170/200/250/300 years to 15/25/35/20/5% for 170/200/250/300/350 years.


### Unbidden
-Changed MTTH from 240 months to 1200 months (comment in code said MTTH should be 100 years, but it was set to 20 years). Effectively reduces probability of Unbidden spawning in a non-Jump Drive empire by a factor of 5. Should fix problems with Unbidden always being the crisis encountered.

-Reduced speedup factor of spawn for empires with jump drive from 0.8 to 0.01. Effectively increases probability of Unbidden spawning in an empire with Jump Drive by a factor of 80.


Researching jump drives now practically GUARANTEES Unbidden almost IMMEDIATELY (within a year). Previously the speedup due to Jump Drive was laughably minor; absolutely worst case they would show up 20% faster than normal.



## Fallen Empires
# Fleets
-Removed requirement that Fallen Empire not be at war to create a new fleet

-Increased time to create a new fleet from 1 month to 360 months. 

Note: new fleets still only spawn if total fleet power < 5000.

# War in Heaven
-Increased chance of Awakened Empire having War in Heaven with rival ethos Fallen Empire from 40% to 55%.

-Increased chance of Awakened Empire having War in Heaven with random Fallen EMpire from 20% to 35%.

-Reduced chance of no War in Heaven post-Awakened Empire from 40% to 10%.




# Disabling changes

## Vanilla Swarm Spawn Probabilities/Remove Risk of No Swarm Spawn
Delete game_start.txt


## Set own Swarm spawn timers/probabilities
Line 255 of game_start.txt. For a probability of no swarm spawn, make one entry x = {} where x is a number, the probability of no spawn happening.


## Vanilla Unbidden Jump Drive Risk
Change line 55 and line 60 of crisis_events_2.txt to "factor = 0.8"


## No Fallen Empire Fleet Respawn
Delete fallen_empire_events.txt


## No War In Heaven Changes
Delete fallen_empire_awakening_events.txt




