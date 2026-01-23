---
layout: project
type: project
image: img/cards.png
title: "Blackjack"
date: 2025
published: true
labels:
  - Python
  - GitHub
summary: "A soon to be blackjack dealer discord bot."
---

<img class="img-fluid" src="../img/blackjack.png">
 
If you have not heard of blackjack here's a simple rundown. First, there are two roles: the player(s) and the dealer. There are separate rules for each role that we will be getting into later. Then, you, and other players if applicable, are assigned two cards faced up, meaning everyone can see your hand. The dealer is also assigned two cards, but players can only see one. The number cards follow the values displayed. In the cases of the jack, queen, and king, they all represent 10s while the ace represents either 1 or 11 (it's your choice!). After you are given these cards, you add them up and see if they are equal to or less than 21. If they add up to 21, great job, you win (well in the worst case tie)! But if they don't, you are asked to hit(get a card) or stand(no card). If you decide to hit and your values add up to over 21, then you bust, meaning you lose. The dealer plays his turn last.

Currently you can only play this game via the terminal, but I do plan on making a discord bot. I also aspire to add a betting function with a server-wide currency system. I think it will be fun playing around and seeing how my friends would go crazy, even though it's non-existent money. With all these aspirations, I know there's more challenges to come, but I'm excited to learn more.

Here's what a run of the code looks like for now:

<hr>

<pre>
Player's Hand: [('6', 'Diamonds'), ('9', 'Spades')] Total: 15
Dealer's Shows: ('3', 'Diamonds')
Hit or Stand? (h/s): h
Player's Hand:  [('6', 'Diamonds'), ('9', 'Spades'), ('King', 'Clubs')] Total:  25
You busted! GG, Dealer wins!
Play again? (y/n): 
</pre>

<hr>

Source: <a href="https://github.com/jogarces/ics-313-text-game"><i class="large github icon "></i>jogarces/ics-313-text-game</a>
