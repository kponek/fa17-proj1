# Q0: Why is this error being thrown?
We haven't created the HomeController, so when we try to route to home#index, the app does not know where to go

# Q1: How are the random Pokemon appearing? What is the common factor between all the possible Pokemon that appear?
Random pokemon are appareaing because we called seeds.rb to make trainerless pokemon.  The common factor is that the index method in HomeController gets all pokemon where the trainer attribute is nil.

# Question 2a: What does the following line do "<%= button_to "Throw a Pokeball!", capture_path(id: @pokemon), :class => "button medium", :method => :patch %>"? Be specific about what "capture_path(id: @pokemon)" is doing. If you're having trouble, look at the Help section in the README.
It creates a button named "Throw a Pokeball". When the button is clicked it redirects to the capture path which is defined in routes. It executes the capture method in the pokemon controller and passes the current pokemon for the parameter ID so that the capture method can identify the pokemon with the id parameter.

# Question 3: What would you name your own Pokemon?
Swegmonstar

# Question 4: What did you pass into the redirect_to? If it is a path, what did that path need? If it is not a path, why is it okay not to have a path here?
I passed trainer_path, but also added current_trainer.id to params as :id

# Question 5: Explain how putting this line "flash[:error] = @pokemon.errors.full_messages.to_sentence" shows error messages on your form.
Everytime the interpreter runs the files, it runs application.html.erb. This file runs all the error conditions and makes a display error message. The if condition in the create new pokemon method checks if the pokemon is saved successfully.

# Give us feedback on the project and decal below!
Project was great, I loved how it walked me through the steps to the project instead of just leaving me with nothing to work with.  I felt that it was hard to retain some of the material in the course, but this project helped me put together everything that we've learned so far!

# Extra credit: Link your Heroku deployed app
