# ♠️ Week08 Bootcamp2019a Project: Matching Card Game

### Goal: Make a 10 card memory game - users must be able to select two cards and check if they are a match. If they are a match, they stay flipped. If not, they flip back over. Game is done when all cards are matched and flipped over. Example: http://www.fruit-burst.co.uk/fun-and-games/pairs-game 

### How to submit your code for review:

- Fork and clone this repo
- Create a new branch called answer
- Checkout answer branch
- Push to your fork
- Issue a pull request
- Your pull request description should contain the following:
  - (1 to 5 no 3) I completed the challenge
  - (1 to 5 no 3) I feel good about my code
  - Anything specific on which you want feedback!

Example:
```
I completed the challenge: 5
I feel good about my code: 4
I'm not sure if my constructors are setup cleanly...
```

Dragon Ball Z Memory Match 

Flip the cards and find the pairs. There are 5 Dragon Ball Z cards, each one shows up twice, and they get shuffled every game. Match all 5 pairs, and you're a Winnnnnnnaaaaaa.

How to Play
- Click a card to flip it over
- Click a second card and try to find its match
- If they match, they stay face up
- If they don't, they flip back over after a second, and it counts as a miss
- Match all 5 pairs to win
- Hit the redo button to shuffle and play again

The scoreboard tracks your wins and misses across games.

How It Works

Shuffling the deck: dealCards() doubles the card list with the spread operator ([...cards, ...cards]) so every picture has a pair. Then for each card spot on the board, it picks a random card out of the deck with splice(). Since splice() removes the card it picks, nothing gets dealt twice.

Flipping cards: turnOver() handles every click. The first card you pick gets saved in firstCard. When you pick a second one, it compares the two image sources. Same picture = match. Different picture = both flip back over.

No cheating allowed: while two unmatched cards are showing, the waiting flag blocks any other clicks until they flip back. You also can't click a card that's already face up.

Winning: every match adds to the match count. When matches equals the number of different cards (5), you win, and your win count goes up.

Built With
- Vanilla JavaScript
- HTML
- CSS  

<img width="2879" height="1570" alt="image" src="https://github.com/user-attachments/assets/86ce2649-a984-4339-b04f-b22ff456adde" />

