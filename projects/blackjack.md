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

This consisted of 3 classes. The core of the project was the card class. Then, I created a deck class which was constructed of 52 card objects. Finally, I was able to create the game class to construct how to implement the deck class to play a game of blackjack.

<h2>Code</h2>
Here is a brief overview on how I structured the project:
<h3>Card Class</h3>
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
<h3>Deck Class</h3>
```
Card [] deck;
int size;

public Deck() {
	deck = new Card[52];
	int position = 0;
	for(int i = 1; i < 14; i++) {
		Card c1 = new Card("hearts", i);
		Card c2 = new Card("diamonds", i);
		Card c3 = new Card("spades", i);
		Card c4 = new Card("clubs", i);
		...
```
<h3>Game Class</h3>
```
Deck myDeck;
int playerScore;
int dealerScore;
String winner;

ArrayList <Card> playerHand;  // To store player's cards
ArrayList <Card> dealerHand;  // to store dealer's cards

public Game() {
	myDeck = new Deck();  //Create a new deck
	myDeck.shuffle(); //Shuffle the deck
	...
```

