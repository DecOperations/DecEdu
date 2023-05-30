# Smart Contracts
Hi! Welcome to DOTPI or the Developer Onboarding Training and Placement Initiative



# Files

 - [ ] What is a smart contract
 - [ ] Popular Languages of smart contracts.
 - [ ] Common Attacks
 - [ ] ~~Writing and Deploying Smart Contracts~~

StackEdit stores your files in your browser, which means all your files are automatically saved locally and are accessible **offline!**

____
What is a smart contract?

Any code deployed on blockchains (broad use),
in general more accurately defined as **finite state machines**

Common Public Definition (likely inaccurate) from Kraken Exchange website:

-  Smart contracts are self-executing contracts defined by computer code, most recognizable in the form of applications built on platforms such as the Ethereum blockchain.

___
Common Attacks

1. Overflow Attacks: Overflow occurs when a mathematical operation results in a value larger than the maximum limit allowed by the data type. In the context of Ethereum smart contracts, an overflow attack can happen when an attacker manipulates the arithmetic operations within a contract to generate unexpected values, potentially leading to unintended consequences or vulnerabilities.

2. Underflow Attacks: Underflow is the opposite of overflow. It happens when a mathematical operation results in a value smaller than the minimum limit allowed by the data type. Similar to overflow attacks, underflow attacks can exploit vulnerabilities in smart contracts by manipulating arithmetic operations to produce unexpected and potentially harmful results.

3. Rentrancy Attacks: Rentrancy attacks exploit the re-entrancy vulnerability in smart contracts. This vulnerability occurs when a contract allows an external contract to call back into its own code before completing previous execution. An attacker can repeatedly call the contract and drain its funds or manipulate its state in unintended ways.

4. Oracle Attacks: An oracle is a third-party service or entity that provides external data to a smart contract. Oracle attacks involve manipulating or compromising the data provided by the oracle to mislead the smart contract. By feeding incorrect or manipulated data, attackers can trick the contract into making incorrect decisions or executing malicious actions.

5. Front Running Attacks: Front running occurs when an entity, typically a miner or an insider, exploits their knowledge of pending transactions to gain an unfair advantage. In the context of Ethereum smart contracts, front running attacks involve monitoring the mempool for transactions containing specific function calls, then quickly executing similar transactions with higher gas fees to manipulate the contract's state or gain financial advantage.

6. Poison Token Attacks: Poison token attacks involve the creation or manipulation of tokens within a smart contract ecosystem to exploit vulnerabilities. Attackers may create tokens with malicious code or hidden functions that can be exploited to compromise the contract or deceive other users.

7. Time Manipulation Attacks: Time manipulation attacks involve exploiting vulnerabilities related to the handling of timestamps or time-related functions in smart contracts. Attackers can manipulate the contract's perception of time to execute specific actions or gain advantages, such as front running or manipulating time-based rewards or penalties.

8. Transaction Order Dependence (TOD): TOD attacks exploit the fact that the order of transactions in a block can impact the outcome of a smart contract. By carefully orchestrating multiple transactions in a specific order, attackers can take advantage of race conditions or unexpected interactions between contracts to their benefit.

9. Cross-Chain Attacks: Cross-chain attacks target vulnerabilities that arise when interacting with other blockchains or external protocols. Attackers exploit inconsistencies or differences in the security models, consensus mechanisms, or communication protocols between different chains to manipulate transactions, steal assets, or compromise the smart contract.

10. Access Control and Permissions: Attackers may exploit weaknesses in access control mechanisms within smart contracts to gain unauthorized privileges or manipulate critical functions. This can include bypassing permission checks, impersonating privileged users, or manipulating the contract's state to gain unauthorized control.

11. Malicious Code Injection: Malicious code injection attacks involve manipulating smart contracts by injecting malicious or unintended code. Attackers may exploit vulnerabilities in contract deployment processes or target vulnerable dependencies to introduce code that can compromise the contract's integrity, security, or functionality.

12. Reentrancy Guard Violation: Reentrancy guard attacks occur when a smart contract fails to properly implement or enforce reentrancy guards. These guards are meant to prevent reentrant calls from other contracts during the execution of critical functions. If the guard is improperly implemented, an attacker can exploit this vulnerability to repeatedly re-enter the contract and manipulate its state or drain its funds.

13. Denial-of-Service (DoS): DoS attacks aim to disrupt or disable the normal functioning of a smart contract by overwhelming it with resource-intensive operations or malicious requests. Attackers may exploit inefficiencies or vulnerabilities in the contract's design or dependencies to consume excessive gas, block execution, or cause the contract to become unresponsive.

14. Dependency Attacks: Dependency attacks involve exploiting vulnerabilities in external dependencies or libraries that a smart contract relies on. Attackers target weaknesses in the implementation or security of these dependencies to manipulate or compromise the contract's behavior or data.

