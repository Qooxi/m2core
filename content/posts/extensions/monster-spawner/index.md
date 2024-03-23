---
title: "Monster Spawner"
date: 2024-03-22T17:04:00+06:00
description: --
price: 150
discount: 50
menu:
  sidebar:
    name: Monster Spawner
    parent: extensions
    identifier: monster-spawner
    weight: 10
tags: ["Extensions", "Gameplay", "Feature"]
categories: ["Extensions"]
hero: images/main-photo.png
---


## Information:
> This solution is designed to alter the respawn timing calculation for individual monsters and to display players the current instance quantity status.
> Depending on the settings in the configuration file, for example, if we set the respawn time for a specific monster to `150 seconds`, it means that from the server `start`, it will respawn exactly every `150 seconds`, for instance: `15:00:00`, `15:01:30`, `15:03:00`, assuming the monster is not being attacked or alive.

## Demonstration
{{< img src="/posts/extensions/monster-spawner/images/demonstration-photo.png" align="center" title="demonstration">}}

## Settings
> The system configuration is in the `.xml` file. You can reload configuration in real time.

```
<Monster-Spawner>
    <Localization map-index="1">
        <Monsters>
            <Monster id="591" x="640" y="700" cooldown="180"/>
        </Monsters>
    </Localization>
</Monster-Spawner>
```
