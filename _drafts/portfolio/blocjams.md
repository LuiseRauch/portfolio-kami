---
layout: post
title: BlocJams
thumbnail-path: "img/potfolio/blocjams_1.png"
short-description: A digital music player like Spotify.

---

{:.center}
![]({{ site.baseurl }}/img/potfolio/blocjams_1.png)


BlocJams is a digital music player like Spotify, created as a means to learn frontend web development. It employs a user-friendly web interface to display and play songs. The mp3 files are accessed through BuzzFeed sounds and the application is built within an Angular framework.

This school project was built in order to utilize HTML, CSS, Javascript and jQuery to produce a responsive, easy-to-navigate website that can generate and play music from a library.

BlocJams is a digital music player similar to Spotify. The website was built to practice and gain understanding of web development concepts.

It is my first Front End project, so it has a heavier focus on website design and user interface than my previous projects, which were more focused on the logic working in the background of most websites (user account logins, for example).
For this project, just about everything I did was completely new to me. While I had dabbled a little with JavaScript code, HTML, and CSS design before Bloc Jams, this project pushed me to:
code a music player bar that responds appropriately to play, pause, skip, back, and scrub commands (and continues to play when the user leaves the page)
integrate jQuery to create animations within the project
learn a whole lot more about controlling the DOM (Document Object Model) through CSS and JavaScript code
refactor my JavaScript and jQuery into AngularJS
build Angular templates, controllers, services, directives, and filters

## BlocJams - the Idea

The main task was to learn how to incorporate and build the entire application using the Angular framework. It was challenging to learn how to initiate Angular modules, controllers and services. It was also difficult to learn and appropriately apply the different types of services. Finally, I had to learn the Angular directives to use in the html pages in order to have the desired functionality.

The challenge here was to build an attractive and fully functional site for finding and playing music, much like Spotify


The aim was to build a simple online music player which would be highly usable, responsive and aesthetically pleasing.


The hardest parts of this project were definitely when I needed to relearn a lot of what I thought I knew about code in order to refactor Bloc Jams into Angular. While AngularJS is an incredible way to condense the amount of redundant code in a project and handle a lot of Back End logic through a Front End code base, it was another learning curve for me that took a long time to work through.


Accessing music through a static website is almost impossible, and if it is, it's frustrating. For Blocjams, it was necessary to circumvent this frustration by allowing a user to simply enter the web app and begin playing music by pressing play. Additionally, accessing a web application that plays music on a mobile phone can be cumbersome and buggy, hence making the Blocjams player responsive was critical. In brief, the two problems I was trying to address in the project were:

Static website music players, which only allowed access to one type of music and not a myriad of albums.
A responsive audio player accessible anywhere.

## BlocJams - the App

The site was centered around one Angular module built with a UI-router to connect the different controllers and services. The controllers were organized according to the different pages within the application- one for the landing page, one for the collection of albums, and one for the album page that lists the album songs. A player-bar controller was also created to compartmentalize the functionality of the bottom bar and incorporate it in the appropriate views.

I built the site initially through HTML and CSS, then added functionality and animation with Javascript and jQuery.

Three pages were implemented: the landing page, the collection page and the album page. The pages feature minimalistic contemporary design. The website uses jQuery as the main library to handle user interactions. Sound was handled by the Buzz library.

Using a variety of images, music files, and JavaScript libraries, the Blocjams player was born. The assets included images of albums and audio files from those albums. jQuery was used to create dynamic movements within the Blocjams player bar and also allowed for simple selection within the album. Consequently, users could easily switch, play, or pause songs in the player bar. Lastly, the player bar itself was adjustable via jQuery selectors and handlers. The audio player song file was enabled via the Buzz API, which allowed users to better interact with the player bar and the volume of the song.




The application is fully functioning with the ability to navigate between the different pages. The song player will play songs upon request with the ability to stop, pause, skip to the next/previous song, skip to a later point in the song, and to control the volume.

The resulting website is attractive and responsive, and functions much like a basic version of Spotify.

BlocJams is a beautiful responsive website. It responds to changes in browser window size and looks good both on a phone and a desktop computer.



The Blocjams static home page, album collection page, and also album contents page. The static page was an aesthetically pleasing introduction to the website and its capabilities. By selecting collection users could access the entirety of the albums available. Thereafter, they could select the album of their choice. Once in the album, users could begin playing by simply selecting the play button. Switching was conducted via the player bar or by selecting a new song. And the user also had the option of changing the place in the song and the volume of the song.

> The Blocjams player only had three pages, but due to its functionality, it provided the music obsessed listener with direct access to what matters most, the song.


To ensure responsiveness, I used certain CSS styling that augmented the structure if the screen size changed. Hence, the music lover could find, select, and play the song of their choice anywhere.



Angular was an efficient way to build this web based music player. BuzzFeed sounds made simple music tasks such as start, stop, and play easy. The UI-Router was an easy and efficient way to structure the application that made the single page application very effective.

This project was a terrific learning experience, allowing me to showcase basic web-building skills and produce a product of which I can be proud.

Making the website allowed me to put some of my web development knowledge into practice and also learn a lot of new things. During the course of development I practiced styling the page with CSS, dynamically altering the contents of pages using JavaScript and learned a couple of libraries. I am now building on that experience in the hopes of creating more complex webpages and applications.


I was surprised to discover how simple API plugins and jQuery could create such a dynamic webpage. Further, I learned the DOM, its magnificent usefulness, and how CSS selectors are used across an interface.

I learned that labeling functions very specifically was key in efficiency as my codebase grew.
