# Guessing Game

### Layout Scope
>- Create a `index.html` file
  - Make a `html` skeleton
  - Make sure to give your page an appropriate title
- Add a set of `script` tags
  - This will hold your javascript code
- Add an input field
  - This input field will take the user's guess
  - Give it an id of `guess_input`
- Add a div
  - This `div` will hold any feedback from the game to the user
  - Give it an id of `response_div`
- Add a button
  - This button will submit the user's guess to the game

### Functional Scope
>- In your script tag, make a variable, called `the_number`, set its value to `null`
- Add a on load handler to the body
  - It should call a function named `pick_number` and assign its return value to the variable `the_number`
- In your script tag, make a function called `pick_number`
    - It takes no parameters
    - It returns a number
    - Inside:
      - It will creates a variable, called `random_number`
      - It will generate a random number between 1 and 10, and then assigns it to the `random_number` variable
      - return `random_number`
- Add a click handler to the button using jQuery.  
  - This click handler will call a function named `make_guess`
- Add a function to your script tags
  - Name it `make_guess`
  - It takes no parameters
  - It returns no values
  - Inside:
    - It will grab the value of the input from above and assign it to a variable named `the_guess`
    - It then compares the variable `the_guess` to the variable `the_number`
      - If `the_guess` is higher than `the_number`, it changes the contents of `#response_div` to **"too high!"**
      - If `the_guess` is lower than `the_number`, it changes the contents of `#response_div` to **"too low!"**
      - If `the_guess` is the same as `the_number`, it changes the contents of `#response_div` to **"You guessed it!"**
