# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version
The application uses 3.4.1 version, check the ruby version using `ruby -v` command.
* Rails version
The application uses 8.0.1 Rails version, check the version using `rails -v` command. If no rails, run `gem install rails`
* System dependencies
Before running the application, make sure you have the following system dependencies:

Ruby (version 3.4.1)
Rails (version 8.0.1)
A database system such as PostgreSQL, MySQL, or SQLite (SQLite is default for development)
Make sure you have these installed on your system.
* Configuration
Make sure your database is configured in config/database.yml for the environment you’re working in (development, test, or production).
* Database creation
Create and set up the database by running the following commands:
bin/rails db:create
This will create the necessary databases for your application.
* Database initialization
If you need to populate the database with some initial data, you can run the seed file with:
bin/rails db:seed
This will load default records into your database, such as movies with title, rating, and release date.

* Deployment instructions
To deploy this application to Heroku (or any platform), follow these steps:
1. Install the Heroku CLI (if not already installed).

2. Create a new Heroku application:
heroku create your-app-name
3. Add a PostgreSQL database (if using PostgreSQL):
heroku addons:create heroku-postgresql:hobby-dev
4. Deploy to Heroku:
git push heroku master
5. Run migrations on Heroku:
heroku run bin/rails db:migrate
6. Open the application:
heroku open


* ...
# hw-hello-rails
