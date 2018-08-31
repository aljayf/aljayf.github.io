---
layout: project
type: project
image: images/Hexadoku.jpg
title: Hexadecimal Sudoku
permalink: projects/sudoku
date: 2017-10-27
labels:
  - Java
summary: Program to solve given hexadecimal sudoku problems.
---

In this project, I created code to solve to solve a 16x16 sudoku problem. In order to do this I implemented three functions; legalValues, checkSudoku, and solveSudoku. The function legalValues looked at the sudoku and found all the possible values that could fill in the spot. The function checkSudoku check if the number at a spot is valid. Finally, solveSudoku uses both legalValues and checkSudoku to solve the entire hexadecimal sudoku by call those functions at every spot in the sudoku determining the solution.
This program was created for an ICS 211 assignment. Correctness has been proven by JUnit tests created by my professor Charleton Moore. The JUnit test consisted of mulitple predetermined hexadecimal sudoku problems, along with their solutions, each at different levels of difficulty.

