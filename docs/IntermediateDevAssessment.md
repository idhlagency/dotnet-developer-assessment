<img src="../images/iDHL-DarkBlue.svg" alt="IDHL Logo" title="IDHL" width="90">

# Intermediate Developer Assessment

## Overview

You will create a blog post page using ASP.NET MVC. The focus is on demonstrating your ability to architect a well-structured solution — applying SOLID principles, separation of concerns, and patterns such as dependency injection and caching alongside the core MVC skills.

We'd expect this to take around **5 hours**, but there's no time limit — work at your own pace and don't feel pressured to rush or over-polish.

## Objectives

1. ASP.NET MVC skills
1. Routing and controllers
1. Creating a service layer demonstrating SOLID principles
1. Unit testing
1. Basic CSS and responsive layout
1. Data retrieval and persistence with caching
1. Form input and validation (client-side and server-side)

## Exercises

### Exercise 1

Develop an MVC view that displays the blog post content, utilising the layout provided in the [template.html](../assets/template.html) file.

Move the [Blog-Posts.json](../assets/Blog-Posts.json) file to an appropriate location in the project for reading and writing data. Replace the section marked `<!--Blog post content-->` with the content from this JSON file.

Load a specific blog post from the JSON file based on its ID, employing MVC routing and the appropriate controller actions. For example: /blog/1/, /blog/2/, /blog/\<ID\>/, etc.

Your solution should demonstrate:
- A service or repository layer with a clear separation from the controller
- Dependency injection throughout
- Caching to avoid repeatedly reading from the JSON file on every request

### Exercise 2

Ensure your service layer is designed to be testable, and demonstrate this with unit tests covering the key behaviours — for example, retrieving a post by ID, handling a post that doesn't exist, and adding a comment. Full coverage isn't the goal; we're more interested in how you've structured your code to support testing.

### Exercise 3

Display a list of comments related to the blog post, sourced from the JSON file. Add this content to the section marked `<!--Blog post comments-->`.

### Exercise 4

In the section marked `<!--Blog post comment form-->`, add a comment form that allows users to submit comments, which will be stored against the relevant blog post item in the Blog-Posts.json file.

Form fields:
- Name (required)
- Email address (required)
- Comment (required)

### Exercise 5

Implement the functionality to reply to a comment. Save the reply in the appropriate section of the JSON file and display it directly underneath the comment to which the user has responded.

### Exercise 6 (Optional)

Incorporate a file upload feature that allows users to attach files to their comments. The uploaded files should be stored separately from the JSON file, while a reference to each file should be captured within the JSON data.

### Exercise 7 (Optional)

Create a blog listing page that displays basic blog cards for each post, with each card linking to the corresponding blog post. If time permits, implement pagination to enhance navigation through the blog posts.