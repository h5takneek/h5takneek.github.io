You'll find the detailed report and documentation of Nawabs' solution of the 'Absurd Agents' PS here!

<h2>The Problem Statement</h2>
<ol>
<li>Implement a server that allows people to play word games like
Wordle, its variants, and Hangman. Details are left to your
imagination, but there should be a feature to let us use our dictionary.</li>
<li>For each game in your service, implement agents that play the game
optimally, mentioning the rationale behind your choice of algorithms
in the report. Rule of thumb, more stats == more marks. </li>
</ol>

<h2>Introduction</h2>
<h3>The Games</h3>
<ol>
  <li>Wordle: Wordle is a web based word game. Players have six attempts to guess a five-letter word, with feedback given for each guess in the form of colored tiles indicating when letters match or occupy the correct position. Every day, a five-letter word is chosen which players aim to guess within six tries. After every guess, each letter is marked as either green, yellow or gray: green indicates that letter is correct and in the correct position, yellow means it is in the answer but not in the right position, while gray indicates it is not in the answer at all. Multiple instances of the same letter in a guess, such as the "o"s in "robot", will be colored green or yellow only if the letter also appears multiple times in the answer; otherwise, excess repeating letters will be colored gray. 
 </li>
  <li>Hangman: Hangman is a guessing game. We'll have a pre-decided word, which we will have to guess. he word to guess is represented by a row of dashes representing each letter or number of the word. Rules may permit or forbid proper nouns, such as names, places, brands, or slang. If the guessing player suggests a letter which occurs in the word, the other player writes it in all its correct positions. Otherwise kf the letter is not in the word then, one of our chances will be eliminated. </li>
  <li>Nerdle: Nerdle is a guessing game like Wordle, but here we have to form a basic mathematical equation using numbers and symbols. </li>
  <li>Word Ladder: Word ladder is a word game where we have the start word and a specified end word. We have to find a chain of other words to link the two, in which two adjacent words (that is, words in successive steps) differ by one letter.</li>
  <li>Jumble: </li>
</ol>
