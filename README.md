Week 4 Lab - Rails Dynamic Pages
-------------------------------

Goals:
----

* Able to create a rails app
* Style the rails app using the asset pipeline
* Use the Router (config/routes) to have a dynamic set of pages
* Pass data from the controller to the views to render


Requirements:
----

1. Craft a Rails app that shows your Surf and Paddle (can expand from day 18)
1. Make the pages dynamic, where:
  * The root page shows the latest post
  * The images at the bottom of the page link link to that post
  * When viewing that post (URL will be /posts/:name) it shows that post


posts should be something like this:

```ruby
@posts = []
@posts << Post.new("waffles", "waffles.jpg", "waffles are the best...")
@posts << Post.new("pancakes", "pancakes.jpg", "pancakes are the best...")
@posts << Post.new("bacons", "bacon.jpg", "bacon is the best...")
```

Notes:
-----

* To find an element in your `@posts` array, use `@posts.find {|p| p.permalink
  == params[:permalink]}` or similar
* There is no database in this lab, but we will have databases next week.


Nightmare Mode
---

1. Add a list of the top 20 most populated cities in the world.
2. When you click on the each city, it should go to `/houston/weather`
3. On the weather page, you should connect to a weather service API (in ruby)
   and display the most current weather information for that city. (humidity,
   rain probability, and temperature)
4. On the weather page, display a high res photo of that city over the entirety
   of the screen (cover). 


