Project Name:
Implement the package guessing game using java with GUI.
Introduction:
The number guessing game is based on a concept where the player guesses a number in ranges from one to ten. If the player guesses the exact number then the player wins else the player loses the game. Since this game provides limited attempts, so, the player must guess the number with the limited attempts.
Description:
1.The system generates a random number from a given range between 1 to 100.
2.The user must enter the number in the displayed dialogue box.
3.If the guessed number is bigger than the actual number, the program will respond with the message that the guessed number is higher than the actual number.
4.If the guessed number is smaller than the actual number, the program will respond with the message that the guessed number is lower than the actual number.
5.If the guessed number is equal to the actual number or if the K trials are exhausted, the program will end with a suitable message.
Approach:
Below are the steps:  
 1.The approach is to generate a random number using the Math.random() method in Java.
2.Now using a loop, take K input from the user, and for each input print whether the number is smaller or larger than the actual number.
3.If within K trials the user guessed the number correctly, print that the user won.
4.Else print that he was not able to guess and then print the actual number.
Rules and Regulation:
1.Limiting the number of attempts.
2.You will be provided limited attempts to guess the number.
3.You must enter only valid integers within the specified range.
4.You cannot leave the game, once started.
Randoms in Java:
Math.random() returns a value ∈[0,1[∈[0,1[, so if you want an integer between min and max, inclusive, you'll need to change a bit:
rand = (int) (Math.random() _ (max - min + 1)) + min;
...which, for 1..100 would make:
rand = (int) (Math.random() _ 100) + 1;
Because I got 0 on my first run of your game. :p
