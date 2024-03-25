---
title: "Marble Creator"
date: 2024-03-22T17:04:00+06:00
description: --
price: 150
discount: 50
menu:
  sidebar:
    name: Marble Creator
    parent: player-activity
    identifier: marble-creator
    weight: 10
tags: ["Player", "Activity"]
categories: ["Player-Activity"]
hero: images/main-photo.png
---


## Information:
> The system allows you to accept a mission thanks to which, after killing the appropriate number of monsters, you will receive a polymorph marble.
{{< alert type="danger" >}}
It is possible to further develop the system, allowing us to get additional items from the player before accepting the mission using a special "Remote Refine" window.
{{< /alert >}}

## Demonstration
{{< img src="/posts/player-activity/alchemist-recipes/images/demonstration-photo.png" align="center" title="demonstration">}}

## Settings
> The system configuration is in the `.xml` file. You can reload configuration in real time.

```
<Marble-Creator>
    <Monster vnum="636" count="100"/>
    <Monster vnum="2002" count="100"/>
</Marble-Creator>

```

## Functionality
- Turning on the window can be done using a button or by talking to a special NPC.
- You can only have one mission active at a time.
- You can cancel a mission at any time.
- After completing the mission, you have to wait some time to start it again, so it makes sense to produce more marbles right away.
- To be able to constantly track the progress of your mission, an additional window with special information is displayed in the taskbar

## Faq
* Can I change the attributes received by a player after completing a mission?
	* `Yes`, all you need to do is change the bonuses in the appropriate item.
* Is there support for the system?
	* `Yes`, for major changes an appropriate fee will be charged.
