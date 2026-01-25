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
## Introduction into Typescript
The introduction into Typescript has helped me boost my confidence and knowledge in a different programming language. After the first two weeks of practicing Typescript, I now have started to gain a grasp on the new language. I have had no prior experience in Typescript or even Javascript. This presented a challenge for me at the beginning of this semester due to the fact I am inexperienced in the Typescript language and have not programmed for over two years. In fact, the only two languages that I have learned in my studies include Java and C. So, at the start of the semester the ES6 learning module was a great refresher back into programming and quick tutorial to learn the basics into Typescript. From a software engineering perspective, I believe that Typescript is a great tool for software engineering due to the ability to set and see what type a function returns. This feature has helped me tremendously with having a guideline for when I am writing my code.

## Athlectic Software Engineering 

An example from Typescript code from the latest assignment: 
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
