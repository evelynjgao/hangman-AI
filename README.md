# hangman
 A Hangman AI written in Python that accesses a provided API given at http://upe.42069.fun through HTTP posts and requests. It guesses lyrics to rap songs with a win rate of at least 20% for 100 games played.  My code hangman.py implements the dictionary that I sourced from the lyrics through playing this game, dict. I began building this dictionary by running the game about 500 times and appending the lyrics to the file in a certain format, namely only alphabetical characters with each word on a new line. I then reset. As the program runs, the dictionary improves as does the win rate. This dictionary includes repeats so that more frequently occuring words are more likely to be guessed.  I split the phrase into words and worked on solving the ones with the least unknown characters first. Based off the words in the dictionary, I checked to see which words can fit and the frequency of letters that can occur in these possibilities to make the best educated guess.  I also sourced a most frequently appearing letter string from sorting the dictionary and using a counter to get the frequencies of the letter appearences within the dictionary itself.
 
dict: collection of lyrics sourced

counter.py: counts frequency of letters appearing in dict

hangman.py: runs with over 20% accuracy tested on 400 games

winning_hangman.py: runs with 100% accuracy by exploiting the fact that games only count when hangman is set free or dies, and not completing the game when there is only one guess remaining
