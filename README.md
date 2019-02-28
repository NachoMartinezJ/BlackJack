# BlackJack

## Rules of the game

#### Objective
------------
The objective of the game is beating the dealer. We can do so in 3 ways: 
 - Getting 21 points.
 - Getting as close as 21 points as we can, while the dealer scores less points than us.
 - The dealer goes over 21 points, **this is called "bust"**
 
#### Card values
--------------
- **Ace** -> 1 or 11.
- **K, Q, J** --> 10.
- **Other cards** --> The value they show in the card.

#### Betting
-------------
Before dealing the cards, players bet an amount 2$ >= 500$.

#### Dealing
--------------
**After betting**, the dealer gives the player and himself one card **face up**. Afterwards, another round of cards is dealt, **face up** for the player and **face down (called hole card)** for the dealer.

#### Naturals
---------------
If a player **receives an ace(11) and a 10** on the first hand, it is considered a **natural blackjack**.

If the dealer doesn't have a natural blackjack himself, **he automatically loses** and must pay the player **x1.5 times the original bet**. However if the dealer also has a natural blackjack it is considered a **tie**, and the **player recovers his original bet**.

If the dealer face up card is a 10 or an ace(11), he may look at the face down card to check if he has a natural blackjack. If this is the case, **he automatically wins** (if none of the previous cases apply).

#### The play
-----------------
The player has two options:

- **Hit** --> The player asks for an additional card. **Its value will be added** to the previous two cards.
- **Stand** --> The player doesn't ask for another card. He plays with the **sum of the two initial cards**.


#### Splitting pairs
----------------------
If a player's **first 2 cards are of the same denomination**, he may choose to **play them as separate hands**. He must bet the same amount in the second hand.

He plays first the left hand, and when he's done, he plays the right hand.

If he's dealt a pair of aces, the player is given one card per ace and may not draw more. Also, **if he hits a blackjack**, he'll receive the **amount of the bet and not x1.5 times more**.

#### Doubling down
--------------------
If a player's **first 2 cards sum 9, 10 or 11** he may choose to double his bet. If he does so, he will receive **only one extra card face down**.

#### Settlement
------------------
- If the **player goes bust**, he has already lost its wager.
- If **dealer goes bust**, he pays the player.
- If **dealer doesn't have 21 points**, pays the player with higher standoff.
- If **dealer has the same amount of points as the player**, nothing happens. Player takes back his bet.

## Features
--------------
- Dealer --> Pc.
- Player --> Human giving input on what to do, how much to bet.
- Deck --> Collection of 52 numbers, mimicking the cards found in a deck.
- The play --> Random number of the collection of 52 numbers.


## Workflow
-----------
1. Ask player how much he wants bet.
2. Cards are dealt: both face up for the player, one of them facing down for the dealer.
3. Check if the player has a natural blackjack.
4. Check if the dealer has a natural blackjack.
5. Check if the player has cards of the same denomination. If it's the case, ask him if he wants to split.
6. Check if the player's cards add up to 9, 10 or 11. If they do, ask the player if he wants to double down.
7. Ask the player if he wants to stand or hit.
8. Check if player has doubled down. If he has and chooses to hit, after dealing him the card, the dealer plays his hand.
9. If the player hits, check score.
10. If the sum of the cards adds up to more than 21 points, the player losses.
11. If the summ of cards is not equal or more than 21 points, player can choose to hit again.
12. In case he lost, we ask the player if he wants to play again, and repeat the process.
 



