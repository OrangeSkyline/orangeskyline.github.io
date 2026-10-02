### Welcome!

This is the start of our Documentation Page! We are [Aaron](https://github.com/Zoidster), [Alex](https://github.com/OrangeSkyline), [Admir](https://github.com/admirsmajic0), [Arieana](https://github.com/atrevizo), [Kingston](https://github.com/KafoolsDelDoe), [Nick](https://github.com/Nicobotic1), and [Richard](https://github.com/richard-RRL)!
If you'd like, click this link to view the website version of this documentation: [Documentation Page](https://orangeskyline.github.io)

---

# Table of Contents:

1. <a href="#markdown-cheat-sheet">Markdown Cheat Sheet(Alex)</a>
2. <a href="#command-line">Command Line(Richard)</a>
3. <a href="#python-cheat-sheet-comparisons">Python Cheat Sheet Comparisons(Kingston)</a>
   - [C++(Aaron)](#CPlusPlus)
   - [C#(Alex)](#CSharp)
   - [Java(Kingston)](#Java)
4. <a href="#django-overview">Django Overview &amp; (Nick)</a>
5. <a href="#setting-up-django">Setting Up Django &amp; (Nick)</a>
6. <a href="#gitgithub-development-environment">Git/GitHub Development Environment(Alex)</a>
7. <a href="#html">HTML(Admir)</a>
8. <a href="#accessibility">Accessibility(Kingston)</a>
9. <a href="#css-w-bootstrap">CSS w/ Bootstrap(Aaron)</a>
10. <a href="#python-virtual-environments">Python Virtual Environment(Arieana)</a>
11. <a href="#python-packages--dependencies">Python Packages &amp; Dependencies(Alex)</a>

# Markdown Cheat Sheet:

- # Bigger Heading = `# Bigger Heading`
- ## Smaller Heading = `## Smaller Heading` (These can go as small as heading 6, which is 6 #'s)
- **Bold** = `**Bold**`
- _Italic_ = `*Italic*`
- [Hyperlink](https://example.com/) = `[Hyperlink](https://example.com/)`
- ![Silver SUV](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTFstbf22H156QSR9N_Lo64AzqUswLFjcylvEEZGDMszw&s) = `![Description of Image](website.com/image.jpg)`
- `Code` = \`Code` OR
  \```
  Code
  \```
- - Thing 1 = `- Thing 1`
- 1. Thing 1 = `1. Thing 1`
- > Words = `> Blockquote`
- `--- Horizontal Line`

---

   <table>
      <thead>
        <tr>
          <th>Name</th>
          <th>Age</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>John</td>
          <td>30</td>
        </tr>
        <tr>
          <td>Jane</td>
          <td>25</td>
        </tr>
      </tbody>
   </table>

   <h3>Table = (Make sure to separate the lines above and below the table by one blank line)</h3>

```
| Name | Age |
|------|-----|
| John | 30  |
| Jane | 25  |
```

# Command Line:

Section by Richard Luna

### Definitions

Command line is a direct function that allows a user to directly control an application with the operating system.
Command Line Shells: These are distinct programs that have pre-made scripts.
Ex. Powershell, Command Prompt, Git CMD
Scripts/Commands: These are automated instructions.
Automate repetitive tasks like committing changes to github or opening a repository to work out of.
These directly communicate with CPUs which is more efficient.

### Example Commands

The following commands include standard GitHub repository commiting/pushing and setting up our Django project with a python virtual machine.
Make sure you have compatible up to date versions of both Python and Django.

  <table>
      <thead>
        <tr>
          <th>Command</th>
          <th>Example</th>
          <th>Description</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Path to directory</td>
          <td><code>"C:\Users\Richa\Downloads"</code></td>
          <td><img src="images/CMDFileLocEX.png" alt="Simple annotated guide showing one way to find a folder's address path">
          How to find your directory path
          You can also "copy address" from your file explorer's top bar that shows the current path</td>
        </tr>
        <tr>
          <td>cd “path to directory”</td>
          <td>`cd "C:\Users\Richa\Downloads"`</td>
          <td>This opens command line to that specific folder for further commands</td>
        </tr>
      </tbody>
   </table>
   
# Python Cheat Sheet Comparisons:
1. <p id="CPlusPlus"><strong>C++</strong></p>

### Variables and Declaration

#### Python

```
age = 25          # Automatically created as an integer
salary = 50000.5  # Automatically created as a float
```

Variables in Python are declared implicitly via specifying the variable name and giving a value, with the type inference.

#### C++

```
int age = 25;             // Explicitly declared as an integer
double salary = 50000.5;  // Explicitly declared as a floating-point
```

Variables in C++ are declared via specifying the type for the variable, the variable name, then an =, then the value for that variable.

### Headers/Comments

#### Python

```
# This is a python comment
```

Comments in Python can be made using the # symbol

#### C++

```
// This is a C++ comment
```

Comments in C++ can be made using two slashes in the manner of // for a single line and /\* for multiple lines.

### Libraries

#### Python

```
# main.py
# Standard library module providing access to system-specific functions and variables
import sys

# Custom local module (math_utils.py) containing mathematical helper functions
import math_utils
```

Libraries in Python are accessed using the `import` keyword followed by the library name. They are also refered to as modules

#### C++

```
// main.cpp
#include <iostream>      // Standard library header for input/output streams
#include "math_utils.h"  // Custom header file wrapped in quotes
```

Libraries in C++ can be accessed via what is called a header file. This is done by using a # sign, then the keyword `include` followed by

(If the header is a standard C++ header) the header name in <> brackets
Ex: `#include <iostream>`

(If the header name is a user made file) the name of the header file and its path relative to the directory being executed from
Ex: `#include "path/to/my_header.h"`

### Functions

#### Python

```
def add(x, y):
    return x + y
```

Functions in python can be defined via the `def` keyword then followed by the function name with its arguments given in () with their type if needed followed by a :
Brackets are not required and function bodies are determined via spacing

#### C++

```
int add(int x, int y) {
    return x + y;
}
```

Functions in C++ can be defined via specifying a return type, or void for no return type, then a name for the function followed by its arguments given in () with their type if needed then {} disclose the body of the function

### Loops

#### Python

```
# For loop: Iterates over a sequence (0 to 4)
for i in range(5):
    print(i)

# While loop: Runs as long as a condition is true
count = 0
while count < 5:
    print(count)
    count += 1
```

Loops in python include the for loop and the while loop

##### For loop:

Defined via the keywords `for i in range`, then () with the first argument is the lowest count and the second argument is the highest count. The highest count will decrement to the lowest over the course of the loop automatically

##### While loop:

Defined via the keyword `while`, then () with the first argument is the lowest count and the second argument is the highest count. The user has to choose how to decrement the counter within the loop body. Then it is ended with a : and the body is indicated via spacing

#### C++

```
// For loop: Initializes, checks condition, and increments
for (int i = 0; i < 5; i++) {
    std::cout << i << "\n";
}

// While loop: Runs as long as the condition is true
int count = 0;
while (count < 5) {
    std::cout << count << "\n";
    count++;
}
```

Loops in C++ include the for loop, the while loop, and the do-while loop

##### For loop:

Defined via the keyword `for`, then in () separated by ; the variable that will be the counter, the condition for when it should exit the loop, then the means of change on the counter, then {} disclose the body of the loop

##### While loop:

Defined via the keyword `while`, then in () a counter/condition is given that is typically modified within the body of the loop, once satisfied the loop terminates

##### Do-While loop:

Defined via the keyword `do` then {} for the body of the loop which usually contains a way to modify the loop counter, then a while keyword, then in () a counter/condition that terminates the loop once satisfied. This allows the loop to execute once even if the condition is satisfied.

### Classes

#### Python

```
class Car:
    # The constructor runs automatically whenever a new Car object is created.
    # "self" refers to the specific Car object being created.
    # "brand: str" and "year: int" are type hints telling us what kind
    # of values we expect to receive.
    def __init__(self, brand: str, year: int):

        # Store the brand inside this particular Car object.
        # "self.brand" is an instance variable, meaning every Car object
        # gets its own separate brand value.
        self.brand = brand

        # The double underscore makes this attribute "private-like."
        # Python uses name mangling here, so it is not intended to be
        # accessed directly outside of the class.
        self.__year = year

    # A method is a function that belongs to a class.
    # "self" allows this method to access data belonging to the object
    # that called it.
    def display_info(self):

        # Access the object's brand and year and display them.
        # The f-string lets us insert variable values directly into the text.
        print(f"Car: {self.brand}, Year: {self.__year}")


# Create a new Car object.
# "Toyota" is passed to the "brand" parameter.
# 2024 is passed to the "year" parameter.
my_car = Car("Toyota", 2024)

# Call the display_info() method belonging to our Car object.
# This prints the information stored inside "my_car."
my_car.display_info()
```

Classes in python are defined via the `class` keyword, then a class name, then a : and then the class body is disclosed via spacing. A constructor for the class can be defined as a function `def __init__(self`,

#### C++

```
#include <iostream>  // Provides std::cout and std::endl for displaying output.
#include <string>    // Provides the std::string data type.

class Car {
private:
    // This variable stores the year of the car.
    // "private" means code outside of the Car class cannot directly
    // access this variable.
    int year;

public:
    // This variable stores the brand of the car.
    // "public" means code outside of the class CAN directly access it.
    std::string brand;

    // Constructor:
    // This function automatically runs when a new Car object is created.
    //
    // "b" receives the car's brand.
    // "y" receives the car's year.
    //
    // The constructor then stores those values in the object's
    // "brand" and "year" variables.
    Car(std::string b, int y) {
        brand = b;
        year = y;
    }

    // Method:
    // A function that belongs to the Car class.
    //
    // This method accesses the object's stored data and prints it.
    void display_info() {
        std::cout << "Car: " << brand
                  << ", Year: " << year
                  << std::endl;
    }
};  // The semicolon after the class definition is required in C++.


int main() {

    // Create a Car object named "my_car."
    //
    // "Toyota" is passed to the constructor's "b" parameter.
    // 2024 is passed to the constructor's "y" parameter.
    //
    // The constructor then stores those values inside my_car.
    Car my_car("Toyota", 2024);

    // Call the display_info() method belonging to my_car.
    // This prints the car's stored brand and year.
    my_car.display_info();

    // Return 0 tells the operating system that the program
    // finished successfully.
    return 0;
}
```

Classes in C++ are defined via the `class` keyword, then a class name, then, within () are arguments to the class with their variable type, then {} denote the body of the class. Then within the body both member variables and member functions can be defined within its public and private tags which disclose which members can be accessed via instantiation of the class. The class can be instantiated as with any other variable type and arguments can be passed in accordance with the classes valid constructors.

---

2. <p id="CSharp"><strong>C#</strong></p>

3. <p id="Java"><strong>Java</strong></p>

# Django Overview:

Section by Nick Larsen

### What is Django?

Django is a Python framework that we can use to help us build web applications. Django does a lot of the heavy lifting in creating the backends of web applications. This allows us to focus our attention on design and process.

### Why would want to use Django?

- Django can help build secure and scalable websites quickly.

- Django does a lot of the heavy lifting for the backend of a website / web application.

- Django is free.

- Django is open source.

- Django uses python.

### What are some websites that were built using Django?

1. Instagram

2. Spotify

3. The Washington Post

# Setting up Django

Section by Nick Larsen

# Git/GitHub Development Environment:

# HTML:

# Accessibility:

# CSS w/ Bootstrap:

## What is it?

### CSS

CSS is a language used for the stylization of webpages on top of base HTML. It can be applied across multiple pages using a style sheet. A style sheet is a pre-defined CSS file that defines declarations that can be used on the different selected elements in HTML to change aspects like their alignment, color, font, size, and many other aesthetic aspects.

### BOOTSTRAP

Bootstrap is a large collection of pre-written CSS and JavaScript that allows for the quick application of styling, layouts, and interactive components to webpages like buttons.

## Setup

### CSS

<img src="images/CSS setup.PNG" alt="Selector {property:value; property:value}">

```
<link rel="stylesheet" href="style.css">```

CSS can be defined in a .css file as a style sheet. To link CSS it is done with the above `<link>` tag with the href attribute telling where to find the CSS file, The document holds different declarations about how the HTML elements in question should be styled via a selector which represents the element, then a key value pair that defines the specifics of the change being undertaken. CSS can be defined in a separate file or written in-document with the HTML.

### BOOTSTRAP

```
<div class="container mt-5">
    <div class="row">
        <div class="col-sm-4">
```

```
<link href="BOOTSTRAP_CSS_URL" rel="stylesheet">
```

## Containers/Grid (BOOTSTRAP)

### Containers

Containers are used to pad the content inside of them. Fluid containers are a responsive design element that adjust to screen width across devices and platforms. Containers can be colored, bordered, buffered, styled, and change the aesthetics of their text

### Grid

<img src="images/Grid.PNG" alt="Selector Image showing combinations of spans using the grid system ranging from span 4+8 to span 12*">

The grid system allows for even spacing of elements across the span of a page for the organization of information and content
To link BOOSTRAP, it is done with the above `<link>` tag with the href attribute pointing to the bootstrap version in use. Once done classes from BOOTSTRAP can be used via inserting `<div>` tags and instantiating the classes within them such that they apply to the children.

## Responsive Design (BOOTSTRAP)

Responsive design is a design methodology that accounts for the differences in layout and size of webpages across different devices. This is a major element of bootstraps design philosophy.

## Navigation/Components (BOOTSTRAP)

### Nav Menus

```
<ul class="nav">
  <li class="nav-item">
	<a class="nav-link" href="#">Link</a>
  </li>
  <li class="nav-item">
	<a class="nav-link" href="#">Link</a>
  </li>
  <li class="nav-item">
	<a class="nav-link" href="#">Link</a>
  </li>
  <li class="nav-item">
	<a class="nav-link disabled" href="#">Disabled</a>
  </li>
</ul>
```

<img src="images/NavMenu.PNG" alt="Selector Nav menu with Link Link Link Disabled">

Simple menus that allow for direct navigation can be made in the form of menus and bars.

### Buttons

```
<button type="button" class="btn btn-primary">Primary</button>
```

<img src="images/Button.PNG" alt="An example of a Button">

Buttons are singlet components on the page that can link to content on other pages or the same page

### Drop Downs

```
<div class="dropdown">
  <button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown">
	Dropdown button
  </button>
  <ul class="dropdown-menu">
	<li><a class="dropdown-item" href="#">Link 1</a></li>
	<li><a class="dropdown-item" href="#">Link 2</a></li>
	<li><a class="dropdown-item" href="#">Link 3</a></li>
  </ul>
</div>
```

<img src="images/DropDown.PNG" alt="An example of a Drop Down Menu">

Drop down are components that when clicked provide multiple selectable options that navigate the page(s)

### Carousel

```
<div id="demo" class="carousel slide" data-bs-ride="carousel">

  <!-- Indicators/dots -->
  <div class="carousel-indicators">
	<button type="button" data-bs-target="#demo" data-bs-slide-to="0" class="active"></button>
	<button type="button" data-bs-target="#demo" data-bs-slide-to="1"></button>
	<button type="button" data-bs-target="#demo" data-bs-slide-to="2"></button>
  </div>

  <!-- The slideshow/carousel -->
  <div class="carousel-inner">
	<div class="carousel-item active">
  	<img src="la.jpg" alt="Los Angeles" class="d-block w-100">
	</div>
	<div class="carousel-item">
  	<img src="chicago.jpg" alt="Chicago" class="d-block w-100">
	</div>
	<div class="carousel-item">
  	<img src="ny.jpg" alt="New York" class="d-block w-100">
	</div>
  </div>

  <!-- Left and right controls/icons -->
  <button class="carousel-control-prev" type="button" data-bs-target="#demo" data-bs-slide="prev">
	<span class="carousel-control-prev-icon"></span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#demo" data-bs-slide="next">
	<span class="carousel-control-next-icon"></span>
  </button>
</div>
```

<img src="images/Carousel.PNG" alt="An example of a Carousel">

A rotating collection of images and content on the page that can be navigated.

##### .carousel

Creates a carousel

##### .carousel-indicators

Adds indicators for the carousel.

##### .carousel-inner

Adds slides to the carousel

##### .carousel-item

Specifies the content of each slide

##### .carousel-control-prev

Adds a left button to the carousel

##### .carousel-control-next

Adds a right button to the carousel

##### .carousel-control-prev-icon

Used together with .carousel-control-prev to create a "previous" button

##### .carousel-control-next-icon

Used together with .carousel-control-next to create a "next" button

##### .slide

Adds a CSS transition and animation effect when sliding from one item to the next.

## Accessibility

Bootstrap includes built-in accessibility features to help make websites usable for people with disabilities. Use semantic HTML, proper labels, and Bootstraps accessibility classes and attributes where needed.

# Python Virtual Environments:

# Python Packages & Dependencies:
