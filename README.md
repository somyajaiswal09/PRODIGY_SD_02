#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() {
    int randomNumber, userGuess, attempts = 0;

    // Initialize random number generator
    srand(time(0));

    // Generate random number between 1 and 100
    randomNumber = rand() % 100 + 1;

    printf("Welcome to the Number Guessing Game!\n");
    printf("I have picked a number between 1 and 100. Can you guess it?\n");

    // Loop until the user guesses the correct number
    do {
        // Prompt user for a guess
        printf("Enter your guess: ");
        scanf("%d", &userGuess);

        // Increment the attempt counter
        attempts++;

        // Compare guess to random number and give feedback
        if (userGuess < randomNumber) {
            printf("Your guess is too low. Try again!\n");
        } else if (userGuess > randomNumber) {
            printf("Your guess is too high. Try again!\n");
        } else {
            printf("Congratulations! You've guessed the number correctly.\n");
            printf("It took you %d attempts.\n", attempts);
        }
    } while (userGuess != randomNumber);

    return 0;
}
