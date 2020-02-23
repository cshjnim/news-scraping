# news-scraping


# Contributor 
Created By: Hyejin Kim, Creator

Date: February 16,2020
- - -


### Overview

"In this assignment, you'll create a web app that lets users view and leave comments on the latest news. But you're not going to actually write any articles; instead, you'll flex your Mongoose and Cheerio muscles to scrape news from another site."

### Instructions

* Create an app that accomplishes the following:

  1. Whenever a user visits your site, the app should scrape stories from a news outlet of your choice and display them for the user. Each scraped article should be saved to your application database. At a minimum, the app should scrape and display the following information for each article:

     * Headline - the title of the article

     * Summary - a short summary of the article

     * URL - the url to the original article

     * Feel free to add more content to your database (photos, bylines, and so on).

  2. Users should also be able to leave comments on the articles displayed and revisit them later. The comments should be saved to the database as well and associated with their articles. Users should also be able to delete comments left on articles. All stored comments should be visible to every user.

* Beyond these requirements, be creative and have fun with this!

### Tips

* Go back to Saturday's activities if you need a refresher on how to partner one model with another.

* Whenever you scrape a site for stories, make sure an article isn't already represented in your database before saving it; Do not save any duplicate entries.

* Don't just clear out your database and populate it with scraped articles whenever a user accesses your site.

  * If your app deletes stories every time someone visits, your users won't be able to see any comments except the ones that they post.



### SCREENSHOTS

* deployed Screenshot: 

![Screenshots](/public/assets/img/news-scrapping.png)


- - -

### Links & Portfolio's Links
*  [Deployed page](https://news-scrapping-cshj.herokuapp.com/)
*  [Hyejin's Portfolio](https://cshjnim.github.io/)

- - -

### Summary of Technologies Used on this project

* Javascript
* Git
* GitHub
* Heroku
* Node
* JSON
* NPM Packages
* handlebar
* mongoose
* cheerio
* axios


- - -

### CHECKLISTS

1. Clearly state the problem the app is trying to solve (i.e. what is it doing and why) &check;
2. Give a high-level overview of how the app is organized &check;
3. Give start-to-finish instructions on how to run the app &check;
4. Include screenshots, gifs or videos of the app functioning &check;
5. Contain a link to a deployed version of the app &check;
6. Clearly list the technologies used in the app &check;
7. State your role in the app development &check;


4. In order to deploy your project to Heroku, you must set up an mLab provision. mLab is remote MongoDB database that Heroku supports natively. Follow these steps to get it running:

5. Create a Heroku app in your project directory.

6. Run this command in your Terminal/Bash window:

* `heroku addons:create mongolab`

* This command will add the free mLab provision to your project.

7. When you go to connect your mongo database to mongoose, do so the following way:

```js
// If deployed, use the deployed database. Otherwise use the local mongoHeadlines database
var MONGODB_URI = process.env.MONGODB_URI || "mongodb://localhost/mongoHeadlines";

mongoose.connect(MONGODB_URI);
```

* This code should connect mongoose to your remote mongolab database if deployed, but otherwise will connect to the local mongoHeadlines database on your computer.

8. [Watch this demo of a possible submission](https://youtu.be/4ltZr3VPmno). See the deployed demo application [here](http://nyt-mongo-scraper.herokuapp.com/).

9. Your site doesn't need to match the demo's style, but feel free to attempt something similar if you'd like. Otherwise, just be creative!

### Hosting on Heroku

Now that we have a backend to our applications, we use Heroku for hosting. Please note that while **Heroku is free**, it will request credit card information if you have more than 5 applications at a time or are adding a database.

Please see [Heroku’s Account Verification Information](https://devcenter.heroku.com/articles/account-verification) for more details.

---
