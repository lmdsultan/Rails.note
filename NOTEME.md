1. Create db within your Rails app --> rake db:create
2. Create a Movie model --> rails g model Movie (your model name should be single/capital)
3. Add a name column to the Movie model --> rails g migration AddNameToMovies
4. To get a list of your migrations --> rails db:migrate:status
5. To start migrations --> rails db:migrate
6. To rollback/undo a migration --> rails db:rollback
7. To rollback/undo multiple migrations --> rails db:rollback STEP=2 (2 is an example number of migrations to roll back)
8. To destroy the whole databse --> rails db:drop
9. To create a new controller with index, new, show, and edit methods --> rails g controller ControllerName index new show edit (your controller should be plural and capital)
10. To destroy a controller --> rails destroy controller ControllerName
11. Show all the possible Rails commands --> rails
12. Show all available routes --> rails routes
13. Enter the console --> rails c
14. Start the server --> rails s
15. To seed your database --> rails db:seed

=========================================================================================================

Devise : https://github.com/plataformatec/devise#getting-started
1- create new app ~> rails new devise-app -d=postgresql

2- Then cd devise-app , create db inside rails ~> rails db:create
3- Add the following line to your Gemfile  file
gem 'devise'
4- in the terminal ~> bundle install

5- Next, you need to run the generator: rails generate devise:install

6- Inside file of config/environments/development.rb: insert this line
config.action_mailer.default_url_options = { host: 'localhost', port: 3000 }

7-  Ensure you have defined root_url to *something* in your config/routes.rb
root to: "home#index"

8- Make new Controller called Home ~> home_controller.rb  with method called index

9- make new folder called Home ~> inside the folder create file called index.html.erb

10-  Inside view put these lines in file layout application.html.erb
       <p class="notice"><%= notice %></p>
       <p class="alert"><%= alert %></p> 
              
11- Then run rails g devise:views in the terminal to make view pages for all devise ex: sign-up , sign-in ..etc

12 - rails generate devise <Name of Model> to create model called User ~> rails generate devise User
       
13- Then rails db:migrate

14-  Restart the server (edited) 
