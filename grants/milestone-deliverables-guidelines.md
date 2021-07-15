# Milestone Deliverables Guidelines

We request you to kindly follow these guidelines for milestones submitted for the purpouse of evaluation. 

## Submission

For the **Concordium Free & Open Grants Program**, please submit your milestones via PR to the [Concordium Free & Open Grant Milestone Delivery repository](https://github.com/Concordium/Concordium-Free-Open-Grant-Milestone-Delivery).

## Invoices

All milestones needs to be reviewed and accepted, however you can already submit your invoices through [this form](https://docs.google.com/forms/).

## Content

The submission should contain the following information: 

 * **Name of the grant project**
 * **Link to the open-source code/delivery** 
 * **[License](#license)**
 * **[Documentation](#documentation)**
 * **[Formatted code](#formatted-code), according to a set of guidelines**
 * **[Testing Guide](#testing-guide)**
 * **A list of the [milestone deliverables](#milestone-deliverables)**
 * **Any [additional information](#additional-information)**

## License

It is necessary for the project to have open source code for your Application to receive the grant funding successfully.  . 
We prefer Apache 2.0, but MIT or Unlicense are also acceptable. If your delivery comprises multiple repositories, make sure to include the license for each of them.

## Documentation

Good documentation is a cornerstone of opensource development, hence we appreciate thisalong with highquality effecient code.

We require that you document (where applicable):

- We recommend you provide an Architecture overview and individual component details as much in detail as possible
- Algorithms and protocols defining the core of your project
- Fundamental building blocks of your technology that isnecessary for operational & performance excellence
- API calls where necessary

Make the documentation public as well, ideally as part of the appropriate code repository wherever possible,unless there are strong reasons you desire to do so otherwise. This will make it easier for the Community uses or adapt your project faster when it is in a simple and crisp format.

**Note**: Only focus on your **own** contributions. Do not write detailed explanations of already existing components, e.g. Proof of Stake , SHA-256 etc

## Formatted code

A codebase that is easy to use is generally reader friendly. We suggest adopting one style from the begenning and adhering to it across the entire team.
This helps to keep the commit history clean and facilitates any reviews of the amended changes with time.

For **Rust**, we encourage formatting any additional support libraries or helpers by following the [Style Guidelines](https://doc.rust-lang.org/1.0.0/style/README.html). If you require any additionhelp you can also reach out to the [DevX Initiative](https://devxinitiative.org).

For **any other** deliveries, please commit to a particular style & let us know which official guidelines you adopt.

## Testing Guide

It is generally recommended that every milestone delivery includes a comprehensive test suite or checklist, consisting of:

### Detailed guide showcasing capacity for milestone accomplishments though code.
Documentation on installation, compilation, running and testing the deliverable(s) adds value. Make sure to include all necessary prerequisites. Common issues while replicating test results involved, among others, undocumented dependencies, version numbers, local database setups, breaking changes in the main branch since delivery, OS- and browser-specific incompatibilities. 

Depending on the deliverable, this could include (but is not limited to)
- how to embed your library in another application,
- how to make example API calls to your service,
- running your web app,and
- steps to complete some desired action in your mobile app.

### Unit tests
As with any quality software project, each logical code component should be testable and definable. 
 
### Integration tests
Docker files are great to avoid problems with versions and dependencies.


**Note**: If you are not delivering code as part of your project, such a test suite is not applicable. This mainly applies to projects centering on design, research or hardware. If that is the case, please provide detailed instructions on how else we can test/run/replicate your deliverable.

## Milestone Deliverables

Please provide a list of milestone deliverables. This list should closely reflect the list of deliverables agreed on in the Pull Request for the **Concordium Free & Open Grant Program**.
 
Each item in the list should include a link to the deliverable itself, e.g.:
- Google Doc link - make sure anyone with the link has View access
- GitHub repository - include the appropriate file/folder in the link

**Please highlight anything that deviates from the contract** and include further information that you think is relevant to the deliverable, either alongside the appropriate deliverable or under [Additional Information](#additional-information). 

Please ensure the repo has the correct open-source license.

| Number | Deliverable | Link | Notes |
| ------------- | ------------- | ------------- | ------------- |
| 01. | License | https://github.com/.../LICENSE | ... | 
| 02. | Documentation | ... | ... | 
| 03. | Testing Guide | ... | ... | 
| a. | ... | ... | ... | 
| b. | ... | ... | ... | 

## Additional Information

Please add any additional comments that you consider relevant for the evaluation.
