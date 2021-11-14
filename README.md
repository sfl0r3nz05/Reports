# Blockchain-based digitization of the Roaming Agreement Drafting Process
- [Blockchain-based digitization of the Roaming Agreement Drafting Process](#blockchain-based-digitization-of-the-roaming-agreement-drafting-process)
    - [Purpose of this Solution Brief](#purpose-of-this-solution-brief)
    - [Intended Audience](#intended-audience)
  - [Abastract](#abastract)
  - [Introduction](#introduction)
  - [The Problem: Methods and mechanisms currently available for drafting and negotiating Roaming Agreements.](#the-problem-methods-and-mechanisms-currently-available-for-drafting-and-negotiating-roaming-agreements)
  - [The Solution: A decentralized blockchain-based platform for the efficient management of Roaming Agreements.](#the-solution-a-decentralized-blockchain-based-platform-for-the-efficient-management-of-roaming-agreements)
  - [Reference Architecture:.](#reference-architecture)
    - [Design details.](#design-details)
    - [Implementation details.](#implementation-details)
    - [Integration with Hyperledger Mentoring Programs.](#integration-with-hyperledger-mentoring-programs)
  - [References](#references)
### Purpose of this Solution Brief
This document describes the transforming of the Telecom Roaming Agreement drafting and negotiation process into a digitalized version based on the transparency promoted by blockchain technology.
### Intended Audience
The audience for this solution brief includes any vendors or users interested in promoting an efficient solution that ensures transparency in the drafting and negotiation of Roaming Agreements between Mobile Network Operators (MNOs).
## Abastract
The ever-growing number of IoT devices means data vulnerability is an ongoing risk. Existing centralized IoT ecosystems have led to concerns about security, privacy, and data use. This solution brief shows that a decentralized ID and access management (DIAM) system for IoT devices provides the best solution for those concerns, and that Hyperledger offers the best technology for such a system.
## Introduction
Roaming  operations  ensure  business  continuity  and  ubiquitous  service  access to  the  end  customer across  various  technology  stacks  including  the  new  5G  and  IoT  technologies. Conceptually, Roaming refers to the capability for a subscriber to access the mobile services offered by the Visited Public Mobile Network (VPMN) via the Home Public Mobile Network (HPMN), when moving out of the coverage range of HPMN [1]. Roaming  services  are an  essential  component  of  an  operator’s  cost  model  with critical  opex  and  capex  impacts. The back office part of this seamless extension of coverage is enabled by the process of wholesale Roaming Agreement, which are technical, commercial, and legal documents that govern the relationship and billing and accounting between the user’s home operator and the visited mobile operator network.

<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram6.PNG">

The Roaming Agreement addresses the technical and commercial components necessary to enable the service to a Roaming Customer, so that it constitutes an essential part of the business, managing issues such as the management of interoperator charges. Therefore conducting a dynamic and transparent roaming agreement drafting process ensures adequate monetization, ensuring the long-term profitability for Telephone company (TELCO).

## The Problem: Methods and mechanisms currently available for drafting and negotiating Roaming Agreements.
The Roaming Agreement addresses the technical and commercial components necessary to enable the service to a Roaming Customer. During the drafting phase of the Roaming Agreement the parties, i.e. the Mobile Network Operators (MNOs), go through a negotiation process that currently still uses asynchronous flows such as email or even regular mail for information exchange. This manual, slow and untrustworthy process has been the reason for the project to promote a transparent negotiation process that ensures the roaming agreement drafting using blockchain technology to record the interactions between MNOs, ensuring reliable traceability. 
A recent study by GSMA [1] enables blockchain for Wholesale Roaming Initiative, however their approach is a rather more general one in terms of negotiation and drafting of the Roaming Agreement.
Such a framework should provide the following capabilities:
* Unique universal identifiers compatible with the internet namespace convention
* Device ownership and lifecycle management from manufacturing to retirement
* Authentication and authorization
* Governance of data access, provenance and privacy
* Advertising of supported “services”
* Ability to adapt and participate in various trust models
## The Solution: A decentralized blockchain-based platform for the efficient management of Roaming Agreements.

Telco blockchain revenue is estimated  to reach around  $1.8b of  $19.9b [3] by  2024.

IoT devices collect, handle, and act on data as proxies for a wide range of users, such as a human, a government agency, or a multinational enterprise.
With tens of billions of IoT devices to be connected over the next few years, numerous IoT devices may represent a single person or institution in multiple roles. And IoT devices may play roles that no one has yet envisioned.
For example, with the rise of autonomous computing powered by machine learning, an IoT device may be able to change roles, ownership, or affiliations dynamically based on external triggers. IoT devices will likely communicate on an ad hoc basis with numerous entities without any pre-existing business relationships.
Decentralized Identifiers (DIDs) enable a standards-based, globally interoperable identity system that puts IoT device owners in control. DIDs enable multiple identifiers to be created at will to help manage anonymity, auditability, correlation across contexts, privacy, revocability, and traceability.
A decentralized ID management system removes the need for any central governing authority and makes way for new models of trust among organizations. All this provides more transparency, improves communications, and saves costs.
## Reference Architecture:.

Figura general de arquitectura

### Design details.
<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram1.PNG">
<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram2.PNG">

### Implementation details.
<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram3.PNG">
<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram4.PNG">
<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram5.PNG">

### Integration with Hyperledger Mentoring Programs.
The Filebeat-Agent is based on the Linux Foundation Project: Blockchain Analyzer: Analyzing Hyperledger Fabric Ledger, Transactions

## References
  1. I. Tanaka, “Volte roaming and interconnection standard technology”, NTT Docomo Technical Journal, vol. 15, no. 2, pp. 37–41, 2013.
  2. Shamit Bhat, "Blockchain for Wholesale Roaming Initiative", online available: https://www.gsma.com/newsroom/wp-content/uploads//GSMA-Blockchain-for-Wholesale-Roaming-MVP-Report.pdf, October 2021.
  3. https://www.globenewswire.com/news-release/2019/10/02/1924300/0/en/Global-Blockchain-in-Telecom-Market-is-Set-to-Reach-USD-1-835-6-million-by-2024-Observing-a-CAGR-of-82-4-during-2019-2024-VynZ-Research.html
  4. Santiago Figueroa-Lorenzo, Ahmad Sghaier, Noureddin Sadawi, and Mohamed Elshrif, "Blockchain-based digitization of the roaming agreement drafting process", online available: https://medium.com/@sfl0r3nz05/blockchain-based-digitization-of-the-roaming-agreement-drafting-process-dec003923521, September 2021.
  5. Santiago Figueroa-Lorenzo, Ahmad Sghaier, Noureddin Sadawi, and Mohamed Elshrif, "NLP Engine to detect variables, standard clauses, variations, and customized texts", online available: https://medium.com/analytics-vidhya/nlp-engine-to-detect-variables-standard-clauses-variations-and-customized-texts-893ff9f903e5, September 2021.2. 
  6. Santiago Figueroa-Lorenzo, Ahmad Sghaier, Noureddin Sadawi, and Mohamed Elshrif, "Chaincode design for managing the drafting of roaming agreements", online available: https://medium.com/@sfl0r3nz05/chaincode-design-for-managing-the-drafting-of-roaming-agreements-73d3ed1b3645, October 2021.
  7. Santiago Figueroa-Lorenzo, Ahmad Sghaier, Noureddin Sadawi, and Mohamed Elshrif, "Chaincode implementation for managing the drafting of roaming agreements", online available: https://medium.com/@sfl0r3nz05/chaincode-implementation-for-managing-the-drafting-of-roaming-agreements-d4ec7363a3d0, November 2021.
