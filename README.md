## Blockchain Novella

### What?
This project is a collaborative writing application where multiple people can write a short story or
passage together by suggesting and voting on the next word to be appended to the story.

After a word is suggested, there will be a countdown which allows alternative word suggestions, and
a voting period to take place. Once the countdown ends and voting has finished, the word is immutably
appended to the novella and the next word suggestion can take place.

### Why?
The purpose of this project is to practice the creation of smart contracts written in Solidity, in
a more abstract and creative use-case than the previous projects I've created.

Creating a project like this which utilises smart contracts in a slightly more unique way than
most current use-cases for smart contracts will undoubtedly reveal some new challenges to solve,
making this project a good way to improve my abilities in creating robust and efficient contracts.

### Ideas
* Haiku mode - the passage automatically terminates once a haiku has been created
* NFT creation - an NFT containing the passage is automatically created and distributed to participants 
once the passage has been completed

### Challenges
#### Transaction Efficiency
People won't want to pay gas for every single word that is added to the passage, and being forced to waste
gas on a passage that isn't very good will drive people away from using the application.

###### Potential solution
One option to avoid this is to locally store the last 'n' completed passages, and display an option to
'mint' the passage which then triggers a transaction. That way, nonsensical passages won't waste the users 
gas, and they can choose which passages are their favourites.

The incentive to mint a passage comes from the creation of an NFT containing the passage, which is 
distributed to whoever minted the passage.