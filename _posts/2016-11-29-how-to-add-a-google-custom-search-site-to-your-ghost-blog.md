---
layout: post
title: How to add a Google Custom Search site to your Ghost blog
---
I could already tell from the search results, adding a Google Custom search box to your Casper theme on your Ghost blog, might not be as straight forward as promised in the tutorials. <br />
I didn't like the look and feel of it on my main page, so I chose to make an extra static search site.

### Create a Google Custom search engine
To add in Google Custom search, you first need to create a search engine for your site. You can do this by going to Google's [Custom Search](https://cse.google.com/cse/create/new) site.

![Screenshot Google Custom Search]({{ site.baseurl }}/img/posts/ScreenShotGoogleCustomSearch.png)

If you'd like your entire blog to be searched, you will need to type in  yoursubdomain.ghost.io/* into the "sites to search" field. Please note the * at the end of the URL. <br />
When you've finished, give your search engine a name, then click the blue "Create" button to continue the process of setting up your custom search engine.

![Screenshot Google Custom Search Success]({{ site.baseurl }}/img/posts/ScreenShotGoogleCustomSearchSuccess.png)

After you've created the custom search engine, you will be taken to a screen that provides you with several options. Select the "get code" button next to the "Add it to your site" option. <br />
Upon clicking the "get code" button, you should be directed to a screen with your custom search engine code.


### Create a static search page
Creating a static search page in Ghost is very similar to creating a post, but it will not show up in your blog post collection on the main site.

![Screenshot Search Ghost Editor]({{ site.baseurl }}/img/posts/ScreenShotSearchEditor.png)

You log in to your blog admin, then click on New Post from the navigation menu on the left and should be on the Ghost editor screen. Simply call your site **Search** in the title and add whatever content you like.

Once you’ve completed writing your page content, you need to designate it as a static page. By clicking “gear” icon in the top right hand corner, the post settings menu is revealed, which controls post details and whether or not the content should be set as a static page.

In this case, we’d like this content to appear as a page, therefore we’ll need to check the empty box next to “Turn this post into a static page”, as shown in the screenshot above.

*Note:The URL of your page will default to the title of the page, broken down using hyphens (i.e. your-page). If you want to change this, simply click inside the URL field and begin typing. You will need to remember this URL if you are planning to link to it within your theme or other posts.*

Publish your static search page by clicking the Save button in the bottom right hand corner of your screen. Beside it, you will see an arrow. Click on the arrow to change the action of the button to Publish Now. The button will turn red. Click on the button again to publish your static page. You will get a success notification once it is live on your blog.


### Create a custom page template

![Screenshot Search Atom Editor]({{ site.baseurl }}/img/posts/ScreenShotAtom.png)

Now that we've created a static page, we'll need to create a custom page template inside our theme. <br />
To do this, first create a new file within your theme's root directory. Page templates must always start out with 'page-' and then include the page URL after the hyphen. So, for example: If you have a contact page with a page URL of "contact" your page template name would be `page-search.hbs`.

Copy the code from your `page.hbs` file. <br />
Once you've created your page template you'll need add some code to it. Copy the code from your theme's `page.hbs` file and paste it into your new page template. When you're finished, save the page template file. We will access this template file again once we've created our form.

Paste the embed code into your page template. <br />
Copy and paste the provided code, we've created earlier with Google's [Custom Search](https://cse.google.com/cse/create/new), into a `<div>` element, where you want both the search box and the search results to render.

#### Save your page template
Once you've placed your embed code into the contact page template, save your template file.

#### Upload the theme to your Ghost blog
Once saved, upload the theme to your blog. Now, when you view your search page you should see your search box.

![Screenshot Search Ghost Blog]({{ site.baseurl }}/img/posts/ScreenShotSearchBlog.png)

### Yay!
