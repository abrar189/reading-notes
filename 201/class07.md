# Domain modeling

 is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.

## Here's some tips to follow when building your own domain models.

1. When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
2. Model its attributes with a constructor function that defines and initializes properties.
3. Model its behaviors with small methods that focus on doing one job well.
4. Create instances using the new keyword followed by a call to a constructor function.
5. Store the newly created object in a variable so you can access its properties and methods from outside.
6. Use the this variable within methods so you can access the object's properties and methods from inside.

# Tables

What's a Table?
A table represents information in a grid format. Examples of tables include financial reports, TV schedules, and sports results


## Basic Table Structure

`<table>`

The `<table>` element is used to create a table. The contents of the table are written out row by row.

`<tr>`

You indicate the start of each row using the opening `<tr>` tag.(The tr stands for table row.)

`<td>`

Each cell of a table is represented using a `<td>` element. (The td stands for table data.)

![image](https://slideplayer.com/slide/4205843/14/images/9/HTML+Tables+Table+Example+How+the+HTML+code+above+looks+in+a+browser%3A.jpg)

## Table Headings

`<th>`

The `<th>` element is used just like the `<td>` element but its purpose is to represent the heading for either a column or a row. (The th stands for table heading.)

![image](https://lh3.googleusercontent.com/proxy47ucXFODVOTjc-vpNsOlhJAIl_hgaewkLx4ny4Wy6NWhOTLjD0HkUVkZ1hkIS4SlWmyMjjmFOpNsg-BrK7lKQVo29VHfrxmeT05PJ35LBxsYDKiEf2A)

# FUNCTIONS, METHODS & OBJECTS

- Functions allow you to group a set of related statements together that represent a single task.
- Functions can take parameters (informatiorJ required to do their job) and may return a value.
- An object is a series of variables and functions that represent something from the world around you.
- In an object, variables are known as properties of the object; functions are known as methods of the object.
- Web browsers implement objects that represent both the browser window and the document loaded into the browser window.
- JavaScript also has several built-in objects such as String, Number, Math, and Date. Their properties and methods offer functionality that help you write scripts.
- Arrays and objects can be used to create complex data sets (and both can contain the other). 