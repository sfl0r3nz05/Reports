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
Despite its importance, the drafting of roaming agreements faces two major shortcomings. On the one hand, authoritative voices such as [2], define the process of drafting and negotiating roaming agreements as a manual, slow and untrustworthy process. Secondly, although GSMA in a recent study has enabled trust mechanisms for Wholesale Roaming Initiative [3], their approach is a rather more general one in terms of negotiation and drafting of the Roaming Agreement. Hence the need to establish a framework that provides capabilities such as:
* Provide a fine-grained methodology that digitizes the Roaming agreement drafting process.
* Promote a transparent negotiation process between MNOs.
* Ensure traceability in the roaming agreement drafting process.
  
## The Solution: A decentralized blockchain-based platform for the efficient management of Roaming Agreements.
Nowadays, blockchain emerges as an essential technology to ensure transparency, traceability and fine-grain analisys of Roaming Agreement drafting and negociation. This is because on the one hand, blockchain has the potential to transform business processes in all industries, as it eliminates the need for "middlemen" and manual processes because it can ensure the validity of stored data (such as transactions) which cannot be subsequently modified without the change being visible to all parties. While on the other hand, blockchain includes smart contracts that define the transaction logic that controls the lifecycle of a business object contained in the world state.

Despite the advantages of the technology, a blockchain process is not conceivable without the integration of a set of technologies. Considering that blockchain-based solutions involve cross-technology integration where multiple technology stacks can contribute to solving a business problem, this project aims to constitute a solution that while having as its basis the properties and advantages defined for blockchain technology integrates a set of open source technologies such as Natural Language Processing (NLP) technologieswith the aim to: 
1. Build a library of drafting items with a set of variables to be extracted from available templates and previous roaming agreements using the NLP Natural Language Processing process
2. Translate the drafting and negotiation process as a blockchain code in Blockchain to digitize the process and provide a maintainable and actionable copy of the agreement.

## Reference Architecture:.

Figura general de arquitectura

### Design details.
<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram1.PNG">
<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram2.PNG">

### Implementation details.
<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram3.PNG">
<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram4.PNG">
<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram5.PNG">

Toda la arquitectura desplegada docker ELK, ETC, cuña para hablar del otro proyecto

#### Integration with Hyperledger Mentoring Programs.
The Filebeat-Agent is based on the Linux Foundation Project: Blockchain Analyzer: Analyzing Hyperledger Fabric Ledger, Transactions

## References
  1. I. Tanaka, “Volte roaming and interconnection standard technology”, NTT Docomo Technical Journal, vol. 15, no. 2, pp. 37–41, 2013.
  2. ROCCO Research, "The International Roaming Agreement", online available: https://www.roccoresearch.com/portfolio-items/the-roaming-agreement/, 2017.
  3. Shamit Bhat, "Blockchain for Wholesale Roaming Initiative", online available: https://www.gsma.com/newsroom/wp-content/uploads//GSMA-Blockchain-for-Wholesale-Roaming-MVP-Report.pdf, October 2021.
  4. VynZ Research, "Global Blockchain in Telecom Market is Set to Reach USD 1,835.6 million by 2024, Observing a CAGR of 82.4% during 2019–2024", https://www.globenewswire.com/news-release/2019/10/02/1924300/0/en/Global-Blockchain-in-Telecom-Market-is-Set-to-Reach-USD-1-835-6-million-by-2024-Observing-a-CAGR-of-82-4-during-2019-2024-VynZ-Research.html
  5. Santiago Figueroa-Lorenzo, Ahmad Sghaier, Noureddin Sadawi, and Mohamed Elshrif, "Blockchain-based digitization of the roaming agreement drafting process", online available: https://medium.com/@sfl0r3nz05/blockchain-based-digitization-of-the-roaming-agreement-drafting-process-dec003923521, September 2021.
  6. Santiago Figueroa-Lorenzo, Ahmad Sghaier, Noureddin Sadawi, and Mohamed Elshrif, "NLP Engine to detect variables, standard clauses, variations, and customized texts", online available: https://medium.com/analytics-vidhya/nlp-engine-to-detect-variables-standard-clauses-variations-and-customized-texts-893ff9f903e5, September 2021.2. 
  7. Santiago Figueroa-Lorenzo, Ahmad Sghaier, Noureddin Sadawi, and Mohamed Elshrif, "Chaincode design for managing the drafting of roaming agreements", online available: https://medium.com/@sfl0r3nz05/chaincode-design-for-managing-the-drafting-of-roaming-agreements-73d3ed1b3645, October 2021.
  8. Santiago Figueroa-Lorenzo, Ahmad Sghaier, Noureddin Sadawi, and Mohamed Elshrif, "Chaincode implementation for managing the drafting of roaming agreements", online available: https://medium.com/@sfl0r3nz05/chaincode-implementation-for-managing-the-drafting-of-roaming-agreements-d4ec7363a3d0, November 2021.
