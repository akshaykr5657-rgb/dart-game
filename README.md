# HTML-Only Arcade Game

A simple, multi-page "click the target" arcade game created using only HTML. This project serves as a basic demonstration of how to create a sequence of interactive pages without using any JavaScript or external CSS.

## Description

The game consists of a series of levels where the player must click on a target emoji (🎯). Each successful click loads a new HTML page, which represents the next level. The target appears in a different, pre-defined location on each level, and the score is updated as simple text on the page.

This project highlights the limitations of HTML as a standalone technology for game development while showing a creative, albeit rudimentary, way to simulate game-like progression.

## How to Play

To run this game, you do not need a web server. You can play it directly from your local files.

1.  **Create a Folder:** Make a new folder on your computer to hold the game files.
2.  **Create the Files:** Inside the new folder, create four empty files with the following exact names:
    * `game.html`
    * `level2.html`
    * `level3.html`
    * `win.html`
3.  **Copy the Code:** Copy the HTML code provided for each file into its corresponding file.
4.  **Start the Game:** Open the `game.html` file in any modern web browser (like Chrome, Firefox, or Edge).
5.  **Click the Target:** Click the 🎯 emoji to advance through the levels until you reach the "You Win!" screen.

## How It Works

The entire "game logic" is based on simple HTML hyperlinks (`<a>` tags).

* **Levels as Pages:** Each level is a separate `.html` file.
* **Actions as Links:** The target on each page is a hyperlink that points to the next level's HTML file.
* **State Management:** Game state, such as the score and the target's position, is not calculated dynamically. Instead, it is hardcoded into the content and inline styles of each individual page. For example, `level2.html` explicitly states "Score: 1", and its target is positioned at a new fixed location.

## Limitations

Since this project uses **only HTML**, it has several inherent limitations:
* **No Randomness:** The target's position is fixed for each level and cannot be randomized.
* **No Dynamic Score:** The score is just text and is not tracked or calculated.
* **No Timers:** There is no way to implement a timer or a time limit.
* **Fixed Levels:** The number of levels is predetermined by the number of HTML files created.

This project is a fun exploration of what's possible within strict constraints. For true game development with dynamic elements, JavaScript is essential.