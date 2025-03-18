This collection of Java programs provides functionality for translating between Morse code and English text.
1. MorseToEnglishTranslator
This program translates Morse code into English letters.
It uses two arrays:
morseCode[]: Stores Morse representations of each letter (A-Z).
letters[]: Stores corresponding English letters.
It takes Morse code input, splits it by spaces (each Morse sequence represents one letter), and converts it to English.
Key Method:
translateToEnglish(String morse):
Splits the Morse code by spaces.
Loops through each Morse character and finds the matching letter.
Appends it to a StringBuilder and returns the final translation.
2. MorseCodeTranslator
This program translates English text into Morse code.
It stores Morse representations in morseCode[] (same as previous).
Takes input from the user, converts it to uppercase, and maps each letter to its Morse code.
Key Method:
translateToMorseCode(String word):
Loops through each letter of the input word.
Converts it to Morse by looking up the array index (c - 'A' gives the position of the letter in morseCode[]).
Adds spaces between Morse symbols for readability.
3. MorseToWords
This program handles both Morse-to-English and English-to-Morse conversions.
It distinguishes words in Morse code using three spaces (" ") between them.
Uses morseAlphabet[] and letters[] arrays for mapping.
Key Methods:
morseToWord(String input):

Splits input into words (using triple spaces " ").
Splits words into Morse letters (using single spaces).
Finds matching English letters and reconstructs the word.
wordToMorse(String input):

Converts each letter to lowercase.
Matches it to Morse code and adds spaces.
Uses three spaces (" ") between words.
main(String[] args):

Takes user input to choose between translation options.
4. main Method (Final Combined Program)
This combines both English-to-Morse and Morse-to-English translation.
Uses an instance of MorseCodeTranslator to call both translation methods.
Key Flow:
Asks the user for a word and converts it to Morse code.
Asks for a Morse input and converts it back to English.
How the Programs Work Together
The first two programs (MorseToEnglishTranslator and MorseCodeTranslator) perform one-way translations (either Morse → English or English → Morse).
The third program (MorseToWords) adds support for word separation.
The last snippet integrates both conversions into one main method.
