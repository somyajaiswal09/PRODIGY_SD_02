### Algorithm 

1. **Initialize Game**:

   * Generate a random number between a predefined range (e.g., 1 to 100).
   * Set an initial guess counter to 0.

2. **User Input**:

   * Prompt the user to guess the number.
   * Validate the input to ensure it is a valid integer within the specified range.

3. **Comparison**:

   * If the guess is correct, print a success message with the number of attempts.
   * If the guess is too low, print a message and prompt for a higher guess.
   * If the guess is too high, print a message and prompt for a lower guess.

4. **Loop**:

   * Repeat steps 2 and 3 until the user guesses the correct number.

5. **Exit Game**:

   * After a correct guess, display a message indicating the number of attempts and exit the game.

---

### Skills Used:

1. **Programming Language**:

   * C for game implementation.

2. **Random Number Generation**:

   * `rand()` function (along with `srand(time(NULL))`) to generate a random number.

3. **User Input**:

   * `scanf()` for user input and validating it.

4. **Loops**:

   * `while` or `do-while` loop to repeatedly prompt the user until they guess correctly.

5. **Conditionals**:

   * `if-else` statements to check whether the guess is too high, too low, or correct.

6. **Input Validation**:

   * Check if the user input is within the valid range and handle invalid inputs.

7. **Basic Output**:

   * `printf()` to display messages to the user.

8. **Data Handling**:

   * Integer variables for storing random numbers, user guesses, and the count of attempts.

9. **Time Handling**:

   * `time.h` library to seed the random number generator with `time(NULL)`.

