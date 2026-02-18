---
title: Halo 4
nav_title: Halo: 4
description: Halo 4 speedrunning hub with category context, core techniques, and links to level guides.
game: Halo 4
series: Halo

og_image: og.webp
square_image: square.webp

platforms:
  - PC
  - Console
leaderboard: https://haloruns.com/leaderboards/h4/solo/fullgame/Easy
discord: https://haloruns.com/discord
order: 16
timing_method: Varies by category
downpatch: sometimes
allowed_versions: "Depends on category"
where_to_buy: "Steam / Xbox Store"
---

Halo 4 is a very glitchy game, much like Halo 2. It is very easy to get out-of-bounds, although OoB areas are rarely modeled. Objects also despawn quickly and often.

Halo 4 speedrunning is still unoptimized and the game has a lot of potential yet to be found.

Halo Runs record page: <http://www.haloruns.com/records?lb=600> (click the timestamps for video links)

## Level Strategies

- [Dawn](levels/dawn/index.md)
- [Requiem](levels/requiem/index.md)
- [Forerunner](levels/forerunner/index.md)
- [Infinity](levels/infinity/index.md)
- [Reclaimer](levels/reclaimer/index.md)
- [Shutdown](levels/shutdown/index.md)
- [Composer](levels/composer/index.md)
- [Midnight](levels/midnight/index.md)

## Movement Techniques

### Box Launching (Gravity Hammer)

