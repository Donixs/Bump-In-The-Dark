---
NoteIcon: City
NoteType: pf2eSettlements
alias: Crown of Ustalav
tags: 
  - pf2e/trait/alignment/lawfulneutral
  - pf2e/trait/government/monarch
  - pf2e/settlement/level/20
statblock: inline
name: "Caliphas"
Pronounced: Kal-LI-phas
Location: Caliphas
Type: Capital
Region: 
- Caliphas
- Ustalav
- Eye of Dread
- Avistan
GovtType: Monarchy
Defences: Seaside, Stone Walls
---

%% This file requires SlRvb's [ITS Callouts Script](https://github.com/SlRvb/Obsidian--ITS-Theme/blob/main/Guide/Callouts.md) %%



> [!infobox]
> # `=this.file.name`
> **Pronounced:**  "`=this.Pronounced`"
> ![[UstalavCaliphasEmblem.png|cover hsmall]]
> ###### Info
> Type |  Stat |
> ---|---|
> **Alias** | `=this.alias` |
> **Type** | `=this.type` |
> **Theme** | Gothic Horror |
> **Region** | `=link(this.Region)` |
> ###### Politics
> Type |  Stat |
> ---|---|
> **Ruler(s)** |Crowned Prince  [[Aduard Ordranti III]]|
> **Leaders** | [[Carmilla Caliphvaso]] |
> **Govt Type** | `=this.GovtType` |
> **Defenses** | `=this.defences` |
> ###### Commerce
> Type |  Stat |
> ---|---|
> **Imports** | Grain, Coal, Spices, Books, Coffee, Tea, Ore|
> **Exports** | Wine, Perfume, Books, Art, Fish, Fashion, Textiles, Literature, Precious Metals|
> ###### Groups
> [[🔰 Group Database|Add New Group]]
> ```dataview
table Type
WHERE contains(Location, this.file.name) AND contains(NoteIcon, "Group")

# **`=this.file.name`**
> [!info|bg-c-purple]- Overview 
> Obsessions, traditions, innovations, and ambitions crash in a storm of secrets over Caliphas, the capital of the Immortal Principality of Ustalav. Over the ages, the fog has lifted from a certain rugged harbor on the northern shore of Lake Encarthan to reveal wildly differing scenes—a rugged trade outpost, a bastion of the dead, a hotbed of discord, and, today, a cultural war zone. Here the beliefs, goods, and wealth of southern Avistan besiege the staunch, provincial traditionalism of Ustalav. Whether through insight or manipulation, the royal court left the nation’s historical seat of power in Ardis 30 years ago, relocating to be among the rising merchant families and powermongers of Caliphas. 
> Since then, the city has known wealth, prestige, and growing arrogance. Today, under the thick fogs and regular storms that are as much a part of the city as its crowded streets, steeple like spires, and treacherous nobility, Caliphas is a city that promises grandeur, but only for a select few. For those without the titles, talent, or wealth to win the city’s fickle affections, Caliphas remains a labyrinth of crime, corruption, disease, exploitation, and horrifying secrets, where lives are cheap and the unwary are all too often swallowed by the fog, never to be seen again.

## Map
> ```leaflet
> id: Capital_Caliphas
> image: [Caliphas.webp]
> lock: false
>bounds: [[0,0], [3670.79, 4766.53]]
>height: 900px
>width: 95%
> lat: 1835.39
> long: 2383.27
> minZoom: -2
> maxZoom: 2
> defaultZoom: -2
> unit: feet
> scale: 1
> darkMode: false
> ```

## Notable Locations

> [!info|bg-c-purple]- Districts
[[Ashtown]] - [[Castle Balatz]], 
[[Blackwood]] - [[Palace of Voices]]
[[North Cushing]] -[[Whiteshaw]]
[[West Cushing]] - [[Maiden's Choir]]
[[Dowell]] - [[Traitor's Drop]], [[Barragaro Road]], [[Brookman's Alley]], [[The Seventh Eye]]
[[Eskcourt]] - [[The Majesty]], [[Restoration Park]], [[Castle Stryithe]]
[[Hawthorne Rows]] - 
[[Laurelight Hill]] - [[Lethean Manor]], [[Havenguard Lunatic Asylum & Vodvani Pathfinder Lodge]], [[Castle Borgoffi]]
[[Leland]] - [[Castle Golbanze]], [[The Reaping Rock]]
[[Valope]] - 

> [!info|bg-c-purple]- Boroughs
> [[Crossleigh]] - [[Dalliance]], [[The Quarterfaux Archives]], [[Mists and Dreams]]
> [[Graystone]] - [[The Cairns]],   [[The Hound's Tooth]], [[Haraday Theater]], [[Castle Mashir]] 
> [[Wrenhyde]] - [[Crown and Carriage Livery Yard]], [[Dawngrace Memorial]] 

> ###### Notable Shops/Services
> [[💲 Shop & Service Database|Add New Shop/Service]]
> ```dataview
table Type, AffiliatedGroup, District
WHERE contains(Location, this.file.name) AND contains(NoteIcon, "Shop")
SORT Type ASC

> ###### Notable Points of Interest
> [[❓ POI Database|Add New Point of Interest]]
> ```dataview
table Type, AffiliatedGroup, District
WHERE contains(Location, this.file.name) AND contains(NoteIcon, "POI")
SORT Type ASC

## Notable Characters

> [[👨‍👩‍👧‍👦 NPC Database|Add New NPC]]
> ```dataview
table Gender, Ancestry, Age, Occupation, AssociatedGroup, AssociatedReligion
WHERE contains(Location, this.file.name) AND contains(NoteIcon, "Character") AND !contains(Condition, "Dead")
SORT choice(Type = "Player", "1", choice(Type = "VIP", "2", choice(Type = "Hostile", "3", choice(Type = "Family", "4", choice(Type = "Friend", "5", choice(Type = "NPC", "6", "7")))))) ASC

## History
TBD

## Statblock
```statblock
columns: 1
forcecolumns: true
layout: Path2eSettlements 
statblock: true
name: "Caliphas"
level: "Settlement 14"
alignment: "LN"
trait_01: "City"
description: "The mist-shrouded capital of Ustalav."
image: "[[UstalavCaliphasEmblem.png]]"
government: "Crownded Prince (Overlord)"
population: "15,640 (14,950 humans, 350 dwarves, 220 elves, 120 other)"
languages: "Common, Varisian, Taldor"
religions: "Pharasma, The Whispering Way"
primimp: "Grain, Coal, Spices, Books, Coffee, Tea"
primexp: "Wine, Perfume, Books, Art, Fish, Fashion, Textiles, Literature"
threats: "Aberrant Horrors, Vampiric Courts ruling from the shadows, eerie hauntings, "
characteristics: 
- name: "Insular People"
  desc: "The people of [[Caliphas]] are suspicious of outsiders and slow to trust. This doubles the time it takes to gather information and increased the DC by 1."
npcs: 
- name: "Aduard Ordranti III"
  desc: "(LN male human)  Crowned Prince "
- name: "Countess Carmilla Caliphvaso"
  desc: "(LE female human) Aristocrat"
- name: ""
  desc: ""
- name: ""
  desc: ""

sourcebook: ""
```
## DM Notes
### Plot Hooks


### Hidden Details


### General Notes