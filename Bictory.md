# Free & Open Grant Proposal Technical Template
## Project name
The name of the project is: Bictory

## Project overview
 
### General
Bictory builing CEX (centralized exchange) for GTU, custom Concordium issued tokens, 
wrapped tokens and other tokens. Our CEX will leverage Concordium identity layer 
for KYC of our users. 

By bringing to life such CEX Bictory will promote Concordium technology as a 
working proof of applications build on top of it and let interact with a blockchain 
to a wide crowd of public, as with technology itself and with Concordium native 
token and new tokens issued on top of it as well.Every user of our CEX will need 
to register at Concordium to create ID.

Our integration with Concordium blockchain will be conducted by maintaining
set on concordium-nodes (HA). Bictory application's backend servers will be 
comunicate with concordium-nodes throw API. API will wrap gRPC interface 
exposed by concordium-node. Our user in order to pass KYC will upload JSON
this id to CEX (when mobile Concordium mobil wallet will support login by 
QRcode this proccess will be much easier)

Our team have vast expirience in blockchain projects, security and scalability 
and we excited about Concordium blockchain identity layer, fast confirmation
and multilanguage smart-contracts (wasm target compatible). We see this as
a opportunuty to build a needed product on new top-notch emerging technology.

### Description 
Following "reverse-engineering" approach we can describe our final product as 
secure, scalable, reliable and fast CEX with legit permission to operate. 
Each feature passed internal security review, we continiusly check our project dependency 
for CVE and each developer familiar with OWASP. Our autoscalable architecture allow
us to keep going with a high load and release resource when where are no need. 
For new region expantion we have well defined terraform fileset (IaC).
Each part of backend system issue logs, and we are checking on system health with Grafana. 
Our UI/UX is a result of long term A/B testing - login proccess simplifed to scan QR-code with 
Concordium app. Same with KYC proccess. Having "Build-in" KYC will help us to
be keep best fees for our users and be in compliance with vast government regulations.


To reach this goal our steps in reverse mode:
* Writing IaC to provition infrastructure in new regions   
* 24h devops support by 3 shifts
* Penitration test
* We check system performance for bottlenecks to rewrite some code in Rust   
* Different benchmarks
* Configuration of Grafana for easy data analysis
* Our cloudbased infrastructure fully provitioned from code (IaC)
* Setting up A/B testing       
* Code refacored, 
* Adding features, testing
* Product owner update features, set new prioroties. 
* Production env deployed and tested & fixed
* POC ready
* Production env provisioned and CI/CD pipleline updated
* Added swagger comments for endpoints, code coverege >90% by automatic tests
* Software architector keep supervition of POC and working on detailed design for dedicated parts of system	
* We have well defined CI/CD pipeline proccess on GitLab with full range of code checkes, from style to static code analysis
* Frontend and backend teams agree on some API, Frontend working on UI and getting data from api stub. Backend provition staging env in cloud, write dockerfiles and docker compouse file to setup local development env.
* We define initial CI/CD pipeline proccess on GitLab, define code review proccess, picking agile approach to project management 
* Software architecture begin analysis and prepare high-level design for POC   
* We make some mockups, discuss ideas and product owner populate backlog with user stories 
* We have idea of CEX

Current problems/issues you are encoutering:
* At the moment we hiring project manager to keep development proccess more organized

How Concordium could help you?:
* We can work together on requirements,definition of an authentication/compliance/KYC 
proccess by Concordium wallet and to be beta testers and to implementators of this feature

### Submission
* You can access CEX UI at http://3.12.144.216/ This internal deploy, please don't try to use real tokens, this CEX running on testnet. After registration, confirmation email will be sent. If you don't find it - please check your spam folder

<p align="center">
  <img src="src/bictory_1.png" style="width:800px";>
</p>

<p align="center">
  <img src="src/bictory_2.png" style="width:800px";>
</p>

<p align="center">
  <img src="src/bictory_3.png" style="width:800px";>
</p>

<p align="center">
  <img src="src/bictory_4.png" style="width:800px";>
</p>

### Benchmark

Please name the projects you are compeeting with: 

### Team

Development team (Backend & Frontend)
* https://github.com/Elam-Harnish
* https://ng.linkedin.com/in/paschal-obba-a7222aa2
* https://gitlab.com/udori
* https://www.linkedin.com/in/rafael-scrooppi/
* https://www.linkedin.com/in/shakhzod-ayibjonov


### Website
https://bictory.io

### Legal

## Development 
Roadmap: 
### Overview
* Total Estimated Duration: Duration of the whole project (i.e 32 weeks)
* Full-Time Equivalent (FTE): 40
* Total Costs: $99k. 

### Milestone 1
* ED: 10 weeks
* FTE: 12
* Cost: $45,000 


| Action| Deliverable | Specs |
| -------- | -------- | -------- |
| 0.1   | License     | MIT    |
| 0.2   | Documentation     | Technical documentation   |
| 0.3   | Concordium-backend bridge     | Backend code connected to concordium-node throw gRPC wrapper   |
| 0.4   | Infratsructure for support of any new token     | Alpha Release of token adapter.      |
| 0.5   | KYC     | Check user identity. User upload JSON     |
| 0.6   | GTU support on DEX     | Deposite/withdraw/sell/buy functionality    |
| 0.7   | System benchmark     | System stress test, check system under load    |
| 0.8   | Penetration test     | Penetration test by 3rd party and our CISO   |

### Milestone 2
* ED: 10 weeks
* FTE: 14
* Cost: $22,500


| Action| Deliverable | Specs |
| -------- | -------- | -------- |
| 0.7   | Backend dashboard     | Development of Backend dashboard     |
| 0.8   | Documentation: Login/KYC throw Concordium mobile wallet     | Cooperate with Concordium define API for Login/KYC functionality     |
| 0.9   | Login/KYC throw Concordium mobile wallet implementation     | First implementation on feature   |
| 1.0   | Custom token's support on DEX     | Deposite/withdraw/sell/buy functionality for custom token issued on Concordium blockchain |
| 1.1   | Ticket system integration     | Integration with 3rd party backend system |

### Milestone 3
* ED: 12 weeks
* FTE: 14
* Cost: $32,000


| Action| Deliverable | Specs |
| -------- | -------- | -------- |
| 1.2   | legal opinion     | legal opinion     |
| 1.3   | Regulatory compliance     | GDPR compliance, automatic archiving of financial info  |
| 1.4   | Identity Revoking anonymity     | Functionality for revoking anonymity in response from cort request    |




### Community and marketing
As a part of the program, we kindly are asking you to produce content that explains your project. It could be videos, blog posts or press hits. 
This is a mandatory requirement to get a grant. 

### What's next?
Please add here what ever makes sense for your future activities. 


