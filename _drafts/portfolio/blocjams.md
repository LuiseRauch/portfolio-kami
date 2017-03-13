---
layout: post
title: BlocJams
thumbnail-path: "img/portfolio/blocjams_3.png"
short-description: A digital music player like Spotify.

---

{:.center}
![Sreenshot BlocJams ]({{ site.baseurl }}/img/portfolio/blocjams_3.png)

**Bloc Jams** is a digital music player like Spotify and was my first frontend project at [bloc.io](https://bloc.io){:target="_blank"}. The aim  was to learn about programming concepts using JavaScript, applying that knowledge by altering the DOM, structuring & styling with HTML and CSS, using my first libraries in jQuery and Buzz and refactoring the code into AngularJS.

> For learning purposes we wrote the application first in plain JavaScript, then jQuery & refactored it into AngularJS. It was interesting to see how little code is needed & how much more intuitive those frameworks/libraries are. While plain JavaScript is challenging for me, I will work on  having a profound knowledge of JS rather than just relying on easier frameworks.  


## BlocJams - the Idea

Just like Spotify, **Bloc Jams** is a simple & user-friendly online music player - highly usable, responsive and aesthetically pleasing.

The focus is on usability that works seamlessly across any device. The Angular single page application allows the user to simply enter the web app and begin playing music by pressing play.

code a music player bar that responds appropriately to play, pause, skip, back, and scrub commands (and continues to play when the user leaves the page)

## BlocJams - the App

The static backbone of the **Bloc Jams** layout with is built with HTML. Then added styling and responsiveness using CSS ,integrate jQuery to create animations and effects within the project  and implemented interactivity and dynamic functionality an Angular framework.


jQuery is a great tool for adding animations and effects to a page, but it's difficult to build a sophisticated frontend application with jQuery alone. In this project, you'll refactor Bloc Jams using AngularJS, commonly referred to as Angular.

build Angular templates, controllers, services, directives, and filters

The site was centered around one Angular module built with a UI-router to connect the different controllers and services. The controllers were organized according to the different pages within the application- one for the landing page, one for the collection of albums, and one for the album page that lists the album songs. A player-bar controller was also created to compartmentalize the functionality of the bottom bar and incorporate it in the appropriate views.

The UI-Router was an easy and efficient way to structure the application that made the single page application very effective.

Sound was handled by the Buzz library.
The mp3 files are accessed through BuzzFeed sounds.
Bloc Jams has been a silent music player so far, and it's time to change that. We'll use the Buzz music library to play and pause music in our application. We've already written many of the functions required to update the interface, so we'll focus more on helper methods that use Buzz to change song playback, volume, and state.


<div class="slideshow">
  <div class="slideshow-container">
    <div class="mySlides fade">
      <img src="/img/portfolio/blocjams_1.png" style="width:100%">
    </div>

    <div class="mySlides fade">
      <img src="/img/portfolio/blocjams_4.png" style="width:100%">
    </div>

    <div class="mySlides fade">
      <img src="/img/portfolio/blocjams_5.png" style="width:100%">
    </div>

    <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
    <a class="next" onclick="plusSlides(1)">&#10095;</a>
  </div>
  <br>
  <div style="text-align:center">
    <span class="dot" onclick="currentSlide(1)"></span>
    <span class="dot" onclick="currentSlide(2)"></span>
    <span class="dot" onclick="currentSlide(3)"></span>

  </div>
</div>

<br />
