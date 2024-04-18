# Question 1
```JS
  makeBoard() {
    this.board = []; // array of rows, each row is array of cells  (board[y][x])
    // Create row, where `HEIGHT` is the height of the game board.
    for (let y = 0; y < this.HEIGHT; y++) {
      this.board.push(Array.from({ length: this.WIDTH }));
    }
  }
```
1.  `{ length: this.WIDTH }`: This creates an object with a property named length set to the value of `this.WIDTH`. For this specific case, the key-value pair is `length: 6`
2. ` Array.from({ length: this.WIDTH })`: This takes the object created in step 1 and creates a new array with a length equal to `this.WIDTH`. The array is initially empty, meaning it contains undefined values for each element.
    -   How did this create a new arry with a length equal to `this.WIDTH`?
        -   from my understanding, `{ length: this.WIDTH }` is an object with ONE property. This confuse me.

# Things to clarify 
```JS
handleClick(evt) {

    // More code

    // place piece in board and add to HTML table
    this.board[y][x] = this.currPlayer;
    this.placeInTable(y, x);

    // More code
  }
```

- Is `this.board[y][x]` accessing `board` variable in the `makeHtmlBoard` method? 


