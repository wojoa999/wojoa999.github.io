---
layout: essay
type: essay
title: "Order-Up"
# All dates must be YYYY-MM-DD format!
date: 2026-04-27
published: true
labels:
  - Design Patterns
  - Software Architecture
  - Professional Development
---
<img width="500px" class="rounded d-block mx-auto" src="../img/kitchen.jpg">

## Cooking-Up Patterns
Picture yourself working in a fine dining restaurant, you are tasked with ensuring that the kitchen runs smoothly. During the diner rush, you realize that the kitchen isn’t operating on simply following a recipe, but a system to keep the kitchen orderly. In software, these systems are considered design patterns. They are pre-designed templates that ensure the organization of logic and architecture. These patterns don't resemble the ingredients themselves, but establish the practices that should occur when pressure arises. Mastering the kitchen of a codebase, design patterns can be categorized into creating, structuring, and behavior. 

A kitchen is divided into stations to allow the staff to accomplish multiple tasks at the same time. It is not efficient for the staff to each complete a single meal or have a single person completing all the tasks. The standardization of stations allows each member to focus on a single “template” and effectively produce it.  As a task is needed to be completed the respective stations will complete the task. 

The location of ingredients within your kitchen plays an important role when trying to complete orders on a busy night. Structural patterns show the ingredients are composed into the meal you order. While you don’t see the cooking of the meal, the customer knows what is happening behind the double-doors to the kitchen. This ensures that the customer sees the meal, but not what is occurring in the kitchen.  

After the meal is completed and placed in the window the executive chef rings the order-up bell. This signals that the order is ready to be served, acting as the communication between the kitchen and the server. The server recognizes this "behavior" and knows that the order is ready to be served to the customer. All the servers are able to hear this bell, but the signal is acknowledged that the meal is ready to change states from the kitchen to the customer.   

## Restaurant Application
The appetizers, entrees, garnish, and desserts fall into the stations designed to organize the kitchen. These categories resemble the components implemented into the application that was designed. Much like the “kitchen”, the components act as the “stations” that help ensure that the application is running smoothly. Rather than storing all of the information into a single file, or staff, the components break the files up into smaller more focused organized categories to help split up the work to improve efficiency. Much like the kitchen, each component doesn't worry about each component's functions, but the end product will result in a fabulous meal. The navbar is used as a component in the application to help clean up the code and can be seen below:

```cpp
<Navbar expand="lg" style={{ backgroundColor: '#024731' }} variant="dark">
      <Container>
        <Navbar.Brand href="/">UH ITS Email Helper</Navbar.Brand>
        <Navbar.Toggle aria-controls="basic-navbar-nav" />
        <Navbar.Collapse id="basic-navbar-nav">
          <Nav className="me-auto justify-content-start">
            {currentUser && (
              <>
                <Nav.Link id="browse-nav" href="/list" active={pathName === '/list'}>
                  Browse Templates
                </Nav.Link>
                <Nav.Link id="add-nav" href="/add" active={pathName === '/add'}>
                  Add Template
                </Nav.Link>
              </>
            )}
            {currentUser && role === 'ADMIN' && (
              <Nav.Link id="admin-stuff-nav" href="/admin" active={pathName === '/admin'}>
                Admin
              </Nav.Link>
            )}
          </Nav>
          <Nav>
```

Behind closed doors of the kitchen, the database actions are correlated to the back of the house that customers do not witness. In this case, the components utilizing the add, edit, and remove functions don't see what is happening behind the closed door. The components act as the customer and only see what is presented upfront. As a result the components only see the meal that is presented upon them. The complex database information is hidden from the components to present a clean and formatted solution. Allowing the components to see what is needed to be seen and when it should be seen. By keeping the messiness away from the customer, the dining room is able to focus on the meal that is presented. The database action for the application when a new template is added is shown below: 

```cpp
/**
 * Creates a new contact in the database.
 * @param template, an object with the following properties: title, template, category, author, tags, used.
 */
export async function addTemplate(template: { title: string; template: string; category: string; author: string; tags: string[]; used: number }) {

  const validatedCategory = categoryMap[template.category] || template.category;

  const created = await prisma.template.create({
    data: {
      title: template.title,
      template: template.template,
      category: validatedCategory,
      tags: template.tags,
      author: template.author,
      used: template.used,
    },
  });
  return created.id;
}
```

The hand that rings the diner bell is the executive chef, but in terms of the application the admin withholds this power. In the digital kitchen, the admin has the ability to ring the bell on the templates that users are allowed to use. If the email template presented is not up to par, the admin has the ability to edit or trash the meal. This ensures that every meal in the application is up to standards. To ensure that proper etiquette is in place, the admin has the ability to manage a kitchen by removing cooks and meals. Ultimately, giving the executive chef power to the admin users of the applications. To ensure the accuracy of dishes and user actions the admin has the final behavioral conclusion to what is sent out of the kitchen. The admin has the ability to edit and delete inadequate templates from the application shown in the snippit below:  

```cpp
<a 
  href={`/edit/${item.id}`} 
  className="btn btn-sm btn-outline-primary"
  style={{ fontSize: '0.75rem', padding: '4px 12px' }}
  onClick={(e) => e.stopPropagation()}
  > 
    Edit
</a>
<button
  className="btn btn-sm btn-outline-danger"
  style={{ fontSize: '0.75rem', padding: '4px 12px' }}
  onClick={async (e) => {
    e.stopPropagation();
    if (confirm(`Delete "${item.title}"?`)) {
      await deleteTemplate(item.id);
      window.location.href = '/list';
    }
  }}
>
    Delete
</button>
```


