# 🃏 Two Classic Card Games in Python

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)

A pair of text-based card games built with **object-oriented Python** and played right inside Jupyter Notebook. No GUI, no dependencies, just clean classes, a well-shuffled deck, and a little bit of luck.

---

## 🎴 Blackjack

> *Get as close to 21 as you can without going over.*

You start with **100 chips**, place your bet, and go head-to-head with a dealer who hits until reaching **17**. Aces flex between **1 and 11**, so every hand keeps you guessing.

**Highlights**
- Clean `Card`, `Deck`, `Hand`, and `Chips` classes
- Proper Ace handling so hands never overshoot silently
- Dealer shows one card, keeping the other hidden
- Win, lose, push, and bust logic with chips tracked every round

**Sample run:** a 60-chip bet goes to the dealer, then a 50-chip bust leaves the player at 50 chips before cashing out.


---

## ⚔️ War

> *Highest card wins — unless it's a tie, and then it's all out WAR.*

The deck is shuffled and split **26 / 26**. Each round both players flip a card and the higher card takes both. On a tie, **WAR** is declared: each player must still hold at least **5 cards**, commits them, and the battle repeats until one side folds.

The match runs until a player is out of cards — or can't afford the cost of war.
In the recorded run it lasted **92 rounds** before Player Two took the win.

**Highlights**
- `Card`, `Deck`, and `Player` classes with `remove_one()` and `add_cards()`
- Even dealing from a shuffled 52-card deck
- War resolution that chains ties into one continuous battle loop
- Round-by-round output, including every `WAR!` moment

---

## 🚀 Getting Started

1. Clone the repository or download both notebooks.
2. Open them with Jupyter Notebook, JupyterLab, or VS Code.
3. Run all cells from top to bottom.

## 🧠 What These Projects Practice

Both notebooks are exercises in **object-oriented design**: modeling real objects (cards, decks, hands, players) as classes, sharing state between them, and keeping game rules in readable methods. Small enough to read in one sitting, structured enough to extend with new games.

## 📜 License

Released under the **MIT License** — free to use, learn from, and modify.
