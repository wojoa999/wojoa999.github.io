---
layout: essay
type: essay
title: "Reflection on Typescript"
# All dates must be YYYY-MM-DD format!
date: 2026-01-25
published: true
labels:
  - Javascript
  - Typescript
---
<img width="100px" class="rounded float-start pe-4" src="../img/download.jpg">

```cpp
class Store{
    inventory: Inventory;

    constructor(inventory: Inventory){
        this.inventory = inventory;
    }
    placeOrder(order: Order): Drink[] {
        const retval: Drink[] = [];
        for(let i = 0; i < order.drink.length; i++){
            const drink = order.drink[i];
            if(this.inventory.haveServings(drink.menuItem.ingredients)){
                retval.push(drink);
            }
        }
        return retval;
    }
}
```
