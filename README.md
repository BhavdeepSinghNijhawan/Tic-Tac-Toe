<h1 align="center">TIC-TAC-TOE</h1>

<p align="center">
  <img src="https://github.com/BhavdeepSinghNijhawan/Tic-Tac-Toe/assets/143419096/1d506056-9ac3-455d-9c61-418c5f19a2a7" />
</p>

## LIVE URL

https://bhavdeepsinghnijhawan.github.io/Tic-Tac-Toe/

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

```
@import url('https://fonts.googleapis.com/css2?family=Baloo+Bhaina+2&family=Roboto&display=swap');
```

- @import url('https://fonts.googleapis.com/css2?family=Baloo+Bhaina+2&family=Roboto&display=swap');

```
*{
    margin: 0;
    padding: 0;
}
```

- This resets the margin and padding for all elements to 0 to ensure consistent styling across browsers.

```
nav{
    background-color: rgb(255, 115, 0);
    color: white;
    height: 65px;
    font-size: 27px;
    display: flex;
    align-items: center;
    padding: 0 12px;
    font-family: 'Roboto', sans-serif;
}
```

- Styles for the **`<nav>`** element: sets background color, text color, height, font size, and padding. Uses Flexbox for alignment and applies the "Roboto" font.

```
nav ul{
    list-style-type: none;
}
```

- Removes the default bullet points from the list inside the **`<nav>`**.

```
.gameContainer{ 
    display: flex;
    justify-content: center;
    margin-top: 50px;
}
```

- Centers the game container horizontally and adds a top margin.

```
.container{
    display: grid;
    grid-template-rows: repeat(3, 10vw);
    grid-template-columns: repeat(3, 10vw);
    font-family: 'Roboto', sans-serif;
    position: relative;
}
```

- Defines a grid layout with 3 rows and 3 columns, each sized at 10 viewport width (vw). Applies the "Roboto" font and positions the grid relatively.

```
.box{
    border: 2px solid black;
    font-size: 8vw;
    cursor: pointer;
    display: flex;
    justify-content: center;
    align-items: center;
}
```

- Adds a 2px black border to each box, sets the font size to 8vw, changes the cursor to a pointer on hover, and centers the content using Flexbox.

```
.box:hover{
    background-color: rgb(255, 115, 0);
}
```

- Changes the background color of a box when hovered.

```
.info {
    font-size: 22px;
}
```

- Sets the font size for elements with the class **`info`**.

```
.gameInfo{
    padding: 0 34px;
    font-family: 'Baloo Bhaina 2', cursive;
}
```

- Adds padding and applies the "Baloo Bhaina 2" font.

```
.gameInfo h1{
    font-size: 2.5rem;
}
```

- Sets the font size for **`h1`** elements inside **`gameInfo`**.

```
.imgbox img{
    width: 0;
    transition: width 1s ease-in-out;
}
```

- Initially sets the width of images inside **`imgbox`** to 0 and animates the width change over 1 second.

```
.br-0{
    border-right: 0;
}
.bl-0{
    border-left: 0;
}
.bt-0{
    border-top: 0;
}
.bb-0{
    border-bottom: 0;
}
```

- These classes remove specific borders from elements, useful for creating the Tic Tac Toe grid layout without double borders.

```
#reset {
    margin: 0 23px;
    padding: 1px 18px;
    background: rgb(255, 115, 0);
    border-radius: 6px;
    cursor: pointer;
    font-family: 'Baloo Bhaina 2';
    font-size: 15px;
    font-weight: bolder;
}
```

- Styles the reset button with margin, padding, background color, rounded corners, and applies the "Baloo Bhaina 2" font.

```
.line{
    background-color: black;
    height: 3px;
    width: 0;
    position: absolute;
    background-color: #911d91;
    transition: width 1s ease-in-out;
}
```

- Defines a line with initial width 0 and animates the width change over 1 second. The background color is set twice, with the second color being **`#911d91`**.

```
@media screen and (max-width: 950px)
{
    .gameContainer{
        flex-wrap: wrap;
    }
    .gameInfo{
        margin-top: 34px;
    }
    .gameInfo h1{
        font-size: 1.5rem;
    }
    .container { 
        grid-template-rows: repeat(3, 20vw);
        grid-template-columns: repeat(3, 20vw);
    }
}
```

- Adjusts the layout for screens smaller than 950px:
  - Wraps the game container.
  - Adds top margin to **`gameInfo`**.
  - Decreases the font size of **`h1`** elements in **`gameInfo`**.
  - Doubles the size of grid rows and columns to 20vw.
  
### JavaScript

## CONTRIBUTOR

- [Bhavdeep Singh Nijhawan](https://www.linkedin.com/in/bhavdeep-singh-nijhawan-739634280)
