# Dice Game

<img width="1440" alt="Screenshot 2023-06-19 at 2 05 21 PM" src="https://github.com/0xJeu/Dice-Game/assets/129988927/fc28f7f8-0a13-4609-a3ac-2775d8743d1a">
This JavaScript code simulates a dice game between two players. The code generates random numbers to determine the outcome of the game and updates the HTML content accordingly.

## How It Works

1. The code generates a random number between 1 and 6 for the first player using the `Math.random()` function. The result is stored in the variable `randomNumber1`.

2. The code selects the first `<img>` element in the HTML using the `document.querySelectorAll("img")[0]` selector and stores it in the variable `img1`. It does the same for the second `<img>` element and stores it in the variable `img2`.

3. It creates a filename for the dice image by appending `randomNumber1` to the string "dice" and then appending ".png". The resulting filename will be "dice1.png" to "dice6.png" based on the value of `randomNumber1`. The filename is stored in the variable `randomDiceImage`.

4. It creates the complete image source path by appending "images/" to the `randomDiceImage`. The resulting path will be "images/dice1.png" to "images/dice6.png". The path is stored in the variable `randomImageSource`.

5. It sets the `src` attribute of `img1` to `randomImageSource` using the `setAttribute()` method. This updates the displayed image of the first player's dice.

6. The code generates a random number between 1 and 6 for the second player and stores it in the variable `randomNumber2`.

7. It creates the image source path for the second player's dice using the filename pattern "images/dice" + `randomNumber2` + ".png". The path is stored in the variable `randomImageSource2`.

8. It sets the `src` attribute of `img2` to `randomImageSource2`, updating the displayed image of the second player's dice.

9. It compares `randomNumber1` and `randomNumber2` to determine the winner of the game. If `randomNumber1` is greater than `randomNumber2`, it sets the text content of the first `<h1>` element to "Player 1 Wins!!". If `randomNumber2` is greater, it sets the text content to "Player 2 Wins!!". Otherwise, if both numbers are equal, it sets the text content to "DRAW".

## How to Use

To use this code, follow these steps:

1. Create an HTML file and link it with a JavaScript file.

2. Copy and paste the provided code into the JavaScript file.

3. Create the necessary HTML elements in the HTML file. You will need two `<img>` elements to display the dice images and one `<h1>` element to display the game result.

4. Create a folder named "images" and place the dice images (dice1.png to dice6.png) inside it.

5. Open the HTML file in a web browser.

6. Each time you refresh the page, the code will generate random numbers and update the dice images and game result accordingly.

## Example Output

Example output when the first player's random number is 4 and the second player's random number is 2:

```
Player 1 Wins!!
```

Example output when the first player's random number is 3 and the second player's random number is 5:

```
Player 2 Wins!!
```

Example output when the first player's random number is 2 and the second player's random number is 2:

```
DRAW
```

## Acknowledgments

This code is a simple implementation of a dice game using JavaScript. Feel free to modify and expand it according to your requirements.


