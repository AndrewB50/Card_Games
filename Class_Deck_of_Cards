# This will be to create a deck of cards as an object. I think. Maybe it will turn into somehting else, but regardless that's the current intention...

# imported methods
import random
import math

# list of suits...
suits = ["Clubs", "Diamonds", "Hearts", "Spades"]

# initialize cards dealt...
dealtCards = []

# Playing card class...
class Playing_Card:
    # create the instance of a card
    def __init__(playingCard, suit, rank):
        # "playingCard" is "self"
        # Here we have suits and ranks...
        # For poker, both will need to be strings, as the value of the card makes no difference in the game, only the type of card matters... 
        playingCard.suit = suit   
        playingCard.rank = rank

    # show the card by printing out the rank and suit
    def showCard(playingCard):
        print("{} of {}".format(playingCard.rank, playingCard.suit))
    
class Deck_of_Cards:
    def __init__(deckOfCards):
        # "deckOfCards" is "self"
        deckOfCards.cards = []
        deckOfCards.build()

    # creates deck of cards...
    def build(deckOfCards):
        # step through each rank in each suit
        # if the rank is equal to a 1, 11, 12, or 13, the value changes to the corresponding face card.
        for s in suits:
            for i in range(1, 14):
                if i == 1:
                    deckOfCards.cards.append(Playing_Card(s, "A"))
                elif i == 11:
                    deckOfCards.cards.append(Playing_Card(s, "J"))
                elif i == 12:
                    deckOfCards.cards.append(Playing_Card(s, "Q"))               
                elif i == 13:
                    deckOfCards.cards.append(Playing_Card(s, "K"))
                else:
                    deckOfCards.cards.append(Playing_Card(s, i))
    
    # displays cards in deck...
    def showDeck(deckOfCards):
        count = 0 
        for c in deckOfCards.cards:
            c.showCard()
    
    # shuffles cards in deck...
    def shuffle(deckOfCards):
         random.shuffle(deckOfCards.cards)

    # counts the number of cards in deck...
    def numOfCards(deckOfCards):
        count = 0
        for i in deckOfCards.cards:
            count+=1
        print(count)

    # draws a single card off the top...
    def drawCard(deckOfCards):
        if len(deckOfCards.cards) >= 0:
            for c in deckOfCards.cards:
                c.showCard()
                c.append(dealtCards)
                deckOfCards.cards.pop()
                break

deck = Deck_of_Cards()
deck.drawCard()


        
