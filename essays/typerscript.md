---
layout: essay
type: essay
title: "Typescript: A New Approach"
# All dates must be YYYY-MM-DD format!
date: 2026-01-25
published: true
labels:
  - Javascript
  - Typescript
---
## Introduction into Typescript

The introduction into Typescript has helped me boost my confidence and knowledge in a different programming language. After the first two weeks of practicing Typescript, I now have started to gain a grasp on the new language. I have had no prior experience in Typescript or even Javascript. This presented a challenge for me at the beginning of this semester due to the fact I am inexperienced in the Typescript language and have not programmed for over two years. In fact, the only two languages that I have learned in my studies include Java and C. So, at the start of the semester the ES6 learning module was a great refresher back into programming and quick tutorial to learn the basics into Typescript. From a software engineering perspective, I believe that Typescript is a great tool for software engineering due to the ability to set and see what type a function returns. This feature has helped me tremendously with having a guideline for when I am writing my code.

## Athlectic Software Engineering 

A key idea we are learning this semester is athletic software engineering. This process is a timed, fast- paced approach to completing assignments in an allotted amount of time. More often than not, these assignments usually require multiple attempts to achieve a certain timeframe. I have mixed feelings about this approach for learning software engineering. While I do enjoy the smaller fast paced assignments, it provides a challenge for someone who isn’t familiar with Typescript. This learning style is unforgiving when you aren’t totally sure how to do the assignment you are tasked with completing, by the time you establish how to complete a task you may be almost out of time. As a person who likes to learn from trial and error, the athletic approach is not a learning style that I care for. I like to see my mistakes and learn from them. While I can do  this from multiple attempts, the amount of time it takes does add up. The athletic software engineering approach could get a different outlook once I have gained experience in Typescript, but as a beginner this approach has not been enjoyable.    

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
The code shows a Store class that places an order if there is enough inventory.
