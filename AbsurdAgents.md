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
  <li>Jumble: In this game, we pick a word from the lexicon, and try ro unjumble it. </li>
</ol>

<h3>Interface</h3>
We present a novel interface for implementing a server that allows us to play word games like Wordle, Hangman, etc. In our implementation, the user must choose a game to which the directory would change. For example, if the user selects “Wordle”, we switch to the Wordle directory. Subsequently, the user would be asked if they want the agent to suggest the appropriate guess or the agent to play the game on several iterations and produce stats. If the latter is selected, the stats produced would be the accuracy and number of strikes it needed on average for guessing.

<h2>Hangman</h2>

<h2>Wordle</h2>

<h2>Nerdle</h2>

<h2>Jumble</h2>

<h2>Word Ladder</h2>

**Definitions**

**Connected words:** Two words are said to be connected to each
other if they both have the same characters at all except **only**
**one** index.

**Mesh:** A data structure containing all the connections of words,
implemented as a dictionary.

**Start:** The initial word provided by the server.

**Target:** The final word we have to reach from the start.

**Current** **word:** The word we currently are at.

**Step:** The number of changes made to the start.

**Branch:** One path from the start to the current word.

**Depth** **of** **a** **Branch:** Number of words in the branch

<h3>Approachto solve</h3>

**Breadth-first search algorithm**

The Breadth-first search algorithm is based on searching for all paths
that are possible to be taken from the start. Each path or branch is
calculated simultaneously, i.e., the depth of all branches is the same
after each iteration.

All the words explored during computations are stored after each
iteration, and the target is searched each time before the next
iteration of the loop starts. Once we find the target, we exit the loop,
and each branch is then searched for the target. The branch containing
the target is the shortest path possible i.e. the optimal solution of
the given word ladder.
