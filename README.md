# TwitterCloneW3

This is a decentralized Twitter clone application built on Ethereum Blockchain, utilizing the power of smart contracts. The application provides functionalities similar to Twitter, such as tweeting, viewing tweets, deleting tweets, and updating user profiles. The application is divided into two main parts: the smart contract built with Solidity and the client-side application built with React.

Specifications

Any user should be able to read all the tweets.
All the tweets should be ordered in a chronological order.
Any user should be able to write tweets.
A user should be able to update a tweet they wrote.
A user should be able to delete a tweet they wrote.
Deleting a tweet should NOT affect the access to the other tweets.
Deleting a tweet should NOT affect the order of the other tweets.
Smart contract(s) should be deployed to Ropsten.
Smart contract(s) should be tested with at least 80% line coverage.

Project Setup

Create a virtual wallet Metamask account and select "Rinkeby Test Network". If you're unfamiliar with this process, consider reading this article.

Get testnet Ether (ETH) to test and troubleshoot our decentralized application. You can get it from Chainlink and Rinkeby Faucet.

Create an account on Alchemy and generate an API key by creating an app. This will allow us to make requests to the Rinkeby Test Network.

After cloning the repo, create a .env file in the same format as .env.example and fill in your keys.

**Installation and Running the Project**

Ensure you have installed Git, Node.js (using nvm is recommended).

**Clone the repository to your local machine:**
1. git clone
**Testing the Smart Contract**
Navigate to the server directory and test the smart contract:
cd server
npx hardhat test

**Deployment**
Navigate to the server directory and deploy the smart contract:

Copy the generated contract address and paste it in the config file.
NOTE: You can also run the scripts inside package.json inside the server directory.

After deploying your smart contract, you can copy the generated contract address and check it out on the Rinkeby Etherscan.


##Smart Contract
This application is powered by a Solidity smart contract named 'Twitter'. The contract provides the core functionalities of the application, such as adding, fetching, and deleting tweets, as well as updating user profiles.

##Functions
`addTweet(string memory tweetText,string memory tweetImg)`: Function to add a new tweet. It requires 0.01 Ether to upload a tweet.
`getAllTweets()`: Function to fetch all tweets.
`getMyTweets()`: Function to fetch all tweets of a specific user.
`getTweet(uint256 id)`: Function to fetch a particular tweet.
`deleteTweet(uint tweetId,boolisDeleted)`: Function to delete a tweet. Only the owner of the tweet can delete it.
`updateTweet(unit256 id)`:Function to update a tweet. Only the owner of the tweet can update it.
`updateUser(string memory newName,string memory newBio,string memory newProfileImg,string memory newProfileBanner)`: Function to update user details.
`getUser(address userAddress)`: Function to get user details.

##Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

##Troubleshooting
If you run into any issues when following the setup instructions do not hesitate to contact me. We would appreciate your feedback!
