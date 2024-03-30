---
title: "Collectioner"
date: 2024-03-22T17:04:00+06:00
description: ---
price: 200
menu:
  sidebar:
    name: Collectioner
    parent: player-activity
    identifier: collectioner
    weight: 10
tags: ["Player", "Activity"]
categories: ["Activity"]
hero: images/main-photo.png
---


## Information:
> The system involves handing in the required items for a specific category. Upon handing in all the items, we receive a reward in the form of a bonus.

## Settings
> The system configuration is in the `.xml` file. You can reload configuration in real time.

```
<Collection-Items>
    <Collect name="TEST">
        <Applies>
            <Apply type="MAX_HP" value="500"/>
            <Apply type="MAX_SP" value="200"/>
        </Applies>
        <Requirements>
            <Item vnum="27102" count="5"/>
            <Item vnum="27105" count="3"/>
            <Gold amount="100000"/>
        </Requirements>
    </Collect>

    <Collect name="TEST2">
        <Applies>
            <Apply type="MAX_SP" value="500"/>
        </Applies>
        <Requirements>
            <Item vnum="27105" count="5"/>
            <Item vnum="85001" count="2"/>
            <Item vnum="71041" count="1"/>
            <Gold amount="100000"/>
        </Requirements>
    </Collect>
</Collection-Items>

```
