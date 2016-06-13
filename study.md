# Rails as an API Study

Use your favorite search engine and the provided readings to research and answer
the following questions (no prior knowledge is expected).

In your answers, be sure to cite any relevant sources you consulted in your
search. We ask you to write answers in your own words in order to see how you
process what you've read. Please do not answer with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Please note:

-   Many of the readings will mention the "view" layer. We won't be covering the
    view layer in this program.
-   We'll use our [rails-api-template](/ga-wdi-boston/rails-api-template)
    repository as the basis for our rails applications.
    This template excludes the "view" layer.

## Required Readings

-   [Starting Ruby on Rails: What I Wish I Knew | BetterExplained](http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/)
-   [Intermediate Rails: Understanding Models, Views and Controllers | BetterExplained](http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/)
-   [Getting Started with Rails — Ruby on Rails Guides](http://guides.rubyonrails.org/getting_started.html)
-   [The Rails Command Line — Ruby on Rails Guides](http://guides.rubyonrails.org/command_line.html)
-   [Rails Routing from the Outside In — Ruby on Rails Guides](http://guides.rubyonrails.org/routing.html)
-   [Action Controller Overview — Ruby on Rails Guides](http://guides.rubyonrails.org/action_controller_overview.html)

## Define Model Responsiblities

In your own words, define what the responsibilities of the model layer are in
Rails.

```md
<!-- your answer here -->
HANDLES DATA

A model are basically all the ruby classes and objects:

- communicate with database
- store information
- validate data
```

## Define Controller Responsiblities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
<!-- your answer here -->
HANDLES DECISIONS
Controllers take user input and make decision what to do with it:

- passing it to the model
- then passing the output to the view
```

## Define Router Responsiblities

In your own words, define what the router does in Rails.

```md
<!-- your answer here -->
The router recorgnize URLs and sends them to the controller. It can generate URLs so you don't need to code the absulute path in the view.

The router looks at the HTTp verb and the URL and matches it with the right controller action.

source: http://www.theodinproject.com/ruby-on-rails/routing
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
<!-- your answer here -->
1. The browser(client) send information(user input) to the Controller.
2. Controller makes decsion about what to do:
  - it might connect to the Model
3. The Model can interact with a database (sending, receving data etc.) and send that back to the Controller.
4. Once the controller is satisfied and think it can process the user request, it sends all the infromation needed to the View.
5. The View decides which HTML,CSS, Javascript will get returned to the browser


```
