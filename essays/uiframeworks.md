---
layout: essay
type: essay
title: "UI Frameworks"
# All dates must be YYYY-MM-DD format!
date: 2026-02-18
published: true
labels:
  - HTML
  - CSS
  - Bootstrap 5
---
<div class="text-center p-4">
  <img width="300px" src="../img/html.jpg" class="img-thumbnail" >
</div>

## My Experience with UI Frameworks

Over the past few weeks, I have become familiar with UI frameworks using HTML, CSS, and Bootstrap 5. As a complete newcomer to these tools, my outlook may differ from someone with more experience. To me, it felt like learning an entirely new programming language. However, the use of classes was a new concept that I picked up on quickly. In this essay, I discuss my experiences using these UI frameworks.

My journey began with learning and implementing HTML and CSS. As a beginner, I found this easier than learning Bootstrap. HTML holds the structure and text, while CSS handles the styling. I initially found this method more intuitive than the expanded workflow of Bootstrap. With CSS, I could simply search for the specific styling I wanted to achieve. However, this simplicity had its drawbacks; I had to update both the CSS and HTML files constantly to add and style text. Overall, learning HTML and CSS was relatively straightforward with only a slight learning curve.

Bootstrap is built on CSS, allowing users to style a webpage without needing a separate stylesheet. While the logic is similar to CSS, the sheer volume of classes provided a slight challenge during the design phase. Bootstrap uses prebuilt classes, and my main struggle was finding the specific class I needed among so many options. With more experience, I can see how Bootstrap is more beneficial than custom CSS—it allows a developer to build an entire page within a single HTML file.

Applying these concepts, I recreated the Island Snow website using mostly Bootstrap. A sample image of the design and the corresponding code are provided below. I was able to effectively recreate the design, achieving high-quality results efficiently.

<div class="text-center p-4">
  <img width="800px" src="../img/sample.png" class="img-thumbnail" >
</div>
<div class="text-center p-4">
  Fig. 1: The recreated Island Snow webpage.
</div>

```html
<div class="navbar bg-light">
            <div class="container">
                <ul class="nav">
                    <li class="nav-item"><i class="bi bi-facebook p-1"></i></li>
                    <li class="nav-item"><i class="bi bi-twitter p-1"></i></li>
                    <li class="nav-item"><i class="bi bi-pinterest p-1"></i></li>
                    <li class="nav-item"><i class="bi bi-instagram p-1"></i></li> 
                </ul>
                <ul class="nav justify-content-end">
                    <li class="nav-item"><i class="bi bi-house-fill p-1"></i></li>
                    <li class="nav-item"><i class="bi bi-search p-1"></i></li>
                    <li class="nav-item"><i class="bi bi-person-fill p-1"></i></li>
                    <div class="nav-item dropdown">
                        <div class="dropdown-toggle" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                        <i class="bi bi-cart p-1"></i> 0
                        </div>
                        <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                            <li>Your cart is empty</li>
                        </ul>
                    </div>
                </ul>
            </div>
        </div>
```
Sample code of how the NavBar was designed without the use of the CSS file. 

```css
footer{
    background-color: #292929;
    color: white;
}
```
The CSS file showing a minimal amount of styling needed. This piece of code was the only code in the CSS file due to that fact that Bootstrap was able to handle the rest.  

In comparison, the webpage was built primarily with Bootstrap, while fine-tuning was completed with CSS. This approach increased my efficiency because I didn't need to switch between files constantly.

Overall, I enjoyed my first experience with UI frameworks. After completing a few exercises and "WODs" (Workouts of the Day), I gained a solid grasp of how they function. I found that the bulk of a website can be completed using Bootstrap classes alone. While it requires more initial learning, the potential for speed and consistency is well worth the effort. I feel much more confident now and look forward to expanding my knowledge of HTML, CSS, and Bootstrap.

