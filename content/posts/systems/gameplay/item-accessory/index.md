---
title: "Item Accessory"
date: 2024-03-22T17:04:00+06:00
description: ---
price: 100
menu:
  sidebar:
    name: Item Accessory
    parent: gameplay
    identifier: item-accessory
    weight: 10
tags: ["Gameplay", "Player", "Items"]
categories: ["Gameplay"]
hero: images/main-photo.png
---


## Information:
> The rewritten version of accessories for items significantly facilitates their management and, above all, offers many more possibilities. From now on, we can create conversions of the same type and in a straightforward configuration specify which items we can place them on.

## Demonstration
{{< img src="/posts/systems/gameplay/item-accessory/images/demonstration-photo-accessory.png" align="center" title="demonstration">}}
{{< img src="/posts/systems/gameplay/item-accessory/images/demonstration-photo-item.png" align="center" title="demonstration">}}

## Settings
> The entire configuration takes place in the item_proto of the accessory. The settings available for adjustment include:
>- items that can be equipped,
>- the percentage we receive,
>- duration of the conversion.

```
#ifdef __RENEWAL_ACCESSORY_SYSTEM_ENABLE__
	// ACCESSORY items
	// Values from 0 - 2 are responsible of vnums that we can put them in
	ITEM_VALUE_ACCESSORY_MULTIPLER = 3,
	ITEM_VALUE_ACCESSORY_TIME = 4,
	ITEM_VALUE_ACCESSORY_TYPE_PERMAMENT = 5,
#endif
```

{{< img src="/posts/systems/gameplay/item-accessory/images/settings-proto.png" align="center" title="proto-declarations">}}

## Functionality
> The system is configurable and has been changed in many ways, including:
>- From now on, you can equip items with various conversions (if possible). This means that we can, for example, insert Ebonite (I) - 5% bonus, Ebonite (II) - 10%, etc.
>- Each accessory individually has its own time which runs in real-time from the moment of insertion.
>- There is a possibility to set a permanent accessory.
