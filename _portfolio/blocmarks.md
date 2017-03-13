---
layout: post
title: Blocmarks
thumbnail-path: "img/portfolio/blocmarks_4.png"
short-description: Social Bookmarking With Email - a production quality social bookmarking app that allows users to send, manage, and share bookmarks.

---

{:.center}
![Screenshot Blocmarks Topic Detail]({{ site.baseurl }}/img/portfolio/blocmarks_4.png)

The major learning objective for **Blocmarks** (find it [here](https://afternoon-hollows-1410.herokuapp.com){:target="_blank"} on Heroku), my second project at [bloc.io](https://bloc.io){:target="_blank"}, was on introducing me to [RubyGems](https://rubygems.org/){:target="_blank"} and API Services rather than building everything from scratch.

>  While being very impressed by the great solutions that are out there I also found myself spending a lot of time customizing gems in later projects to get the exact functionality that I needed.

## Blocmarks - the Idea

**Blocmarks** is an application that allows its user to bookmark URLs via email, peruse other user's bookmarks and maintain a personal index of categorized bookmarks.

It's easy enough to bookmark a URL in your browser, but eventually your bookmark library may get cluttered and it may require effort to manage bookmarks.
Wouldn't you also like the ability to share bookmarks with friends? That is not something you can do easily from your native browser.

**Blocmarks** should solve these problems by organizing bookmarks by topic and making them public so that other users can find them and add bookmarks to their own **Blocmarks** profile.

## Blocmarks - the App

<div class="slideshow">
  <div class="slideshow-container">
    <div class="mySlides fade">
      <img src="/img/portfolio/blocmarks_1.png" style="width:100%">
    </div>

    <div class="mySlides fade">
      <img src="/img/portfolio/blocmarks_3.png" style="width:100%">
    </div>

    <div class="mySlides fade">
      <img src="/img/portfolio/blocmarks_5.png" style="width:100%">
    </div>

    <div class="mySlides fade">
      <img src="/img/portfolio/blocmarks_6.png" style="width:100%">
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

To allow **Blocmarks** users to sign up and send emails for account confirmation I used the [Devise gem](https://github.com/plataformatec/devise){:target="_blank"} for authentication and implemented user sign in/out.

I created an index of all topics and their bookmarks and implement CRUD to allow users to create, delete and update topics and bookmarks.

To email a URL to **Blocmarks** and have it saved in the database I useed [Mailgun](https://www.mailgun.com/) to configure **Blocmarks** to receive an email containing a bookmark URL. I parsed and converted incoming emails into bookmark objects that belong to a topic.

I used the [Pundit](https://github.com/elabs/pundit){:target="_blank"} gem for authorization to make the user the only one allowed to delete and update their bookmarks & topics (only if there are no bookmarks created by someone else)

I implemented liking & unliking bookmarks and created User Profiles to see a list of bookmarks on personal profiles that have been added and or liked.

With [Embedly](http://embed.ly/){:target="_blank"} I created URL previews for each bookmark and used [FriendlyId](https://github.com/norman/friendly_id){:target="_blank"} for the **Blocmarks** to have pretty & readable URLs.
