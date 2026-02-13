<img src="../images/iDHL-DarkBlue.svg" alt="IDHL Logo" title="IDHL" width="90">

# Junior Developer Assessment

## Overview

You will create a blog post page using ASP.NET MVC. The focus is on demonstrating your fundamental skills in MVC, data handling, and basic front-end development.

We'd expect this to take around **3 hours**, but there's no time limit — work at your own pace and don't feel pressured to rush or over-polish.

## Objectives

1. ASP.NET MVC skills
1. Routing and controllers
1. Basic CSS and responsive layout
1. Data retrieval and persistence
1. Form input and validation

## Exercises

### Exercise 1

Develop an MVC view that displays the blog post content, utilising the layout provided in the [template.html](../assets/template.html) file.

Move the [Blog-Posts.json](../assets/Blog-Posts.json) file to an appropriate location in the project for reading and writing data. Replace the section marked `<!--Blog post content-->` with the content from this JSON file.

Load a specific blog post from the JSON file based on its ID, employing MVC routing and the appropriate controller actions. For example: /blog/1/, /blog/2/, /blog/\<ID\>/, etc.

### Exercise 2

Display a list of comments related to the blog post, sourced from the JSON file. Add this content to the section marked `<!--Blog post comments-->`.

### Exercise 3

In the section marked `<!--Blog post comment form-->`, add a comment form that allows users to submit comments, which will be stored against the relevant blog post item in the Blog-Posts.json file.

Form fields:
- Name (required)
- Email address (required)
- Comment (required)

### Exercise 4 (Optional)

Implement the functionality to reply to a comment. Save the reply in the appropriate section of the JSON file and display it directly underneath the comment to which the user has responded.