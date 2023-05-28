---
noteType: pf2eMonster
aliases: "The Flesh"
tags: 
  - pf2e/creature/type/abberation
  - pf2e/creature/level/4
statblock: inline
name: "The Flesh"
level: 4
---

```statblock
columns: 2
forcecolumns: true
layout: Path2eBlock
statblock: true
source: "TB"
name: "The Flesh"
level: "Creature 4"
alignment: "NE"
size: "Medium"
rare_03: "Rare"
trait_03: "Fleshwarp"
trait_04: "Amphibious"
trait_05: "Aberration"
modifier: 8
perception:
  - name: "Perception"
    desc: "Perception +8; __darkvision (60ft)__;"
languages: "Aklo, Any Language the Host knows "
skills:
  - name: "Skills"
    desc: "__Survival__: +10 (1d20+10), __Deception__: +10 (1d20+10)"
abilityMods: [5, 2, 5, 2, 2, 2]

abilities_mid:
 - name: "Assume Form"
   desc: "*⬻{ .Pathfinder }* ([[fleshwarp-loag|fleshwarp]], [[manipulate]], [[occult]], [[transmutation]]); The flesh consumes the corpse of a Medium or smaller Humanoid or Beast within 5 feet of it and transforms into that creature. Its statistics, other than its size, are the same in the new form. Any equipment it is wearing or carrying melds into the new form. It can’t activate, use, wield, or otherwise benefit from any of its equipment. It reverts to its true, aberrant form if it dies, makes a Manipulate Flesh attack, or uses Assume Form while transformed."
 - name: "Grab"
   desc: "*⬻{ .Pathfinder }* __Requirements__ The monster's last action was a success with a Strike that lists Grab in its damage entry, or it has a creature grabbed using this action. __Effect__ The monster automatically [[grab|Grabs]]  the target until the end of the monster's next turn. The creature is Grabbed by whichever body part the monster attacked with, and that body part can't be used to Strike creatures until the grab is ended. Using [[Grab]] extends the duration of the monster's Grab until the end of its next turn for all creatures grabbed by it. A grabbed creature can use the [[Escape]] action to get out of the grab, and the Grab ends for a grabbed creatures if the monster moves away from it."
 - name: "Attack of Opportunity"
   desc: "*⬲{ .Pathfinder }* __Trigger__ A creature within your reach uses a manipulate action or a move action, makes a ranged attack, or leaves a square during a move action it's using. You lash out at a foe that leaves an opening. Make a melee Strike against the triggering creature. If your attack is a critical hit and the trigger was a manipulate action, you disrupt that action. This Strike doesn't count toward your multiple attack penalty, and your multiple attack penalty doesn't apply to this Strike. Only slam."
 - name: "Regeneration"
   desc: "*⭓{ .Pathfinder }* This monster regains the listed number of Hit Points each round at the beginning of its turn. Its Dying condition never increases beyond Dying 3 as long as its regeneration is active. However, if it takes damage of a type listed in the regeneration entry, its regeneration deactivates until the end of its next turn. Deactivate the regeneration before applying any damage of a listed type, since that damage might kill the monster by bringing it to Dying 4."

speed: 25 feet

ac: 18
armorclass:
  - name: AC
    desc: "18; __Fort__: +14 (1d20+14), __Ref__: +8 (1d20+8), __Will__: +8 (1d20+8)"
hp: 78
health:
  - name: HP
    desc: "78; regeneration 10 (deactivated by fire or acid); __Immunities__ controlled, emotion"

attacks:
  - name: Melee
    desc: "Slam +14 __Damage__ 2d8+5 (2d8+5) bludgeoning"
  - name: Melee
    desc: "Manifold Bite +12 ([[deadly|deadly d8]]) __Damage__ 2d4+5 (2d4+5) piercing"
  - name: Melee
    desc: "Tentacle +12 ([[grapple]]) __Damage__ 2d6+5 (2d6+5) bludgeoning"
  - name: Ranged
    desc: "Acidic Mucus +12 ([[acid|acid]], [[range increment|range increment 25 feet]]) __Damage__ 2d8 + 1d8 persistent (2d8+1d8) acid"

sourcebook: "Tome of Beasts pg 367"
```