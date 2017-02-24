---
layout: post
title: Blocitoff
thumbnail-path: "img/blocitoff.png"
short-description: Build a self-destructing to-do list application.

---

{:.center}
![]({{ site.baseurl }}/img/blocitoff.png)

## Explanation

Blocitoff is a self-destructing to-do list application using Ruby on Rails. Users add items to to-do lists, and items are automatically deleted after seven days. This self-destructing functionality is designed to keep the list manageable: users must prioritize and complete items or let them go.



Blocitoff allows users to create self-destructing to-do lists. Items are automatically deleted after seven days. The hypothesis is that if the to-do items is not important enough to be completed after seven days, it doesn’t belong on your to-do list.

It allows users to create a free account, sign in, and make to-do lists that clear items out for you after a week so they don't get too cluttered!

In Blocitoff I used  features such as the Devise gem for creating users and Bootstrap to pretty things up. Some new things I learned (or did on my own for the first time in this project) included:

        using the faker gem to seed data instead of the random_data file from my versions of Bloccit and Blocipedia
        using Ajax to add and delete items off the to-do list without refreshing the page
        displaying the time from when the item was created to when it will be deleted
        creating custom rake tasks to delete all to-do items over seven days old

        Blocitoff Is a simple To-do list app using Ruby on Rails. It allows users to create lists of things they need to complete, with a self-disruptive that functions as way to help you complete your goals in 7 days or less.



## Problem

But I did struggle with implementing Ajax to refresh the to-do list without refreshing the page.

Everyone uses to-do lists. The issue that arises out of a personal to-do list is that we put things off and we say that it will get done “tomorrow”.

To-do lists are easily to make but harder to get them done when it comes to it. The "Ill just do it later" attitude always seems to arise when it comes to finishing off something we have put asside but Blocitoff hopes to help by implementing its self-disruptive feature.

## Solution

The solution was something my mentor and I went over a few weeks ago in regards to the Bloccit introductory project: pointing to the right part of the site to refresh. Initially, my JavaScript file was pointing to the checkmark that says you've completed a to-do item rather than the text of the to-do item itself. I created an ID specific to the to-do items that fixed the issue.


Users can have multiple do-items
A user can mark to-do items as complete and have item deleted
User can see how many days items remain before automated deleted
Items are automately deleted after seven days


This application hopes to remedy some of those issues by self-destructing to-do items that are a week old. The philosophy is that you should do it within a week, and if you don’t you probably will never get around to it. This makes users more accountable for their to-do items, and forces them to think of completing things that are going to be destroyed soon.

The self-disruptive feature in Blocitoff is implemented to automatically delete to-do item that weren't completed within 7 days of it being created. It is implemented by creating a rake task like so :

{% highlight ruby %} desc "Delete Expired Items (7 days)" task delete_items: :environment do Item.where("created_at <= ?", Time.now - 7.days).destroy_all end {% endhighlight %}


## Results

I find that using the Blocitoff utility did want me to complete tasks before a week was over.

As a result Blocitoff allows the user to create and manage their to-do items as well as encouraging the user to complete them before they expire. Blocitoff was my first project going solo and it allowed me to follow a User Story tool to complete the tasks that was ask for.



Bacon ipsum dolor amet filet mignon meatball spare ribs fatback bacon shankle. Kielbasa andouille fatback salami, boudin bresaola pig alcatra turkey spare ribs jerky. Corned beef bresaola leberkas salami alcatra beef landjaeger venison shank bacon meatloaf beef ribs picanha. Leberkas sausage brisket porchetta shankle prosciutto chicken picanha kielbasa pig kevin t-bone turducken filet mignon jowl.

> Bacon ipsum dolor amet filet mignon meatball spare ribs fatback bacon shankle. Kielbasa andouille fatback salami, boudin bresaola pig alcatra turkey spare ribs jerky. Corned beef bresaola leberkas salami alcatra beef landjaeger venison shank bacon meatloaf beef ribs picanha. Leberkas sausage brisket porchetta shankle prosciutto chicken picanha kielbasa pig kevin t-bone turducken filet mignon jowl.

Bacon ipsum dolor amet filet mignon meatball spare ribs fatback bacon shankle. Kielbasa andouille fatback salami, boudin bresaola pig alcatra turkey spare ribs jerky. Corned beef bresaola leberkas salami alcatra beef landjaeger venison shank bacon meatloaf beef ribs picanha. Leberkas sausage brisket porchetta shankle prosciutto chicken picanha kielbasa pig kevin t-bone turducken filet mignon jowl.

## Conclusion

Overall with this project I learned a lot about Ruby and Rails

I have found that this is a very useful application to utilize in a multitude of ways. In addition to serving as a template, this also provides a variety of rspec tests that may be applied to all CRUD actions.

I feel much prouder of my work on Blocitoff than my work on Blocipedia even though I feel like Blocipedia was a tougher project. I ran into a handful of snags, but I feel as though I've gotten more adept at problem-solving on my own without having to have things shown to me directly. There will always be new challenges, of course, but Blocitoff has given me more confidence as a developer that should help me keep moving forward in my next Ruby on Rails project!

Bloccitoff was a good introduction to rake tasks that could be run manually or automatically. I also playing around with some Ajax to implement a more smooth experience when marking to-do items as complete.
