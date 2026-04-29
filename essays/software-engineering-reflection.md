---
layout: essay
type: essay
title: "Software Engineering"
# All dates must be YYYY-MM-DD format!
date: 2026-04-29
published: true 
labels:
  - Reflection
  - Coding Standards
  - Functional Programming
---
<div class="d-flex justify-content-center gap-3">
  <img width="200px" class="rounded" src="../img/computer.jpg">
  <img width="200px" class="rounded" src="../img/computer.jpg">
  <img width="200px" class="rounded" src="../img/computer.jpg">
</div>


## Introduction
Software engineering has much more to offer than just coding; it is a discipline that utilizes engineering solutions to develop software. Mastering these concepts requires more than just the theory, it demands hands-on applications to recognize patterns in the codebase. Throughout the enhancement of my software development skills, I explored valuable topics related to software engineering. I developed my skills through athletic programming, which focuses on high repetitions to quickly produce quality results under pressure. Utilizing workouts of the day (WODs) to enhance and understand concepts that covered important factors such as coding standards and functional programming. I developed my software engineering skills using web application development to explore important computer engineering topics. By drawing connections to other applications of software engineering, I gained a clearer understanding of their purpose, demonstrating that these core principles are universal in software applications. The following sections explore how these core principles apply to software applications.

## Coding Standards
Coding standards are used in any programming language that appears in any software engineering and computer science work. The understanding of how your work should be structured is a common practice that any programmer should possess. Coding standards are the blueprint of how code should be structured so it is readable, maintainable, and clean. The standard is imperative to all programmers due to its ability to allow anyone to read any type of code and understand the code. In order to implement these standards, I utilized ESLint, a code analysis tool that implements coding standard enforcement, best practices, and style. The uniformity ensures that, while working in a team, the codebase remains understandable. While I practiced my skills in web application development, coding standards will appear and be a common practice within any form of coding. The standards for each application may differ, but overall will serve the same purpose. Testing out my skills in a team project, the coding standards became vital. This uniformly allowed the modules of the project to merge seamlessly. Coding standards are the blueprint for writing code to allow programmers to design projects in groups, updating code, and reviewing all code not only applied to software engineering, but all disciplines. In practice, I used the linter, Airbnb style, in which the style in web application design is shown below:
```tsx
/* Renders a single note in the List Notes table. See list/page.tsx. */
const NoteItem = ({ note }: { note: Note }  ) => (
  <ListGroup.Item>
    <p className="fw-lighter">{note.createdAt.toLocaleDateString('en-US')}</p>
    <p>{note.note}</p>
  </ListGroup.Item>
);
```

## Functional Programming
A significant practice that was explored in my software engineering journey was functional programming. Functional programming is a programming paradigm that utilizes the functions for creating reusable code. It fits perfectly into the software engineering discipline due to the effect on making code efficient and reusable. The application of pure functions makes code easier to understand, test, and debug. Pure functions are functions that will return the same output with specific input. Through practice with functional paradigms, I gained an understanding that applying logic such as “for” or “while” loops in functions is not always necessary. I utilized the applications of higher-order functions such as map, filter, and sort methods to find solutions, allowing the functions to be used in multiple solutions rather than having a single application. The idea of functional programming does not only exist within web application development, but reaches all coding applications. Functional programming has a large presence in the financial and data processing sectors due to its predictability and lack of side effects. The functionality allows these fields to create precise calculations using a mathematical approach. Functional programming was a unique way to explore software engineering solutions that can be applied across multiple applications to provide reusable solutions. In practice, I created a function to total degrees offered by the University of Hawaii by using functional programming which is shown below:

```tsx
function totalDegrees(data: UhData[]): number{
    return data.reduce(function(sum, item){
        return sum + item.awards;
    }, 0)
}
```

## Conclusion
Software engineering has taught me valuable applications that expand beyond web application development. While my focus was structured for web application development, I am now equipped with the proper knowledge to utilize these skills across all coding applications. A goal of software engineers is to provide reusable code that is efficient, simple, and understandable. Practicing coding standards allowed me to write code that is easily readable and pairs well with working in group projects. The application of functional programming has equipped me with the skills to be able to write efficient and reusable code that can be applied in multiple settings, rather than just one. I was able to test my learnings through athletic programming to be fast and efficient with the work that I was providing, demonstrating that my knowledge can be used within any application of software engineering. Mastering these fundamentals is just the baseline. The real challenge lies in utilizing these principles  