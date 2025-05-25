 ```mermaid flowchart TD Start([Start the Game]) --> Step1[Generate a number between 1 and 10] Step1 --> Step2[Say "Guess a number between 1 and 10!"] Step2 --> Step3{Is the input a number?} Step3 -- No --> Error[Say "You must choose a number"] --> Step2 Step3 -- Yes --> Step4{Is the guess correct?} Step4 -- Yes --> Win[Say "That is correct!"] --> End([End]) Step4 -- No --> Step5{Too high or too low?} Step5 -- Too high --> TipHigh[Say "Oops too high!"] --> Step2 Step5 -- Too low --> TipLow[Say "Uh-oh too low!"] --> Step2```
1. The game starts and generates a random number between 1 and 10.
2. The user is asked to guess a number between 1 and 10.
3. If the user enters a non-numeric value, the game shows an error and asks again.
4. If the input is valid, the game checks if the guess is correct:
   - If correct: it displays “That is correct!” and the user wins, the game ends.
   - If incorrect: it checks if the guess is too high or too low.
5. Based on the guess, the game gives a hint and asks for another guess.
6. The process repeats until the user guesses the correct number.
