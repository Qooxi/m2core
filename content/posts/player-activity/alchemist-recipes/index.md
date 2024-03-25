---
title: "Alchemist Research"
date: 2024-03-22T17:04:00+06:00
description: Introduction to Sample Post
price: 150
discount: 50
menu:
  sidebar:
    name: Alchemist Research
    parent: player-activity
    identifier: alchemist-recipes
    weight: 10
tags: ["Player", "Activity"]
categories: ["Activity"]
hero: images/main-photo.png
---


## Information:
> This system allows you to define any number of required item types for a specific ID. This means that we can utilize the same system with different required items for different NPCs or missions, etc.
> Upon returning the required item, our character will permanently receive its attributes.
## Demonstration
{{< img src="/posts/player-activity/alchemist-recipes/images/demonstration-photo.png" align="center" title="demonstration">}}

## Settings
> The system configuration is in the `.xml` file. You can reload configuration in real time.

```
<Research-Recipes>
	<Recipe npc-vnum="20001">
		<Item main-vnum="178003" chance-vnum="178001" cooldown-vnum="178002"/>
		<Item main-vnum="178004" chance-vnum="178001" cooldown-vnum="178002"/>
		<Item main-vnum="178005" chance-vnum="178001" cooldown-vnum="178002"/>
	</Recipe>
</Research-Recipes>
```

> To make everything clear and easy to set up without unnecessary problems, the configurations responsible for returning a specific item are set in item_proto.
{{< img src="/posts/player-activity/alchemist-recipes/images/settings-proto.png" align="center" title="proto">}}
{{< img src="/posts/player-activity/alchemist-recipes/images/settings-proto-declarations.png" align="center" title="proto-declarations">}}

## Functionality
> Thanks to the flexibility of the system, you can specify for each item:
>- The required quantity of items
>- The chance for accepting the item
>- The cooldown time until the next return of the goods if successful
>- The cooldown time until the next return of the goods in case of failure
>- Required item that increases the chance of acceptance
>- Required item that reduces the cooldown time until the item can be returned again

## Faq
* Can I create a button system instead of an NPC?
	* `Yes`, just connect the appropriate package to open with the correct (ID)
* Can I change the attributes received by a player after completing a mission?
	* `Yes`, all you need to do is change the bonuses in the appropriate item.
* Is there support for the system?
	* `Yes`, for major changes an appropriate fee will be charged.
