# RFP ( Request for Proposal ) for Concordium | Sirius

Dear all, this is where you'll find some ideas that reflect Concordium's needs. Please feel free to reach us out if you have any question or even better, pick one of these ideas and begin to build it!

Concordium brings trust in innovating technologies. 

Trust and reliability is the key to business. Concordium differs from other blockchains by offering previously unseen guarantees of transparency, and regulation without compromising privacy: i) Built-in identity management, ii) Compliance readiness by design, iii) Low stable transaction fees, iv) Deployed smart contracts and token standard, v) Fast, secure and real finality at scale.
Concordium Mainnet went live in June 2021 and our focus now includes connecting to the blockchain ecosystem and building tools for a first class developer and integrator experience.  

  
  ## eSealing 
* Published May 9, 2022
* Status: Closed (July 11, 2022)

Service for eSealing of files (photos, documents, data sheets)

#### Overall goals and scope of proposal

We want to enable anyone to easily eSeal documents on blockchain. The service contains two functionalities: Ease of access to tamper proof sealing of files and verification check of sealed files.
* Ease of access to tamper proof sealing of files: Anyone with an Concordium account should be able to take a file and submit it to the service, The file is then hashed and a transaction of the ‘Register Data’ type is created with the file’s hash in the memo field. The user can then use his wallet to sign and send the transaction to the blockchain paying the transaction fee. 
* Verification check of sealed files: Anyone (this does not require an account) should be able to take a file and then submit it for a verification check. The file is then hashed and it is checked whether there are transactions on-chain that contain the hash in the memo field. If this is the case, then the transaction number, sender and date is listed. If there are more than 1 transaction that meets the criterion they are listed with the oldest at the top. 
  
  
#### Ideas and hints for solution design

We imagine the solution to be a website that makes it possible to drag and drop files, prepare a transaction that is then signed with the mobile wallet and later also web wallet - when the web wallet becomes available. In the same website it should be possible to verify or check a file for any earlier registrations. Furthermore, the website should leave space for documentation of the service and explanation of the functionality and benefits. 
The solution should also contain API endpoints to the functionalities. The entire code should be open sourced. 

For inspiration, we encourage you to have a look at this [Registry Service](https://notary.northstake.dk/) which contains much of the same functionality, except that this service only timestamps files and transactions are signed from a centralized account. The code for this service is available for reuse if relevant.  


#### Elements of proposal
Possible of table of contents for the proposal
* Our understanding of the project
* Solution description - potentially basic mock-ups 
* Project team, timeplan and Budget 

We anticipate that the time needed to complete this project will be 30-40 hours. Yet larger project proposals are welcome 

We look forward to receiving your proposal and collaborating on this project. For any questions please reach out to Keld Stehr Nielsen, +45 51714334, [ksn@concordium.com](mailto:ksn@concordium.com)

Sincerely
Concordium AG

  
  
  
  
  
  
  ## Registry Storage
* Published April 11, 2022
* Status: Open
  
  
Document folder or database that automatically generates tamper proof registrations of document content on the Concordium Blockchain 
  
  
#### Background
There is already a small application running on Concordium that showcases a central capability of the blockchain: The possibility to easily create tamper proof registrations of information and the possibility easily for anyone to access that registration - and easily being able to trust the authenticity of the record. 
This basic service (link) registers the hash of a data set, document or photo in a simple transaction that has a timestamp. By the nature of the blockchain this registration is tamper proof. After that, anyone can prove for a particular document that it was not changed after the initial registration. The service also includes API enabled endpoints.
  
  
#### Overall goals and scope of proposal

We want to extend the registry service to include an off-chain document storage facility. As a user, you should be able to store your files in a location that is integrated to the Concordium Registry service via the API endpoint. More specifically, you should be able to:
* Set up and manage a specific folder or database on a document storage facility (e.g. AWS, IPFS, Google Drive, GCP, Microsoft office, Apple MacOS, Apple Cloud) so that documents in that folder or database are automatically hashed and registered using the Concordium Registry Service. 
* Documents should be automatically registered on Concordium 1) when it is first moved and saved in the folder, and 2) if the document content is changed. This could for instance be achieved either via an event based solution or via daily/scheduled registrations.
* (optional) Via a simple app keep status of when documents were registered on the blockchain.  
    
Imagined High level process flow:
<p align="center">
  <img src="https://github.com/Concordium/Concordium-Free-Open-Grants-Program/blob/main/src/Registry storage example.png" style="width:500px";>
</p>
  
We imagine the ideal solution to be 
* a set of detailed instructions that for a set of large storage storage providers (e.g. AWS, IFPS, Google Drive, GCP, Microsoft office, Apple MacOS, Apple Cloud) explains how to connect a document folder or database to the registry service so that automated registrations can be done. 
* Code snippets or a small application needed to automate the registration and configure it.
* A simple browser based app that keeps track that can be connected to a folder and keeps track of the documents’ registrations.     
  

#### Elements of proposal

  Possible of table of contents for the proposal
* Our understanding of the project
* Solution description - potentially basic mock-ups 
* Project team, timeplan and Budget 

We anticipate that the time needed to complete this project will be 30-40 hours. Yet larger project proposals are welcome 

We look forward to receiving your proposal and collaborating on this project. For any questions please reach out to Keld Stehr Nielsen, +45 51714334, ksn@concordium.com

Sincerely
Concordium AG




## Certification Lookup
* Published April 11, 2022
* Status: Closed (July 11, 2022)

Service for retrieving information about Concordium accounts

#### Overall goals and scope of proposal
We want to enable anyone to easily check online data that is available for a particular Concordium account. This could be useful e.g. prior to making a transfer to that address, or to check which Id provider issued the ID underlying the account. 

The application developed should allow a user to enter an account address. The app then retrieves information about the owner of the account, such as
* Number of credentials and threshold (Multiuser accounts will have more than one credential)
  
 For each credential:
- ID provider (Genesis, Notabene, DTS)
- Anonymity revokers
- Public attributes (i.e., attributes which are published on  the chain)
- Date of issuing
- Date of expiry of the underlying ID object

Most of this is public information which can be retrieved from the node directly. Getting and displaying the right names and logos for IDPs and ARs requires a little extra work, but is not complicated.

Simplified sample screenshot:
<p align="center">
  <img src="https://github.com/Concordium/Concordium-Free-Open-Grants-Program/blob/main/src/Account lookup example.PNG" style="width:300px";>
</p>
    
  We imagine the ideal solution to be
- Webpage that enables search on individual accounts and provides instructions for how to use the service
- API endpoints for the service 

#### Elements of proposal

Possible of table of contents for the proposal

- Our understanding of the project
- Solution description - potentially basic mock-ups 
- Project team, timeplan and Budget 


We anticipate that the time needed to complete this project will be 30-40 hours. Yet larger project proposals are welcome 

We look forward to receiving your proposal and collaborating on this project. For any questions please reach out to Keld Stehr Nielsen, +45 51714334, ksn@concordium.com

Sincerely
Concordium AG


### Are these projects not for you? Check our open RFPs from Alpha Centauri: https://github.com/Concordium/Concordium-Free-Open-Grants-Program/blob/main/rfps/RFP-Alpha-Centauri.md



    
