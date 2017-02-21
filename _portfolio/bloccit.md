---
layout: post
title: Bloccit
thumbnail-path: "img/portfolio/bloccit_5.png"
short-description: A Reddit replica where people can post, vote on, share and save links and comments.

---


{:.center}
![Sreenshot Bloccit Sign Up]({{ site.baseurl }}/img/portfolio/bloccit_5.png)


**Bloccit** (find it [here](https://peaceful-bayou-3140.herokuapp.com/){:target="_blank"} on Heroku) was my first project at [bloc.io](https://bloc.io){:target="_blank"}. The purpose of **Bloccit** was to learn the fundamentals of web development, Rails and TDD and to built a robust web application with a comprehensive test suite. Along the way, I've learned about clients, servers, MVC architecture, RESTful API design, refactoring, and much more.

> It was impressive how quickly you can set up a Rails App with a good tutorial and no prior experience in coding.

## Bloccit - the Idea

Just like Reddit, **Bloccit** is a Ruby on Rails web app where people can post, vote on, share & save links and comments. **Bloccit** users will create a large number of posts, and will therefore need a way to organize, or categorize them.

The app should provide authentication & authorization and associate users and posts, to allow ownership of content in **Bloccit**.
A voting feature should be implemented because users will want a feature to distinguish the good from the bad.

## Bloccit - the App

To create **Bloccit** I first started designing a basic UI as a foundation to build on, created static views and provided the structure (HTML) & the style (CSS).

I created data models so when **Bloccit** users post information and comment on those posts - posts & comments are persistent, I used the ORM library ActiveRecord to communicate with the database and seeded data.

I Implemented CRUD operations on my models so the users can perform these actions from the views, nested resources and refactored code. And added validation methods for the database.


<div class="slideshow">
  <div class="slideshow-container">
    <div class="mySlides fade">
      <img src="/img/portfolio/bloccit_1.png" style="width:100%">
    </div>

    <div class="mySlides fade">
      <img src="/img/portfolio/bloccit_2.png" style="width:100%">
    </div>

    <div class="mySlides fade">
      <img src="/img/portfolio/bloccit_4.png" style="width:100%">
    </div>

    <div class="mySlides fade">
      <img src="/img/portfolio/bloccit_3.png" style="width:100%">
    </div>

    <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
    <a class="next" onclick="plusSlides(1)">&#10095;</a>
  </div>
  <br>
  <div style="text-align:center">
    <span class="dot" onclick="currentSlide(1)"></span>
    <span class="dot" onclick="currentSlide(2)"></span>
    <span class="dot" onclick="currentSlide(3)"></span>
    <span class="dot" onclick="currentSlide(4)"></span>
  </div>
</div>

<br />

I built a user authentication system (instead of using Devise or similar) to get a better feeling on how it works, associated users and posts to allow ownership of content by defining roles & rules. I added authorization and used shallow nesting to prevent routes from becoming long.

I then added three more features - lables, favourites and voting. The labeling feature - to learn about the many-to-many relationship and polymorphism, the voting feature using inclusion validation - and the favoriting feature to allow users to flag posts to notify them when a post receives a new comment using ActionMailer and callbacks.

I also used Ajax to delete & create comments, without reloading the page and in the end build a RESTful API for **Bloccit**, to make the system's data available for other developers to use.
