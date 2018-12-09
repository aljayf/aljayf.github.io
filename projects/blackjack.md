---
layout: project
type : project
image: images/blackjack.jpg
title: Blackjack
permalink: projects/blackjack
date: 2017-02-19
labels:
  - Java
summary: A command line game of blackjack.
---
This program allows the user to blackjack against a CPU. Prior to a game of blackjack, the user is prompted if he/she wants to play a game of blackjack. If the user types "No" the program is terminated. If the user types "Yes" a game of blackjack begins. Any other input provided by the user, the user is prompted to try again. Once a game of blackjack begins, two cards goes to the user then two to the dealer. If the dealer has "21", the user automatically loses. Else, the user has the option to hit or stand and play a regular game of blackjack.

In result of this project, I gained a better understanding of Object-Oriented Programming. This project played a fundamental role in my understanding of how to structure a project. I learned how to use multiple classes to build one big project and how to build off of other classes.

In this project, It consisted of 3 classes. The core of the project was the card class. Then, I created a deck class which was constructed of 52 card objects. Finally, I was able to create the game class to construct how to implement the deck class to play a game of blackjack.

<h3>Code</h3>
<h4>Card Class</h4>
```
  public String name, suit;
	public int rank, value;

	public Card(String suit1,int rank1) {
		String [] names = {"ace","2","3","4","5","6","7","8","9",
				"10","jack","queen","king"};
		suit = suit1;
		rank = rank1;
    ...
```
