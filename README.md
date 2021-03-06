# Flatiron Fantasy Football

Welcome to the Flatiron Fantasy Football game. Here you can log in or sign up for a contest, view the player analytics ,view your score and win prize.However a user who is an admin can create a team.

## Ruby Version:

We are using `Ruby Version 2.6.1` for our application

## System Dependencies

 `gem'bcrypt'`, `gem 'fantasy_football_nerd'`( for API data) and `gem'csv'`(for CSV data) was added in our gemfile.

## Setup:
* Fork and clone the repository

* Prior to starting the server, run bundle install, rails db:migrate and   
  rails db:seed.
  Bundler gem is already installed so running bundle install would install rails and all its dependencies.

* Next open the rails console with rails c.

* Run the methods Player.update_salary_modifiers to update salary_modifier 
  columns in the players table.

* The seed file will update with scores for players for Week 1-3. If at a future date you would like to add scores for newer weeks, download the new week's csv from https://www.fantasypros.com/nfl/reports/leaders/ and save it in the storage folder as "points_week_#weeknumber.csv" then run Contest.new_scores_for_week(#weeknumber) in rails c to update the database.


## Creating Database:

* Gnerate tables and controllers by
`rails g resource modelname colname:datatype` 

* Create associations in the modelname.rb and then run `rails db:migrate` and after creating seeds in seeds.rb file run `rails db:seed`.

* Our database is setup.

* to test out associations run `rails c` and test out the associations.

## Validations:

* Create validations inside the model.rb file.

## Running the application:

* We are using Behavior Driven Development.

* To run our application type `rails s` and then type `localhost:3000` in the browser.

* To check a specific webpage type specific url/route after localhost:3000 to view the corresponding webpage example  run `localhost:3000/contests` to checkout the contests or main page.

* If you get error running the application try clearing out the login session from the cookie editor.


Our model follows single responsibility principle and most of our logic is in our models

 # Acknowledgements
Our instructors Ix and Adam

# Created By
Andrew Mullan https://github.com/MullaN
Arpita Dutta https://github.com/Arpita-22
Margarita Morozova https://github.com/rita-morozova

