
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
> **Theme** | TBD |
> **Region** | `=link(this.Region)` |
> ###### Politics
> Type |  Stat |
> ---|---|
> **Ruler(s)** | TBD |
> **Leaders** | TBD |
> **Govt Type** | `=this.GovtType` |
> **Defenses** | `=this.defences` |
> ###### Commerce
> Type |  Stat |
> ---|---|
> **Imports** | TBD |
> **Exports** | TBD |
> ###### Groups
> [[🔰 Group Database|Add New Group]]
> ```dataview
table Type
WHERE contains(Location, this.file.name) AND contains(NoteIcon, "Group")

# **`=this.file.name`**
> [!info|bg-c-purple]- Overview
TBD

## Map
> ```leaflet
> id: Region_Ustalav
> image: [[UstalavRegion.webp]]
> lock: false
>bounds: [[0,0], [572.33, 374.93]]
>height: 900px
>width: 95%
> lat: 286.17
> long: 187.47
> minZoom: -2
> maxZoom: 2
> defaultZoom: 1
> unit: miles
> scale: 1
> darkMode: false
> ```

## Notable Locations

> [!info|bg-c-purple]- Counties
TBD

> ###### Notable Cities
> [[💲 Shop & Service Database|Add New Shop/Service]]
> ```dataview
table Type, AffiliatedGroup
WHERE contains(Location, this.file.name) AND contains(NoteIcon, "Shop")
SORT Type ASC

> ###### Notable Points of Interest
> [[❓ POI Database|Add New Point of Interest]]
> ```dataview
table Type, AffiliatedGroup
WHERE contains(Location, this.file.name) AND contains(NoteIcon, "POI")
SORT Type ASC

## Notable Characters

> [[👨‍👩‍👧‍👦 NPC Database|Add New NPC]]
> ```dataview
table Gender, Race, Age, Occupation, AssociatedGroup, AssociatedReligion
WHERE contains(Location, this.file.name) AND contains(NoteIcon, "Character") AND !contains(Condition, "Dead")
SORT choice(Type = "Player", "1", choice(Type = "VIP", "2", choice(Type = "Hostile", "3", choice(Type = "Family", "4", choice(Type = "Friend", "5", choice(Type = "NPC", "6", "7")))))) ASC

## History
Hierarchy of Ranks

Prince/Princess, Count/Countess, Duch/Duchess, Earl, Maruess/Marchioness, Baron/Baroness



## DM Notes
### Plot Hooks


### Hidden Details


### General Notes