15. Delegatecall and Callcode Attacks: Delegatecall and callcode are low-level functions in Ethereum that allow contracts to invoke code from other contracts while preserving the context of the calling contract. However, if these functions are not used carefully, they can introduce vulnerabilities. Attackers can leverage delegatecall or callcode to manipulate the execution flow, exploit unintended interactions, or escalate privileges within a contract.

16. Chain Reorganization Attacks: Chain reorganization attacks take advantage of Ethereum's consensus mechanism, which occasionally allows for the reorganization of blocks. Attackers can execute transactions or perform actions on the blockchain, only to have those actions invalidated later due to a chain reorganization. This can be used to manipulate the contract's state or deceive other users.

It's worth noting that new types of attacks may emerge as the Ethereum ecosystem evolves. Staying informed about the latest security practices, participating in security audits, and regularly updating your smart contract code is the industry standard!

___
Types of Contracts

NFTs, Fungibles, Services, On/Off-Chain Oracles, Governance, Voting, Time Locks, Storage, Multi-Signature Wallets, and TCRs, 

****
Standards -


EIP vs. ERC

EIP -> Ethereum Improvement Proposal
ERC -> Ethereum Request for Comment
 
Common Standards ->

ERC-20 -> Fungible Standard -> Think Water

ERC-721 - NFT standard  -> Think Snowflake

ERC-1155 - Multi-Token Standard combines 721 and 20 into 1 can be used for things such as in game items -> In game might look like Item category of Currency (NFT type), Gold (type Erc-20), Silver (Currency ERC-20)

EIP - Wallet signing


Terms - 

Audit -> Companies like [Certik](https://www.certik.com/), [OpenZeppelin](https://www.openzeppelin.com/), & [ConsenSys Diligence](https://consensys.net/diligence/), do a extensive review and evaluations vulnerabilities to peer review the code and dependencies, data inputs, user functions etc. to give a second signoff to communities and management typically.

Block -> List of txs processed and added to ledger in sequence hence a chain of blocks blockchain

dApp -> Decentralized application

Explorer -> Shows info about blockchain tx

Hash -> Cryptographic generated value (usually by signed message SIWE)

Initialization - Loading variables that remain static into the solidity code on deployment.

Internal vs External Transactions -> Smart contract vs user initiated actions on blockchain.

Testnet -> Environment where realtime test contracts, tools, tokens and dapps operate at no cost for Q&A (typically pre launch)

Token - NFT or FT is a non fungible smart contract based on mapped values to accounts on the ethereum plockchain

Turing Complete - **A computational system that can compute every Turing- computable function** is **called Turing-complete (or** Turing-powerful)
Scope & Permissions - Public and private Functions



Tooling


Web Environments

[Remix](https://remix.ethereum.org/) - Web based solidity/Ethereum IDE


CLIs -

Hardhat -  [Hardhat | Ethereum development environment for professionals by Nomic Foundation](https://hardhat.org/)

Foundry - [Introduction - Foundry Book (getfoundry.sh)](https://book.getfoundry.sh/) 


Packages & Tools:

[OpenZeppelin](https://www.openzeppelin.com/) - Provides security products to build, automate, and operate dApps

[OpenZeppelin | Defender](https://www.openzeppelin.com/defender) - Secure operations platform for smart contracts

[Safe – Previously Gnosis Safe ](https://safe.global/) - Crypto wallet, web3 account abstraction developer stack

[OpenZeppelin Contracts Wizard](https://wizard.openzeppelin.com/) - Audited premade boilerplate contract generator

[Chainlink Documentation](https://docs.chain.link/) -> General functions, Blockchain Oracles for Connected Smart Contracts

[Crytic/evm-opcodes](https://github.com/crytic/evm-opcodes) -Ethereum OpCodes - Ethereum opcodes and instruction reference.


Tools:

[Alchemy](https://alchemy.com/?r=e17e6ebd4cbbb1be) - Node Endpoint creation 

[Tenderly | Ethereum Development Platform](https://tenderly.co/) - Smart Contract GUI FULL FEATURED

[Etherscan](https://etherscan.io/) - Endpoint 


Simulations ->

[ETH.Build - Educational Sandbox For Web3](https://eth.build/)


Pragma (Version)

General Rules - 
A. No public user defined inputs when posible
B.


Static vs. Upgradable =>

Static - Unchangable deployed smart contract.

Upgradable - Changeable through a Proxy contract: 2 types UUPS and Transparent

Standard vs. Defacto Standard -> 

Essentially while some things arent included into the standard (eg. ERC-20) they may have been added to a "defacto" standard which means a best practice or adopted for convivence while not necessary for the standard.


Steps for deployment

 - Setup Dev Environment with Hardhat
 - Create new Hardhat project
 - Configure .env with your API keys
 - Write deploy script
 - Compile contract after importing from OpenZeppelin Wizard
 - Deploy to testnet
 - Deploy to mainnet 
 - Migrate to etherscan
 - Done!
