# node-cure

Welcome!

This project is a meta-repository for the USENIX Security'18 paper *[A Sense of Time for JavaScript and Node.js: First-Class Timeouts as a Cure for Event Handler Poisoning](https://www.usenix.org/conference/usenixsecurity18/presentation/davis)* by James C. Davis (@davisjam), Eric R. Williamson (@ewmson), and Dongyoon Lee (@dylosy).

In this project:
- We described the "Event Handler Poisoning" (EHP) attack on server-side programs that use the event-driven architecture -- for example, many Node.js applications fit this description.
- We identified many examples of possible EHP vectors in the [snyk.io](https://snyk.io/) vulnerability database.
- We explored *First-Class Timeouts* as an approach to detecting and responding to EHP attacks.
- We documented potential EHP vectors among Node.js core APIs, changed the implementation of `fs.readFile`, and prepared a guide about EHP attacks for [nodejs.org](https://nodejs.org/en/).

The reproducibility package consists of three repositories:
- [node-cure-snykAnalysis](https://github.com/VTLeeLab/node-cure-snykAnalysis): the scripts for our EHP-themed analysis of the Snyk.io database (section 3.4).
- [node-cure-outreach](https://github.com/VTLeeLab/node-cure-outreach): links to our outreach efforts in the Node.js community (section 7).
- [node-cure-prototype](https://github.com/VTLeeLab/node-cure-prototype): the source code for the *Node.cure* prototype (section 5).
