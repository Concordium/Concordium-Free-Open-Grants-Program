# Free & Open Grant Proposal Technical Template
## Project name
The name of the project is: 
* CCD Node gRPC Exporter

## Project overview
 
### General
* Prometheus exporter that scrapes downtime and meta information for a specified remote or local CCD Node. All data is collected from a blockchain node via gRPC requests. CCD Nodes do not export these metrics by default. We will open source this monitoring solution and make it for every node operator available. We want to develop such tool, since we operate nodes ourself and require a monitoring solution.

### Description 
We work based on a "reverse-engineering" approach. We kindly ask you to: 
* Define the final product, we like teams who dream a little bit here
All in one monitoring solution for any concordium node operator.
* Describe in a reverse mode, what are the steps you aim to follow to reach your goal
We already identfied the need for such product and already scetched out a conecpt. The implementation and testing is still missing.
* Describe the current problems/issues you are encoutering
Currently no problems, beside finding the time to develop said product.
* Define how Concordium could help you
Assistance in questions related to the gRPC endpoint of the node and promoting the final product.

### Submission
Please submit the following (if and when relevant): 
* The CCD Node gRPC Exporter will be running in its own docker container. The exporter will scrape a remote or local CCD Node in a defined time interval and will expose the metrics for prometheus so that alerts e.g. for nodes out of sync can be configured. 
The deployment and configuration with Docker will be as easy as one line of code.

### Benchmark

Please name the projects you are compeeting with: 
* None what we are aware of.

### Team
* [David Bohnhoff](https://www.linkedin.com/in/david-bohnhoff/) – Virtual Hive GmbH CEO
* [Robert Grütze ](https://www.linkedin.com/in/robert-gruetze/) - Virtual Hive GmbH CTO - [Github](https://github.com/UltraViolentLight)
* [Christian Bohnhoff ]() - Virtual Hive GmbH CIO


### Website
* https://virtualhive.io

### Legal
If relevant, what's the structure you're going to use in order to develop and commercialise your project? 
N/A, since completely open source.

## Development 
This is the most important part of the application. This section shall explain in detail, the milestones of your project. These milestones will appear in the grant agreement. 
Please find below a roadmap example: 
### Overview
* Total Estimated Duration: ~10 days
* Full-Time Equivalent (FTE): 1.5 FTE
* Total Costs: $15k. 

### Deliverables

| Action| Deliverable | Specs |
| -------- | -------- | -------- |
| 0.1   | License     | MIT    |
| 0.2   | Documentation     | Complete documentation, which describes deployment, usage and maintance.   |
| 0.3   | Complete Source Code in Github     | To build from scratch.    |
| 0.4   | Prebuild Docker Image in Container Registry     | For docker deployment.    |
| 0.5   | Grafana Dashboard     | Grafana Dashboard Template to visulize metrics.   |

### Community and marketing
A medium blog post will be released which describes the deployment, usage and maintance of the CCD Node gRPC Exporter. 

### What's next?
* We will await the grant and will start the development right away.

