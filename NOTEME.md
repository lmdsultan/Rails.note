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
