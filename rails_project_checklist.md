# Rails project checklist:

## From Scratch
- check git config for `user.name` and `user.email`
- check local Rails version `rails -v`
- create rails project: `rails new project_name`
  - EXCEPTION: planning on deploying to Heroku
    - Set default database to postgres: `rails new -d postgresql`
    - too late? See ["SQLite on Heroku"](https://devcenter.heroku.com/articles/sqlite3)
- create RESTful resources in routes.rb
- models
  - e.g. `class Category < ApplicationRecord`
  - associations
- migrations
  - e.g. `rails g migration CreateZombiesTable name:string, body:text`
- bin/rails db:migrate
- If using seeds
  - create seeds file
  - bin/rails db:seed
- controllers
  - e.g. `class CategoriesController < ApplicationController`
  - Add RESTful actions (ISNECUD)
    - index
    - show
    - new
    - edit
    - create
    - update
    - destroy
- views
  - e.g. index.html.erb
  - [RoR Guide: Helpers for nested routes](http://guides.rubyonrails.org/routing.html#controller-namespaces-and-routing)

## More Resources
- [CodeSchool Rails Cheatsheet](http://courseware.codeschool.com/rails_for_zombies_2_cheatsheets.pdf)
- [Rails Blog Tutorial](http://guides.rubyonrails.org/getting_started.html)
- @reedr3's [Rails Views guide](https://docs.google.com/presentation/d/1YnQ60gS43gvF4rlrQBIGzItQXdptHyHJgJ3au4zJLVU/edit#slide=id.g16a951c5c0_0_58)
