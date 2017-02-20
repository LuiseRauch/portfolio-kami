---
layout: post
title: Blocmarks
thumbnail-path: "img/blocflix.png"
short-description: Social Bookmarking With Email - a production quality social bookmarking app that allows users to send, manage, and share bookmarks.

---
https://afternoon-hollows-1410.herokuapp.com
{:.center}
![]({{ site.baseurl }}/img/blocflix.png)

## Explanation

 This is a social bookmarking site that allows users to browse topics and bookmarks created by others. Users are also able to add bookmarks to topics they've created or add on to topics created by others. Users are also able to favorite bookmarks created by others and have them added to their profile.


## Problem


blocmarks allowed me to stash bookmarks according to topics. An easy way to navigate and find what I needed to reference I a few clicks.

 many users carry in a large library of bookmarks.

 It would be nice to have the ability to share bookmarks with friends.

## Solution

 to send emails to blocmarks to create new bookmark entries in the database. implement and configure Mailgun to receive incoming emails. The email needs only the topic in the subject and the url in the body to be parsed and stored by blocmarks.

> Liking bookmarks allowed users to remember which bookmarks owned by others they liked. The liked bookmarks would then be placed along with their own in their user profile for easy reference.

Blocmarks will solve these problems by organizing bookmarks by topic and making them public so that other users can find them and add bookmarks to their own Blocmarks profile.


## Results

 When I started the project I was concerned if blocmarks was going to be useable at completion. The large amount of bookmarks people had was going to be a barrier for adoption. The CSV uploader and saving bookmarks from received email neutralized this fear instantaneously.


## Conclusion

I will definitely keep email and database integration present for all of my future projects.

The major learning objective for this app was to continue to build off of my introduction to test-first development in Blocipedia. I also wanted to focus more on Front-end development to create an improved user experience. To do this I challenged myself to implement a new Front-end framework, Zurb Foundation, and also utilize Sass(CSS pre-proccessor) for cleaner more modular stylesheets.

This application was a great experience as it challenged me to learn and utilize new technologies, such as Sass, the Embed.ly API, and a New Front-end Framework. Learning new technologies has it's challenges, but may be the thing I find most rewarding and exciting about the world of web-development. In web development, there is a never ending desire to improve our current tool-set, build things that make development faster and more enjoyable, and push the limits of what we think is possible.
