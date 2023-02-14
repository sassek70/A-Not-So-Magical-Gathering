# A-Not-So-Magical-Gathering

A Not So Magical Gathering is my capstone project at Flatiron School and was developed using React.js and Ruby on Rails. This application is Player vs. Player card game that uses Ruby-on-Rails Action Cable and React.js websockets to connect two players in a game session.

##GETTING STARTED:

There are two ways to start a game. You can either Host a game or join a game if you have been sent a Game Key. If you choose to host a game, a game key will be displayed when the game loads. Send this key to the person you wish to play against.

##HOW TO PLAY:

When you host or join a game, you will be given a deck containing thirty (30) random cards, five (5) cards will displayed on your table at a time. Both players start with twenty (20) health. The Host player always has the first turn. On your turn, you can select a Card to attack or skip your turn. Once you click "Confirm Attack", your Opponent then gets to choose a Card to defend with. If the Defending Player chooses a card to defend with, the Power value of each card is compared against the Toughness value. Both player's card tables and total health will be updated based on the results

##EXAMPLE TURN

1. Player 1 (Host) attacks with a Power: 3, Toughness: 3 Card.
2. Player 2 defends with a Power: 1, Toughness: 2 Card.
3. The Power of the Attacking Card is greater than the Toughness of the Defending Card.
4. The Defending Card is destroyed and removed from the table and replaced with a new card from the Defending Player's deck.
5. Defending Card only blocked 2 damage and the Attacking Card has a Power of 3, 1 damage point remains and is applied to the Defending Player's health
6. The Defending Player's health is updated to 19
7. Since the Attacking Card's Toughness is greater than the Defending Cards Power, it remains on the table. It is now Player 2's turn

END OF GAME
The two (2) main ways for the game to end is when either player has 0 or less health remaining or if neither player has any cards available. In the first case, the player that has more than 0 health is declared the winner. In the second case, the game is considered a draw.

***IMPORTANT***
It is currently impossible to rejoin a game. If you refresh the page, navigate to a different page, close the browser tab, close the browser window or lose connection, you will be locked out of the game.



A Not So Magical Gathering is unofficial Fan Content permitted under the Fan Content Policy. Not approved/endorsed by Wizards. Portions of the materials used are property of Wizards of the Coast. ©Wizards of the Coast LLC.
A Not So Magical Gathering is a simplified battle-card game based on [Wizards of the Coast's](https://company.wizards.com/en) trading-card game [Magic: The Gathering](https://magic.wizards.com/en) and was created as a cap-stone project for [Flatiron School's Software Engineering](https://flatironschool.com/courses/coding-bootcamp/) course.
Card images and Artist information provided by the [Scryfall API](https://scryfall.com/docs/api/cards).

[A Not So Magical Gathering live site](https://a-not-so-magical-gathering.onrender.com/) - NOTE: After a period of inactivity, the hosting service will take the back-end server offline to conserve resources. It may take up to a minute to be brought online. You should see a list of users in the "Leaderboard" section when ther server is active.<br>
[Front-end Repo](https://github.com/sassek70/phase-5-frontend)<br>
[Back-end Repo](https://github.com/sassek70/phase-5-backend)
