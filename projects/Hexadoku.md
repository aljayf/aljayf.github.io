---
layout: project
type: project
image: images/Hexadoku.jpg
title: Hexadecimal Sudoku
permalink: projects/sudoku
date: 2017-10-27
labels:
  - Java
  - Recursion
summary: Program to solve given hexadecimal sudoku problems.
---

In this project, I created code to solve to solve a 16x16 Sudoku problem. To do this, I implemented three functions; legalValues, checkSudoku, and solveSudoku. The function legalValues looked at the Sudoku and found all the possible values that could fill in the spot. The function checkSudoku check if the number at a spot is valid. Finally, solveSudoku uses both legalValues and checkSudoku to solve the entire hexadecimal sudoku by call those functions at every spot in the sudoku determining the solution.

This program was created for an ICS 211 assignment. Correctness has been proven by JUnit tests created by my professor Charleton Moore. The JUnit test consisted of multiple predetermined hexadecimal Sudoku problems, along with their solutions, each at different levels of difficulty.

This project thought me one of the central ideas of problem solving in computer science. Using **recursion** played a major role in this project as it allowed me to use smaller instances of the bigger problem to solve the same problem.

<h2>Code</h2>
Below is a snip of how I implemented recursion to solve the big problem:

```
private static boolean solveSudoku(int[][] sudoku, int row, int column) {
    
    if (row == 16) {
      return checkSudoku(sudoku, false);
    }
    int nextRow = row;
    int nextColumn = column + 1;
    if (nextColumn == 16) {
      nextColumn = 0;
      nextRow++;
    }

    if (sudoku[row][column] != -1) {
      if (solveSudoku(sudoku,nextRow,nextColumn)) {
        return checkSudoku(sudoku,false);
      }
    } else {
      ...
```
