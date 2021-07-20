# RFP ( Request for Proposal ) for Alpha Centuri in the Concordium Stack

Dear all, this is where you'll find some ideas that reflect Concordium's needs. Please feel free to reach us out if you have any question or even better, pick one of these ideas and begin to build it!

### Wallets
 * Web Wallet
 For test and development purpose and to be used on Open Testnet including backend service.
 * Community Wallet
 An independent and community driven wallet for $GTU.
 
 ### Telemetry and Reporting
 We need good (web) applications providing information about the blockchain in an unbiased way. This includes information about events on the chain and statistics related to baker economics and performance.
 * Concordium Bot - an extensible chatbot for Matrix/Riot that knows to speak on Matrix.
 * Concordium Telegram Bot – A Telegram bot for monitoring on-chain events.
 * Concordium Tokenomics Statistics – Concordium network statistics. Shows network information and staking details from bakers and intentions. 
 * Concordium Guardian – a CLI tool and a library to monitor on-chain states and events. 
 * ConcordiumScan – A community dashboard.
 
 ### Storage
 Storage of data on the blockchain must be minimized. The blockchain should only be used to store the necessary information for smart contracts, accounts and to register data stored externally (e.g., for provenance or time stamping).

* Tools and librairies that can support functionality for:
  ** registering meta data on the blockchain and store the data off-chain.
  ** retrieve stored meta data and validate its integrity against the chain.

* Integration with several DBs i.e:
    ** ProvenDB
    ** Enterprise DBs (Oracle, MySQL, NoSQL, MangoDB)
    ** Google Cloud
    ** AWS
    ** Microsoft Azure
    ** IBM Cloud
    ** Alibaba Cloud

### Dev Tools
Enhance development tools to provide a good environment for making smart contracts and other applications building on our Blockchain. This may require extensions made by Concordium but we invite for contributions to create tools to provide efficient UI/UX.
* LocalDeV – a local development environment for Concordium including testing and local execution of smart contracts. This may build on top of the tools already provided by Concordium. 
* Concordium Debug Kit (SC and dapps)
    ** SC Development tools – Tools to build SC in Rust on the Concordium Blockchain
    ** May require improvements to Rust debugger
* Concordium-Sign – A tool to build, sign and submit transactions. The Concordium Client does this, but a more user-friendly tool would be nice, and the tool should be more flexible with respect to key handling. Special tools for the following must be considered.
    ** HTTP application for Concordium to make transactions in a web application
    ** Interaction with smart contracts
* Administration/monitoring tools for nodes. The Node Dashboard is the first such tool, but tools providing more functionality and information to the  node runner will be needed. Purpose specific tools could also be useful (e.g., for providing information about earned rewards and information about balances). The tool must run on Mac, Linux and Windows.

### User Interfaces

* Concordium Starter – A starter kit to custom UIs for Concordium (VueJS)
* Concordium Front-End – A starter kit to custom UIs for Concordium (ReactJS)
* Generic smart contract user interface - Possibly limited to work with our SC templates

### Libraries
* Concordium-Wasm – WebAssembly Library for interacting with the chain 
* cWASM – a collection of WebAssembly utilities used on pwasm-ethereum contract development 
* eConcordium – a WebAssembly interpreter for Ethereum-like SC
* SDKs on top of the gRPC interface, including documentation, testing and maintenance for: 
    ** Go
    ** C++
    ** .NET
    ** Python
    ** Java
* SDK for interacting with smart contracts built on top of the above SDK
* SDKs for chain interaction that can be used as a basis for UI tools in general
* Web Service Layer (e.g., Rest)

### Data Conversion
This section deals with tools making it easier to access the information in the blockchain for different, specific purposes:
* Archive - A tool to run alongside a Concordium Node to archive all blocks, states.
* GraphQL Builder - Generate a GraphQL database from a Concordium chain’s data.
* Concordium-storage - A tool which scans Concordium chain and stores balance-relevant transactions in a DB.








