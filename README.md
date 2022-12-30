# cop2805cMod1GPA  
  
This assignment will assess your knowledge of concepts from COP2551C and COP2800C.  
  
- Design and implement a Java program which represents a standard 52-card deck of playing cards.
- The deck must include 4 suits: Clubs, Diamonds, Hearts, and Spades.
- The deck must provide a variable which serves as a collection of 52 Card objects, which  
  are instantiated from a separate Card class with the following characteristics:
  - Each card must include a numeric point value using the "BlackJack" numbering system as follows:
      - Ace (1 point)
      - 2, 3, 4, ... , 10  (2 points, 3 points, 4 points, ... , 10 points)
      - Jack (10 points)
      - Queen (10 points)
      - King (10 points)
  - Each "Face" card - (Ace, Jack, Queen, King) must be identified as such using a private instance variable
  - Each card must include a private instance variable which indicates whether it has been dealt in a hand or not
  - Each card must include a private instance variable which indicates its suit as described above
  - The Card class must include accessors and mutators as required.
  - Include an overridden toString method in your Card class to display the card's state (all instance variable values)  
    Use this method whenever you display a card.
- Your collection object must be either a Java **array** or a Java **ArrayList**,  
  do not use any advanced data structures for this assignment.  
- Your card deck class must include a method to deal a random hand of any size between 1 and 52
  with no duplicates.
    - Hint: I use a naive brute-force algorithm for this feature:
      - start with an empty hand (e.g. an empty array list of cards)
      - loop for the size of the hand (should be a parameter passed to your method)
        - select a random card from the deck (use the Random API with the nextInt method)
        - if the card has not been dealt, add it to the hand and increment the loop index
        - (do not increment the index if the card has already been dealt)
      - once the loop exits, you will have the full hand which is the return value of the method
- Your card deck class must include a method to display a dealt hand
- Test your program by dealing and displaying a single hand

- Sample output is shown below:

card deck created.  
size of hand = 5  
8 of Diamonds (dealt: true)  
King of Spades (dealt: true)  
Jack of Spades (dealt: true)  
2 of Clubs (dealt: true)  
4 of Hearts (dealt: true)  
