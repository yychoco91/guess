# Guessing Game

### Layout Scope
- Add a set of script tags
  - this will hold your javascript code
- Add an input field
  - this input field will take the user's guess
  - give it an id of "guess_input"
- Add a div
  - this div will hold any feedback from game to the user
  - give it an id of "response_div"
- Add a button
  - this button will submit the user's guess to the game

### Functional Scope
- In your script tag, make a variable, called 'the_number', set it's value to null
- Add a on load handler to the body
  - it calls the function "pick_number" and assigns its return value to the variable "the_number"
- In your script tag, make a function called "pick_number"
    - it takes no parameters
    - it returns a number
    - inside
      - it creates a variable, called random_number
      - it gets a random number between 1 and 10, and assigns it to random_number
      - return random_number
- Add a click handler to the button.  
  - This click handler will call a function, "make_guess"
- Add a function to your script tags
  - name it make_guess
  - it takes no parameters
  - it returns no values
  - inside
    - it grabs the value of the input from above and assigns it to a variable "the_guess"
    - it compares the variable "the_guess" to the variable "the_number"
      - if the_guess is higher, it changes the contents of #response_div to "too high!"
      - if the_guess is lower, it changes the contents of #response_div to "too low!"
      - if the_guess is the same as the_number, change the contents of #response_div to "You guessed it!"
