# How to play

## Rules (spades variant)
Draw a diagram of the system that you threat model / risk analyze before dealing cards. Play like “Spades”, where everyone must play in the same suit if they can (just play a different suit if you don't have cards from the suit in play), and the highest “bidder” takes the trick and may start the next round. In Elevation of MLsec, cards in the Dataset risk suit are trump. Use a diagram / model of an ML system, ML lifecycle or a system with an ML component. The player should be able to explain how the risk relates to the model. In case of an argument, when something is not clear from the diagram, the player may make the necessary assumptions about the system to call a risk, or the team may agree upon a playbook for their system.

The ace of each suit is an open risk card. When a ace is played, the player must identify a risk not listed on another card. To help with this, see the summary cards in the back of the deck.

**Points:** 1 for a threat on your card, +1 for taking the trick.

When all the cards have been played, whoever has the most points wins. Don’t forget to triage the threats you discovered, and lastly remember to have fun.

## Setup cheatsheet
(Taken from https://github.com/adamshostack/eop/blob/master/cheatsheet.md) 

1. Draw a system model where everyone can see it, for example on a whiteboard or on a large screen.
2. Ask everyone to set aside skepticism for 15 minutes.
3. Setup details
    - Goal: Win hands by connecting the threat on the card to the system and playing the highest card of the current suit.
    - Play in small groups (3-6 people), using one deck per group.  Remove the front cards (instructions, strategy) and the back (lists of threats), so you only have threat cards, and shuffle those. Deal the whole deck to the players.
    - Give the players a few minutes to study their hand and the system at hand before you begin
    - Determine the first player based on who has the lowest card of Input risks.
4. Play!
    - Make sure people take notes on the threats
    - Some people will play collaboratively with their hands face up in front of them, others competitively, with cards close to their chest. Choose the approach that you wish.

# Variants

We recommend that you play with the game and adjust it so it suits better for your team. Here are a couple of variants.

## Speed variant

The process of laying down and explaining risks for every player is somewhat time consuming. A speed variant plays the same way, but only the person who won the trick explains how their card relates to the system. An extra point is still awarded if the player can explain how the threat relates to the system.
**Points:** 1 for a threat on your card, +1 for taking the trick.


## Non-spades variant

### Playing the game
This game variant simply sinks through the deck and doesn't have any rules to award points outside of being able to explain how threats relate to the system.

The player who gets to start the game will draw the top card of the deck and place it face up next to the system model.
They then have to identity a vulnerability in the system model corresponding to the drawn threat.
If they are unable to do so, the player clockwise of them gets to attempt to identify a vulnerability.
This process continues until either a player successfully identifies a vulnerability matching the card or all players have failed to do so.

If a player successfully identifies a vulnerability, they should write down the vulnerability they identified and place the threat card in front of themselves.
The game then continues with the player clockwise of them drawing a new card from the deck.

If no player manages to identify a vulnerability for a card, then the card is removed from play and the player who originally drew it from the deck gets to draw a new card.

**Points:** 1 for a threat on your card


### Ending the game
The game ends when the deck is empty. The winner of the game is the player who identified the most vulnerabilities, i.e. the player who has the most cards placed in front of themselves.
