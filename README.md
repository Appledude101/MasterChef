This is a proof of concept for a project and should not be used in any real applications without proper due dillagence.
USE AT YOUR OWN RISK!!!!

# MasterChef
All Contracts used injected web-3 through remix. In order to write to the contracts, you will need to use the contract through remix.

Step 1: Go to contract adress below and copy the source code.  
Step 2: Paste source code into file on remix and compile it (make sure you are using correct version of compiler!).  
Step 3: Go to Deploy and Run Trasactions, DO NOT DEPLOY WHAT YOU COMPILED! Instead choose the enviroment to be injected web-3 and then in
the At Address paste the contract address you copied the source code from.  
Now you should see the contract you wanted to interact with under deployed contracts. You can then use the functions on remix to then interact with the contract on the Rinkeby Testnet.  

# Contract Addresses on Rinkeby Testnet:  
Apple Token: [0x3cC148f103Af20f43ebfcFc15bc5bbF172c6B1d0](https://rinkeby.etherscan.io/address/0x3cc148f103af20f43ebfcfc15bc5bbf172c6b1d0) (Use Compiler Version 0.6.12)  
AppleMasterChef: [0xa55Ef7630c19a050733F2D0848493b07300EA57f](https://rinkeby.etherscan.io/address/0xa55ef7630c19a050733f2d0848493b07300ea57f) (Use Compiler Version 0.6.12). 

Currently AppleMasterChef only has one LP-Pool, but it is really just a single sided staking for the apple token itself. There was initially 1,000,000 apple minted before AppleMasterChef was made owner of the token. In order to earn more apple you must now stake apple in the LP-Pool with PID=0. Once more LP's are added, then there will be more opportunities to earn apple.  

To test deposit/withdrawl/rewards: (Can see transaction history under this wallet [0x7b94ec20B75A4818B252bcd25A3b52c477FEb0c6](https://rinkeby.etherscan.io/address/0x7b94ec20b75a4818b252bcd25a3b52c477feb0c6)). 
1. Deposited 100,000 Apple.
2. Withdrew 100,000 Apple. (Emmisions were set to 0 so no rewards gained).  
Then emmisions where set to 1 Apple per block and allocation changed from 0 to 1 so that emmisions would be gained.  
1. Deposited 100,000 Apple.  
2. Withdrew 100,000 Apple from the pool and recieved 100,036.3 Apple (33 Apple as rewards from the contract and 3.3 Apple as the Dev Fee)
