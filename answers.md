# Q0: Why is this error being thrown? 
#	  The controller PokemonController hasn't been generated yet.

# Q1: How are the random Pokemon appearing? What is the common factor between all the possible Pokemon that appear? *
#	The seed file generates four pokemon, Bulbasaur, Squirtle, Charmander and Pikachu, each with a random level between 1 and 20  but with no trainer id declared. Then, in the home controller, the pokemon field is set to the list of all pokemon without trainer ids attached. So, the wild pokemon are all seeded pokemon without trainers.

# Question 2a: What does the following line do "<%= button_to "Throw a Pokeball!", capture_path(id: @pokemon), :class => "button medium", :method => :patch %>"? Be specific about what "capture_path(id: @pokemon)" is doing. If you're having trouble, look at the Help section in the README.

# Question 3: What would you name your own Pokemon?
Pokeman

# Question 4: What did you pass into the redirect_to? If it is a path, what did that path need? If it is not a path, why is it okay not to have a path here?
I passed a string for a path to redirect_to. The path needed the trainer's id to decide which trainer show page to direct to. 

# Question 5: Explain how putting this line "flash[:error] = @pokemon.errors.full_messages.to_sentence" shows error messages on your form.
applications.html.erb will render _messages.html.erb, which will in turn flash an alert message if there exists one. The line in the question is what makes sure the alert message is not nil.

# Give us feedback on the project and decal below!

# Extra credit: Link your Heroku deployed app
