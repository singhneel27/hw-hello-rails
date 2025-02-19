<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>hw-hello-rails</title>
</head>
<body>
    <h1>hw-hello-rails</h1>
    <p>This is a simple Ruby on Rails application designed to manage and display a collection of movies.</p>

    <h2>Prerequisites</h2>
    <p>Before you begin, ensure that you have the following software installed:</p>
    <ul>
        <li><strong>Ruby</strong> (version 3.4.1):<br>Check your installed Ruby version by running:
            <pre>ruby -v</pre>
            If you don't have Ruby installed, you can install it by following the instructions at <a href="https://www.ruby-lang.org/en/documentation/installation/" target="_blank">Ruby Official Installation Guide</a>.
        </li>
        <li><strong>Rails</strong> (version 8.0.1):<br>Check your installed Rails version by running:
            <pre>rails -v</pre>
            If you don't have Rails installed, run the following command to install it:
            <pre>gem install rails</pre>
        </li>
        <li><strong>Database System</strong>:<br>The application is compatible with PostgreSQL, MySQL, or SQLite (SQLite is the default for development).<br>Ensure you have a database system installed and configured for your environment. You can find installation instructions for each system here:
            <ul>
                <li><a href="https://www.postgresql.org/download/" target="_blank">PostgreSQL Installation Guide</a></li>
                <li><a href="https://dev.mysql.com/downloads/" target="_blank">MySQL Installation Guide</a></li>
                <li><a href="https://www.sqlite.org/download.html" target="_blank">SQLite Installation Guide</a></li>
            </ul>
        </li>
    </ul>

    <h2>Setup</h2>
    <ol>
        <li><strong>Clone the repository</strong>:<br>Clone the repository to your local machine:
            <pre>git clone https://github.com/your-username/hw-hello-rails.git
cd hw-hello-rails</pre>
        </li>
        <li><strong>Install dependencies</strong>:<br>Install the required Ruby gems by running:
            <pre>bundle install</pre>
        </li>
        <li><strong>Configure the database</strong>:<br>Before running the application, ensure your database is correctly configured in the <code>config/database.yml</code> file for the appropriate environment (<code>development</code>, <code>test</code>, or <code>production</code>).
        </li>
        <li><strong>Create the database</strong>:<br>Run the following command to create the database:
            <pre>bin/rails db:create</pre>
        </li>
        <li><strong>Initialize the database with seed data</strong>:<br>If you want to populate the database with some initial data (like default movies), run:
            <pre>bin/rails db:seed</pre>
        </li>
    </ol>

    <h2>Running the Application</h2>
    <p>Once the setup is complete, you can start the Rails server with:</p>
    <pre>bin/rails server</pre>
    <p>By default, the application will be accessible at <a href="http://localhost:3000" target="_blank">http://localhost:3000</a>.</p>

    <h2>Deployment Instructions</h2>
    <p>If you want to deploy the application to a cloud platform like Heroku, follow these steps:</p>
    <ol>
        <li><strong>Install the Heroku CLI</strong>:<br>If you don't have the Heroku CLI installed, you can download it from <a href="https://devcenter.heroku.com/articles/heroku-cli" target="_blank">Heroku CLI Documentation</a>.</li>
        <li><strong>Create a new Heroku app</strong>:<br>Run the following command to create a new Heroku application:
            <pre>heroku create your-app-name</pre>
        </li>
        <li><strong>Add a PostgreSQL database</strong>:<br>If you're using PostgreSQL, add the Heroku PostgreSQL add-on with:
            <pre>heroku addons:create heroku-postgresql:hobby-dev</pre>
        </li>
        <li><strong>Deploy the application to Heroku</strong>:<br>Push your code to Heroku by running:
            <pre>git push heroku master</pre>
        </li>
        <li><strong>Run migrations on Heroku</strong>:<br>Apply any pending migrations to the Heroku database by running:
            <pre>heroku run bin/rails db:migrate</pre>
        </li>
        <li><strong>Open the application</strong>:<br>Once everything is deployed, open your application in the browser with:
            <pre>heroku open</pre>
        </li>
    </ol>

    <h2>Additional Notes</h2>
    <ul>
        <li>The application uses <strong>SQLite</strong> by default for development. You can switch to a different database system (such as PostgreSQL or MySQL) by modifying the <code>config/database.yml</code> file.</li>
        <li>If you encounter any issues, refer to the <a href="https://guides.ruby-on-rails.org/" target="_blank">Rails Guides</a> for troubleshooting and further configuration.</li>
    </ul>

    <h2>License</h2>
    <p>This project is licensed under the MIT License - see the <a href="LICENSE.md" target="_blank">LICENSE.md</a> file for details.</p>

</body>
</html>
