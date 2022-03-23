# Dark Souls 3 Cheat Sheet

To view the cheat sheet [click here](https://azy2.github.io/Elden-Ring-Intended-Route/).

This checklist was created by adopting the source code from the [Dark Souls 3 Cheat Sheet](https://github.com/ZKjellberg/dark-souls-3-cheat-sheet) created by [ZKjellberg](https://github.com/zkjellberg).

The walkthrough is thanks to [Athrek](https://www.reddit.com/r/Roundtable_Guides/comments/tiouti/guide_to_the_intended_route_through_the_game/).

## Contribution Guide

If you are interested in contributing to this guide, I welcome Pull Requests.

All entries in a checklist are stored in data.yaml.

Each page of the site starts like this:
```yaml
---
title: "The Page Title"
id: page_title
sections:
```

Eeach section on a page starts like this:
```yaml
  -
    title: Section Title
    id: section_title
    num: 1
    items:
      - [1, "f_boss", "Boss fight info goes here"]
```

All ids haveto be unique and the `num:` field also has to be unique. Within an item the first number has to be uinque as well. If you are adding a new line find the biggest number in that section and increase it by 1. The numbers do not have to be in order and you should not ever change an existing number because it will break everyones saved progress.

The second field in an item (`"f_boss"`) is used for the filtering system. The full list of filter classes is:

| Class   | Description |
|---      |--- |
| f_boss  | Boss fights |
| f_miss  | Content that can be permanently missed |
| f_npc   | NPC side quests |
| f_estus | Estus Shards |
| f_bone  | Undead Bone Shards |
| f_tome  | Sorcery Scrolls, Pyromancy Tomes, and Divine Tomes |
| f_coal  | Coals |
| f_ash   | Umbral Ashes |
| f_gest  | Gestures |
| f_sorc  | Sorceries |
| f_pyro  | Pyromancies |
| f_mirac | Miracles |
| f_ring  | Rings |
| f_weap  | Weapons, Spell Tools, and Shields |
| f_arm   | Armor Sets or individual pieces |
| f_tit   | Titanite |
| f_gem   | Gems |
| f_cov   | Covenants |
| f_misc  | *any other items* |

If none of these filter classes match, use `""`, or consider adding a new one.

In addition to the filter classes, there is a second type of classes used to control the visibility of entries based on which playthrough the user is on:

| Class  | Description |
|---     |--- |
| h_ng+  | items hidden on NG+ and beyond, e.g., Ashen Estus Flask |
| s_ng+  | items shown on NG+ and beyond, e.g., +1 rings |
| s_ng++ | items shown on NG++ and beyond, e.g., +2 rings |
