<h1 align="center">TIC-TAC-TOE</h1>

<p align="center">
  <img src="https://github.com/BhavdeepSinghNijhawan/Tic-Tac-Toe/assets/143419096/1d506056-9ac3-455d-9c61-418c5f19a2a7" />
</p>

## LIVE URL

https://bhavdeepsinghnijhawan.github.io/Tic-Tac-Toe/

## TECHNICAL STACKS

Tic-Tac-Toe, also known as noughts and crosses or Xs and Os, is a classic paper-and-pencil game typically played on a 3x3 grid. Two players take turns marking spaces in the grid with their respective symbols, usually "X" for one player and "O" for the other, until one player achieves a line of three of their symbols either horizontally, vertically, or diagonally. The objective of the game is to be the first player to create a line of three of their symbols and prevent the opponent from doing so. If the grid is filled without any player achieving a winning line, the game ends in a draw. Tic-tac-toe is simple, easy to learn, and often played as a recreational game by children and adults alike.

## TECHNOLOGY STACK

### HTML

```
<!DOCTYPE html>
<html lang="en">
```

- **`<!DOCTYPE html>:`** This declares the document to be an HTML5 document.
- **`<html lang="en">:`** This tag opens the HTML document and sets the language to English.

```
<head>
  <meta charset="UTF-8" />
  <meta http-equiv="X-UA-Compatible" content="IE=edge" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Tic Tac Toe</title>
  <link rel="stylesheet" href="style.css" />
</head>
```
- **`<head>:`** This section contains meta-information about the document.
- **`<meta charset="UTF-8" />:`** This sets the character encoding to UTF-8.
- **`<meta http-equiv="X-UA-Compatible" content="IE=edge" />:`** This ensures the document is compatible with Internet Explorer.
- **`<meta name="viewport" content="width=device-width, initial-scale=1.0" />:`** This sets the viewport to make the website responsive on all devices.
- **`<title>Tic Tac Toe</title>:`** This sets the title of the document that appears in the browser tab.
- **`<link rel="stylesheet" href="style.css" />:`** This links the HTML document to an external CSS file for styling.

```
<body>
  <nav>
    <ul>
      <li>Bhavdeep Singh Nijhawan</li>
    </ul>
  </nav>
```

- **`<body>:`** This section contains the content of the HTML document.
- **`<nav>:`** This defines a navigation section.
- **`<ul>:`** This defines an unordered list.
- **`<li>Bhavdeep Singh Nijhawan</li>:`** This defines a list item with the name "Bhavdeep Singh Nijhawan".

```
<div class="gameContainer">
    <div class="container">
      <div class="line"></div>
```

- **`<div class="gameContainer">:`** This defines a container for the game, with the class gameContainer.
- **`<div class="container">:`** This defines another container inside the game container, with the class container.
- **`<div class="line"></div>:`** This defines a line element, presumably for visual styling in the game.

```
  <div class="box bt-0 bl-0"><span class="boxtext"></span></div>
  <div class="box bt-0"><span class="boxtext"></span></div>
  <div class="box bt-0 br-0"><span class="boxtext"></span></div>
  <div class="box bl-0"><span class="boxtext"></span></div>
  <div class="box"><span class="boxtext"></span></div>
  <div class="box br-0"><span class="boxtext"></span></div>
  <div class="box bl-0 bb-0"><span class="boxtext"></span></div>
  <div class="box bb-0"><span class="boxtext"></span></div>
  <div class="box bb-0 br-0"><span class="boxtext"></span></div>
</div>
```

- These lines define the individual boxes of the Tic Tac Toe grid. Each box has the class box and may have additional classes like bt-0, bl-0, br-0, bb-0 for styling purposes (likely to remove borders on specific sides).
- **`<span class="boxtext"></span>:`** This span is inside each box and will likely be used to display the X or O text.

```
      <div class="gameInfo">
        <h1>TIC TAC TOE</h1>
        <div>
          <span class="info">Starting With X: All the Best</span>
          <button id="reset">RESET</button>
        </div>
        <div class="imgbox">
        </div>
      </div>
    </div>
    <script src="script.js"></script>
  </body>
</html>
```

- **`<div class="gameInfo">:`** This section provides information about the game.
- **`<h1>TIC TAC TOE</h1>:`** This displays the main heading of the game.
- **`<span class="info">Starting With X: All the Best</span>:`** This displays some initial game information.
- **`<button id="reset">RESET</button>:`** This button is used to reset the game.
- **`<div class="imgbox">:`** This div is likely for displaying images, though it's empty in the provided code.
- **`<script src="script.js"></script>:`** This includes an external JavaScript file, which will contain the game's logic and functionality.

### CSS

### JavaScript

# CONTRIBUTOR

- [Bhavdeep Singh Nijhawan](https://www.linkedin.com/in/bhavdeep-singh-nijhawan-739634280)
