# Rotten Potatoes

This repository contains the Rotten Potatoes application, a movie review platform built using Ruby on Rails.

## Application Link:
https://rottenpotatoesns-835a2dba8950.herokuapp.com/

## Prerequisites
Before running the application, ensure you have the following installed:

### System Dependencies
- **Ruby** (Version 3.4.1) - Check your Ruby version using:
  ```sh
  ruby -v
  ```
  If Ruby is not installed, download it from [ruby-lang.org](https://www.ruby-lang.org/).

- **Rails** (Version 8.0.1) - Verify your Rails version using:
  ```sh
  rails -v
  ```
  If Rails is not installed, run:
  ```sh
  gem install rails
  ```

- **Database System**: The application supports **PostgreSQL, MySQL, or SQLite** (SQLite is used by default for development).

## Configuration
Ensure your database is properly configured in `config/database.yml` based on the environment (development, test, or production).

## Setup Instructions
### 1. Clone the Repository
```sh
git clone https://github.com/singhneel27/hw-hello-rails.git
cd hw-hello-rails
```

### 2. Install Dependencies
```sh
bundle install
```

### 3. Database Setup
#### Create the Database
```sh
bin/rails db:create
```
This will generate the necessary databases.

#### Apply Migrations
```sh
rails db:migrate
```

#### Seed the Database
If you need to populate the database with default records (e.g., movies with titles, ratings, and release dates), run:
```sh
rails db:seed
```

## Running the Application
Start the Rails server using:
```sh
rails server
```
By default, the server will be hosted at:
```
http://127.0.0.1:3000
```

## Contributing
Feel free to submit issues and pull requests to improve this project.

---
### Repository: hw-hello-rails

