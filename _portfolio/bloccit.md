---
layout: post
title: Bloccit
thumbnail-path: "img/portfolio/bloccit_5.png"
short-description: A Reddit replica where people can post, vote on, share and save links and comments.

---

{:.center}
![Sreenshot Bloccit Sign Up]({{ site.baseurl }}/img/portfolio/bloccit_5.png)

## Explanation

Just like Reddit, Bloccit (find it [here](https://peaceful-bayou-3140.herokuapp.com/) on Heroku) is a Ruby on Rails web app where people can post, vote on, share & save links and comments.
It also provides authentication and authorization.

This was my first project at [bloc.io](https://bloc.io).

## Problem

We anticipated that Bloccit users will create a large number of posts, and will therefore need a way to organize, or categorize them.
Also we wanted to associate users and posts, to allow ownership of content in Bloccit. And implement a voting feature because users will want a feature to distinguish the good from the bad.

## Solution & Results

To create Bloccit I first started designing a basic UI as a foundation to build on, created static views and provided the structure (HTML) & the style (CSS).

Then created data models so when Bloccit users post information and comment on those posts - posts & comments are persisting, used the ORM library ActiveRecord to communicate with the database and seeded data.

![Sreenshot Bloccit Topics]({{ site.baseurl }}/img/portfolio/bloccit_2.png)

I Implemented CRUD operations on my models so the users can perform these actions from the views, nested resources and refactored code.
And added validation methods for the database.

![Sreenshot Bloccit New Post]({{ site.baseurl }}/img/portfolio/bloccit_4.png)

I built a user authentication system (instead of using Devise or similar) to get a better feeling on how it works, associated users and posts to allow ownership of content by defining roles & rules. I added authorization and used shallow nesting to prevent routes from becoming long.

I then added three more features - lables, favourites and voting. The labeling feature - to learn about the many-to-many relationship and polymorphism, the voting feature using inclusion validation - and the favoriting feature to allow users to flag posts to notify them when a post receives a new comment using ActionMailer and callbacks.

![Sreenshot Bloccit Post]({{ site.baseurl }}/img/portfolio/bloccit_3.png)

I also used Ajax to delete & create comments, without reloading the page and in the end build a RESTful API for Bloccit, to make the system's data available for other developers to use.

## Conclusion

The purpose of this project was to learn the fundamentals of web development, Rails and TDD.
I am now able to built a robust web application with a comprehensive test suite. Along the way, I've learned about clients, servers, MVC architecture, RESTful API design, refactoring, and much more.
