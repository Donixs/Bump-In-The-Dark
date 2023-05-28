---
noteType: pf2eSettlement
aliases: "{{{name}}}"
tags: {{#each traits}}{{#if (test this (toRegex "^(aberration|dream|time|humanoid|animal|astral|beast|dragon|fey|fiend|spirit|celestial|construct|elemental|plant|undead|giant|ooze|fungus|monitor|petitioner)$"))}}
  - pf2e/creature/type/{{this}}{{/if}}{{/each}}
  - pf2e/creature/level/{{level}}
statblock: inline
name: "{{{name}}}"
level: {{level}}
---

```statblock
columns: 2
forcecolumns: true
layout: Path2eBlock
statblock: true
{{#if source}}source: "{{{source}}}"{{/if}}
name: "{{{name}}}"
level: "{{#if isNpc}}NPC {{else}}Creature {{/if}}{{level}}"
{{#each traits}}
{{#if (test this (toRegex "^(lg|ng|cg|ln|n|cn|le|ne|ce)$"))}}
alignment: "{{uppercase this}}"
{{else}}
{{#if (test this (toRegex "^(rare|uncommon|common|unique)$"))}}
{{{table this "common" "rare_01: \"Common\"" "uncommon" "rare_02: \"Uncommon\"" "rare" "rare_03: \"Rare\"" "unique" "rare_04: \"Unique\""}}}
{{else}}
{{#if (test this (toRegex "^(tiny|small|medium|large|huge|gargantuan)$"))}}
size: "{{capitalize this}}"
{{else}}
trait_0{{add @index 1}}: "{{capitalizeAll this}}"
{{/if}}
{{/if}}
{{/if}}
{{/each}}

sourcebook: "{{#if source}}_{{{capitalizeAll (table (downcase source) "b1" "Bestiary" "b2" "Bestiary 2" "b3" "Bestiary 3" "gmg" "Gamemastery Guide" "botd" "Book of the Dead" "loil" "Lost Omens: Impossible Lands" "apg" "Advanced Player's Guide" "crb" "Core Rule Book" "da" "Dark Archive" "lome" "Lost Omens: The Mwangi Expanse" "som" "Secrets of Magic" "av1" "Abominations Vaults #1: Ruins of Gauntlight" "av2" "Abominations Vaults #2: Hands of the Devil" "av3" "Abominations Vaults #3: Eyes of Empty Death" "fop" "The Fall of Plaguestone" "aoa1" "Age of Ashes #1: Hellknight Hill" "aoa2" "Age of Ashes #2: Cult of Cinders" "aoa1" "Age of Ashes #1: Hellknight Hill" "aoa3" "Age of Ashes #3: Tomorrow Must Burn" "aoa4" "Age of Ashes #4: Fires of the Haunted City" "aoa5" "Age of Ashes #5: Against the Scarlet Triad" "aoa6" "Age of Ashes #6: Broken Promises" "aoe1" "Agents of Edgewatch #1: Devil at the Dreaming Palace" "aoe2" "Agents of Edgewatch #2: Sixty Feet Under" "aoe3" "Agents of Edgewatch #3: All or Nothing" "aoe4" "Agents of Edgewatch #4: Assault on Hunting Lodge Seven" "aoe5" "Agents of Edgewatch #5: Belly of the Black Whale" "aoe6" "Agents of Edgewatch #6: Ruins of the Radiant Siege" "ec1" "Extinction Curse #1: The Show Must Go On" "ec2" "Extinction Curse #2: Legacy of the Lost God" "ec3" "Extinction Curse #3: Life's Long Shadows" "ec4" "Extinction Curse #4: Siege of the Dinosaurs" "ec5" "Extinction Curse #5: Lord of the Black Sands" "ec6" "Extinction Curse #6: The Apocalypse Prophet" "frp1" "Fists of the Ruby Phoenix #1: Despair on Danger Island" "frp2" "Fists of the Ruby Phoenix #2: Ready? Fight!" "frp3" "Fists of the Ruby Phoenix #3: King of the Mountain" "ltiba" "Little Trouble in Big Absalom" "ngd" "Night of the Gray Death" "ooa1" "Outlaws of Alkenstar #1: Punks in a Powder Keg" "ooa2" "Outlaws of Alkenstar #2: Cradle of Quartz" "ooa3" "Outlaws of Alkenstar #3: The Smoking Gun" "sot1" "Strength of Thousands #1: Kindled Magic" "sot2" "Strength of Thousands #2: Spoken on the Song Wind" "sot3" "Strength of Thousands #3: Hurricane's Howl" "sot4" "Strength of Thousands #4: Secrets of the Temple-City" "sot5" "Strength of Thousands #5: Doorway to the Red Star" "sot6" "Strength of Thousands #6: Shadows of the Ancients" "sli" "The Slithering" "tio" "Troubles in Otari")}}}_{{#if page}}, page {{page}}{{/if}}{{else}}_Pathfinder_{{/if}}."
```