# Styling Rock, Paper, Scissors
## This is a practice project from the codecademy front end platform. Much of this code was already set up for me.
>In this project, you will get the chance to practice styling React applications using different techniques.

>You will be styling a game of Rock, Paper, Scissors. However, rather than sticking to one technique, you will be asked to modify its appearance using inline styling syntax, object variable syntax, and, finally, CSS modules!

>Throughout the project, you’ll be able to explore the advantages and disadvantages of each approach and practice React naming conventions for style properties.

>By the end of this practice project, you will have improved your skills in styling React applications using various techniques and gained a deeper understanding of the different approaches. You will be able to apply your learnings to future React projects and improve your coding skills!

## I took the following steps to practice styling in React:
### Inline Styling
1.  Take a look at Game.js. The game is already functional, but it needs some styling.

    Start by practicing your understanding of inline styling.

    Find the <h1> element responsible for the game’s title, “Rock Paper Scissors”.

    Apply an inline style to change the font size property to 48, and set the margin top property to 0.

    Object Variable Styling
2.  Next, let’s define a few object variables to use for styling.
    Above the Game component, create an object variable named choiceStyles. The object should contain the following properties:
        Display with the value of flex.
        Align items with the value of center.
        Margin bottom with a value of 40 pixels.

3.  Under the choiceStyles, define another object variable named emojiStyles with the following properties:
        Font size with the value 64 pixels.
        Margin right with the value of 20 pixels.

4.  Under the emojiStyles, define another object variable named nameStyles with the following properties:
        Margin of 0 pixels.
        Font size of 24 pixels.
        Color with the value of #ffff.
5.  Last, under the nameStyles, define another object variable named resultStyle with the following properties:
        Margin top of 40 pixels.
        Font size of 48 pixels.
        Color with the value of #ffff.
6. Great job! Our object variable styles are now defined. It’s time to apply it.
        Apply the styles in choiceStyles to the <div> surrounding:

        <span>{playerChoice.emoji}</span>
        <p>You chose {playerChoice.name}</p>

        and the <div> container surrounding:

        <span>{codeyChoice.emoji}</span>
        <p>The computer chose {codeyChoice.name}</p>

7.  Apply the styles in emojiStyles to:

    <span>{playerChoice.emoji}</span>

    as well as:

    <span>{codeyChoice.emoji}</span>

8.   Apply the styles in nameStyles to:

    <p>You chose {playerChoice.name}</p>

    as well as:

    <p>Codey chose {codeyChoice.name}</p>

9.  Last, apply resultStyle to:
        <h2>{result}</h2>

10. Click Save to run your code. Your page should render with some styles applied. It doesn’t look great yet, because we’re not done with the        
    styling—but if you see the text and emojis in a bigger size, you’re on the right track!

### CSS Module Styling
11. Let’s proceed to styling with CSS modules now.
    Open up Game.module.css. Take a look inside. There are already styles defined in there for you. All we have to do is apply it!
    Go back to Game.js and apply the styles for the .container selector to the very first <div> after in the return statement:
    return (
    <div>
        <h1 style={{ fontSize: 48, marginTop: 0 }}>Rock Paper Scissors</h1>
        ...
    </div>
    );
    Remember to import the CSS module into an object named styles!

12. Apply the styles for the .choices selector to the <div> containing the rock, paper, scissors buttons.
    You can find this <div> under the <h1> title and above the logic for mapping over the CHOICES object array.

13. Next, apply the .results selector to the <div> containing the game’s results.
    You can find this <div> between playerChoice && codeyChoice && ( and <div style={choiceStyles}>.

14. Lastly, apply the styles for the .button selector to the Play Again button and each choice button.

15. Press Save to run and see how the Rock Paper Scissors game has been fleshed out and styled in three different ways!