{{#Widget:YouTube\|id=VPeyV0nv3mM\|right\|caption=Box launching with the hammer in H4.}} {{#Widget:YouTube\|id=niFxeoBBXRE\|right}} It is now harder to use it for horizontal distance though it is easier to gain vertical distance. There aren't very many opportunities for box launching, as the Gravity Hammer only spawns on the last mission, Midnight. [This](http://www.youtube.com/watch?v=_Duu2_UgWIg#t=10m14s) is arguably the best use for it in the entire mission.

### Grenade Jumping

Halo 4's grenade jumps are significantly less consistent than other games in the series.

### Muscle Running

Muscle Run Analysis by EightBitNacho

The "muscle run" is a technique used in Halo 4 to extend the amount of time sprint can be used. Since sprint is not unlimited, the idea is to jump and melee at a certain point while sprinting - meleeing cancels the sprint to make it start recharging, and jumping carries the sprint momentum, allowing what seems like infinite sprint. With proper execution it seemed faster, so I tested it properly to find some kind of "sweet spot" that saved the most time.

To do this, I created a long flat running track in Forge and timed myself running from one side to the other, repeating this six times for each test. The techniques I tested are as follows:

NORMAL: Sprint normally, walk while recharging, then sprint again when ready. MUSCLE: Sprint, jump/melee after a certain length of time, repeat. CANCEL: Sprint, jump/cancel after a certain length of time, repeat.

The idea behind CANCEL was to see if meleeing has any effect. Cancelling simply means pressing the sprint button again to stop the sprint.

With MUSCLE and CANCEL, I ran with a Covenant Carbine and counted the cycles the gun makes as Master Chief runs. When sprint is first pressed, then gun drops immediately, then begins to bob up and down. After the initial drop, I counted the "dig" animations, which you can plainly see if you try this yourself. The cycles I tested were 1 dig (~0.85s), between 1 and 2 (~1.15s), 2 digs (~1.45s), between 2 and 3 (~1.75s), and 3 digs (~2.05s). The amount of time between pressing sprint and meleeing/cancelling is in brackets.

<hr>

The results are as follows:

TYPE DIGS AVG TIME

NORMAL --- 27.49 s

MUSCLE 1.0 28.93 s MUSCLE 1.5 27.67 s MUSCLE 2.0 26.87 s MUSCLE 2.5 26.57 s MUSCLE 3.0 27.03 s\*

CANCEL 1.0 29.10 s CANCEL 1.5 28.05 s CANCEL 2.0 27.15 s CANCEL 2.5 26.59 s CANCEL 3.0 27.08 s\*

- Sprint ran out during testing.

<hr>

What these results mean is:

Normal sprinting is fast enough that people who can't nail the muscle run are only at a very small disadvantage, but a disadvantage nonetheless. Muscle running is more effective the longer you wait between cycles, but if you wait too long, you don't give the sprint enough time to recharge and it runs out. This means that muscle running over long distances should never have cycles longer than 2.5 digs to conserve sprint, but shorter distances can have longer cycles because sprint won't run out. Also, the more time spent in the air, the more sprint gets recharged. Muscle running downhill can have longer cycles; conversely, muscle running uphill should have shorter cycles. For some odd reason, cancelling seems to become more effective the longer the cycles are (compared to meleeing). At its most optimal it becomes equal to meleeing, so there's no need to ever use cancelling.

tl;dr - To run at optimal speed, jump and melee 1.7 seconds after hitting sprint, then continue sprinting as soon as you land. Repeat.

### Spring Jump/Super Jump

Jump then crouch while in midair, for some reason some of Chief's jump height is saved in the crouch. After landing, crouch and jump at same time and there will be extra height to the jump allowing places that originally cant be reached to be reached (Not used for full game runs).

## Enemies

Halo 4 added a new race of enemies called Prometheans. They are basically like Tron robots that tend to be bullet sponges.

### Promethean Knights

Knights often use Suppressors and LightRifles. They are capable of teleporting and have an absurdly fast shield recharge rate. They often use teleport to give their shields time to recharge. They lack a visual cue for shield damage unlike Elites, which can make them unpleasant to fight. They are a little harder to fight in close combat. They can deploy Watchers from their carapace, although this is usually scripted. Knights have three variants.

Knight Lancers are similar to normal Knights, but they use teleport more frequently. They possess a distinctive zig-zag charge attack, which is very predictable, easily avoidable, and rarely used. They usually deploy an Auto-Sentry. There are a few instances of Lancers wielding a Binary Rifle, these apparently have Promethean Vision and are extremely dangerous.

Knight Battlewagons have orange spikes on their back. They are similar to normal Knights, but they are harder to approach due to their Scattershot. Besides that, the only thing you have to worry about is their unique jump attack, which is also rarely used.

Knight Commanders are fiery in appearance and almost always have an Incineration Cannon. They possess an overpowered explosive jump which can be devastating. They can also fire off shots during this jump.

### Watchers

Imagine every Drone/Engineer having a fast recharging shield, a lot of health, a bottomless clip rifle, deflecting grenades thrown at them or their allies, and being able to shield each other or their allies. Then imagine them having a ridiculously small and strange hitbox, being able to move very quickly, and having a high tendency to flee or randomly fly around when engaged. They can resurrect their dead commanders. They will swarm you at every waking moment; cover is rarely an option so keep your distance when you can. They are very spammable, although this is rare in Campaign.

Generally, they should be prioritized first.

Anti-Watcher tactics:

- Sometimes, all you have do is kill a single Knight and every Watcher in the vincinity will naively vie for the task of resurrection, becoming extremely vulnerable
- It's very easy to sprint/jetpack past when there's only a few of them flying around. Some Watchers will spawn with a scripted task in mind i.e. spawn a Promethean turret, giving you ample amount of time to engage or run past them
- Also, if you have an automatic weapon, you can send them packing with a few bursts, giving you enough time to take out a bunch of Crawlers or a Knight
- They can be quickly taken out with ranged precision rifles, especially snipers. With the main rifles, it only takes 3-5 precise shots to their eye, which has a ridiculously small hitbox

### Crawlers

Essentially Skirmisher reincarnate, but with less health, agility, and responsiveness. They are easily taken out with headshots but melee can keep them at bay. Just watch out for the Crawler Snipe - they are essentially mobile Jackal snipers.
