# Blockchain-based digitization of the Roaming Agreement Drafting Process
- [Blockchain-based digitization of the Roaming Agreement Drafting Process](#blockchain-based-digitization-of-the-roaming-agreement-drafting-process)
    - [Purpose of this Solution Brief](#purpose-of-this-solution-brief)
    - [Intended Audience](#intended-audience)
  - [Abstract](#abstract)
  - [Introduction](#introduction)
  - [Roaming Agreement Overview.](#roaming-agreement-overview)
  - [The Problem: Methods and mechanisms currently available for drafting and negotiating Roaming Agreements.](#the-problem-methods-and-mechanisms-currently-available-for-drafting-and-negotiating-roaming-agreements)
  - [The Solution: A decentralized blockchain-based platform for the efficient management of Roaming Agreements.](#the-solution-a-decentralized-blockchain-based-platform-for-the-efficient-management-of-roaming-agreements)
  - [Reference Architecture.](#reference-architecture)
  - [Application lifecycle](#application-lifecycle)
  - [Solution Design Details.](#solution-design-details)
    - [NLP-Engine design](#nlp-engine-design)
    - [Chaincode design](#chaincode-design)
  - [Implementation details.](#implementation-details)
    - [NLP Implementation](#nlp-implementation)
    - [Detection of Variables](#detection-of-variables)
    - [Analysis based on Amazon Comprehend](#analysis-based-on-amazon-comprehend)
    - [Comparisons of sub-articles](#comparisons-of-sub-articles)
    - [Analysis of Similarities](#analysis-of-similarities)
      - [Populate the file with the classification of articles/sub-articles](#populate-the-file-with-the-classification-of-articlessub-articles)
    - [Chaincode Implementation lifecycle](#chaincode-implementation-lifecycle)
      - [Chaincode implementation details](#chaincode-implementation-details)
    - [Integration with Hyperledger Mentoring Programs.](#integration-with-hyperledger-mentoring-programs)
  - [Future works](#future-works)
  - [References](#references)
  
### Purpose of this Solution Brief
This document describes the transforming of the Telecom Roaming Agreement drafting and negotiation process into a digitalized version based on the transparency promoted by blockchain technology.

### Intended Audience
The audience for this solution brief includes any vendors or users interested in promoting an efficient solution that ensures transparency in the drafting and negotiation of Roaming Agreements between Mobile Network Operators (MNOs).

## Abstract
The project looks at how to facilitate the process of Telecom Roaming Agreements drafting and negotiation. The project looks at first constructing a library of drafting articles with a set of variables that will be extracted from the available templates and previous Roaming Agreements using Natural Language Processing process NLP. The second part will be towards translating the drafting and negotiation process as a chaincode on Blockchain to digitalize the process and provide a maintainable and actionable copy of the agreement. The project focuses on how to be able to digitalize the legal process and make it automated through smart contracts to be more efficient and less error prone.

## Introduction
Roaming operations ensure business continuity and ubiquitous service access to the end customer across various technology stacks including the new 5G and IoT technologies. Conceptually, Roaming refers to the capability for a subscriber to access the mobile services offered by the Visited Public Mobile Network (VPMN) via the Home Public Mobile Network (HPMN), when moving out of the coverage range of HPMN [1]. Roaming services are an essential component of an operator’s cost model with critical opex and capex impacts. The back office part of this seamless extension of coverage is enabled by the process of wholesale Roaming Agreement, which are technical, commercial, and legal documents that govern the relationship and billing and accounting between the user’s home operator and the visited mobile operator network.

<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram6.PNG">

The Roaming Agreement addresses the technical and commercial components necessary to enable the service to a Roaming Customer, so that it constitutes an essential part of the business, managing issues such as the management of interoperator charges. Therefore conducting a dynamic and transparent Roaming Agreement drafting process ensures adequate monetization, ensuring the long-term profitability for Telephone company (TELCO).

## Roaming Agreement Overview.
To standardize the legal commercial aspects of the Roaming Agreement, the GSM Association broadly outlines the content of such Roaming Agreement in standardized form for its members [2]. Thus, based on these GSMA-defined template standards, MNOs should be concerned with conducting the Roaming Agreement drafting process as part of a negotiation process. On the one hand, during the drafting process of the Roaming Agreement, the parties should analyze the articles contained in the standard templates to determine whether:

1. Leave an article as found in the template thereby establishing a standard clause.
2. Introduce certain variations in the articles/sub-articles, by changing variables, e.g., MNO, dates, penalties, currencies, and so on concerning the original text, i.e., the GSMA templates.
3. Introduce completely new articles/sub-articles that respond to particular interests by constituting customized texts.
4. Specify the value of certain variables that are found in a certain text, such as dates, names of entities, amounts, and others.

On the other hand, the lifecycle of the Roaming Agreement negotiation process is presented as the compilation of a set of best practices integrated into 7 phases. These phases do not represent standards or rules that must be followed in a mandatory way.

<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram11.PNG">

## The Problem: Methods and mechanisms currently available for drafting and negotiating Roaming Agreements.
Despite its importance, the drafting of Roaming Agreements faces two major shortcomings. On the one hand, authoritative voices such as [3], define the process of drafting and negotiating Roaming Agreements as a manual, slow and untrustworthy process, since it is mostly very ‘analog’ with successive exchanges of information between the parties using traditional means such as email or regular mail. Secondly, although GSMA in a recent study has enabled trust mechanisms for Wholesale Roaming Initiative [4], their approach is a rather more general one in terms of negotiation and drafting of the Roaming Agreement. Hence the need to establish a framework that provides capabilities such as:

* Provide a fine-grained methodology that digitizes the Roaming agreement drafting process.
* Promote a transparent negotiation process between MNOs.
* Ensure traceability in the Roaming Agreement drafting process.
  
## The Solution: A decentralized blockchain-based platform for the efficient management of Roaming Agreements.
Nowadays, blockchain emerges as an essential technology to ensure transparency, traceability and fine-grain analysis of Roaming Agreement drafting and negotiation. This is because on the one hand, blockchain has the potential to transform business processes in all industries, as it eliminates the need for "middlemen" and manual processes because it can ensure the validity of stored data (such as transactions) which cannot be subsequently modified without the change being visible to all parties. While on the other hand, blockchain includes smart contracts that define the transaction logic that controls the lifecycle of a business object contained in the world state.

Despite the advantages of the technology, a blockchain process is not conceivable without the integration of a set of technologies. Considering that blockchain-based solutions involve cross-technology integration where multiple technology stacks can contribute to solving a business problem, this project aims to constitute a solution that while having as its basis the properties and advantages defined for blockchain technology integrates a set of open source technologies such as Natural Language Processing (NLP) technologies with the aim to:
 
1. Build a library of drafting items with a set of variables to be extracted from available templates and previous Roaming Agreements using the NLP Natural Language Processing process
2. Translate the drafting and negotiation process as a blockchain code in Blockchain to digitize the process and provide a maintainable and actionable copy of the agreement.

## Reference Architecture.

Figura general de arquitectura

## Application lifecycle

Decir que el NLP engine termina formando un template que sirve como base pero que puede ser modificado.

Figura general de arquitectura
<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram2.PNG">

## Solution Design Details.
The design details are approached both from the NLP Engine point of view and from the Chaincode point of view.

### NLP-Engine design
To determine as accurately as possible the presence of these four characteristics as part of each of the articles that make up the Roaming Agreement in this project, a tool for text processing and analysis based on Natural Language Processing (NLP) has been designed, which is hereinafter referred to as the NLP engine.

The logic designed for the NLP Engine has two approaches: detection and comparison.

- Detection represents the location of variables in the Roaming Agreement.
- Comparison is performed between each sub-article present in the Roaming Agreement concerning the sub-articles present in the GSMA template.
  
While a near-total coincidence between texts at the sub-article level represents a standard clause, a near-zero coincidence between texts (or simply the non-existence of the sub-article) represents a customized text. The intermediate case is represented by the variation where there is a high coincidence and the differences are given by the presence of variables such as MNO, date, currencies, etc.

### Chaincode design
From a design point of view, the project chaincode is defined by actions and statuses, where interactions through actions allow the transition between each of the statuses. The statuses represent the different phases and transitions starting with the enabling of a Mobile Network Operator (MNO) until it reaches the final signed Roaming Agreement with another counterparty, MNO. Therefore, it is necessary to put the focus on the statuses that govern the chaincode. Thus, the chaincode for Roaming Agreement negotiation consists of three stages: (1) Statuses for Roaming Agreement Negotiation, (2) Statuses for the Articles Negotiation and (3) Statuses for the Article Drafting.

The Statuses for Roaming Agreement Negotiation allows the negotiation to be conducted at the highest level, to determine when the final version of the Roaming Agreement is reached. Without being too rigorous with each of the transitions that take place, the **Figure XXX** shows each of the states that make up this stage. Thus, in the initial status, the MNOs must be enrolled, which enables either of the two MNOs participating in the negotiation to propose to initiate the Roaming Agreement drafting process. Once the initiation of the agreement is confirmed, the negotiation of the drafting of articles and sub-articles proceeds, where the other stages are involved, ending with a proposal and confirmation of acceptance of the Roaming Agreement.

<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram7.PNG">

The negotiation at the articles level is an intermediate stage to determine whether all the articles belonging to the Roaming Agreement have reached the status of being accepted by both parties. Thus, as shown in the **Figure XXX**, belonging to the Statuses for the Article Drafting stage, once an article is added, it goes through a transition of proposed changes until finally the article is accepted by both parties.

<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram8.PNG">

However, the fact that all articles are in accepted status by both MNOs at a given time does not necessarily imply that the Roaming Agreement is close to being reached, but both entities may intend to add a new article despite that all currently added articles are in an accepted status. For this purpose, the Statuses for the Articles Negotiation stage exists. As shown in the **Figure XXX**, the function of this stage is to control the status of all articles added. For this, it establishes a transient status that determines that all added articles are accepted. On the one hand, this stage allows continuing the article drafting process if a new article is proposed. On the other hand, this stage allows moving towards the achievement of the final version of the Roaming Agreement.

<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram9.PNG">

As mentioned, the transition between states is due to the interaction between the two parties through the identified actions. From a programming point of view, the actions are performed through chaincode methods, which are invoked or queried using the frontend application through a middleware/backend service. The **Table XXX** defines the set of design methods that are part of the chaincode.

<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Table1.PNG">

## Implementation details.
<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram1.PNG">

Toda la arquitectura desplegada docker ELK, ETC, cuña para hablar del otro proyecto

### NLP Implementation
The **Figure XXX** shows the overall architecture of the NLP Engine that integrates over a docker infrastructure, establishing as inputs the Roaming Agreement, as well as the GSMA templates; as processing layer the logic associated to the NLP Engine and as output the classification of articles in of standard clauses, variations, customized texts, and variables.

<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram12.PNG">

### Detection of Variables
Variable detection goes through the following steps:
1. A parsing of the Roaming Agreement document converted into text is carried out, removing undesired characters.
2. The parsed text is divided into groups of 100 words, from which entities, key phrases, and syntax are detected using the Amazon Comprehend tool [1].
3. Post-processing mechanisms are applied based on the combination of the detected elements, i.e., entities, key phrases, and syntax.

### Analysis based on Amazon Comprehend
Entities, key phrases, and syntax are detected using Amazon Comprehend Tool. Each piece of text (100 words) sent to the Amazon Comprehend tool via REST API returns a list of objects as shown in expression (1) when entities have been detected. This information is combined with processing and validations based on expression (2) and expression (3), allowing to determine variables. Expression (2) constitutes an object of the list of objects returned by Amazon Comprehend when key phrases are detected. Expression (3) also constitutes an object of the list of objects returned by Amazon Comprehend when syntax analysis is performed.

Expression (1):
```
{‘BeginOffset’:0,’EndOffset’:8,’Score’:0.43067169189453125,’Text’:’Proximus’,’Type’:’ORGANIZATION’}
```

Expression (2):
```
{‘BeginOffset’:0,’EndOffset’:24, ‘Score’:0.956875205039978,’Text’:’Proximus reference offer’} (2)
```

Expression (3):
```
{‘BeginOffset’: 0,’EndOffset’:8,’PartOfSpeech’:{‘Score’:0.9324524402618408,’Tag’:’PROPN’} (3)
```

### Comparisons of sub-articles
To establish comparisons between text elements a pre-processing step is necessary:
1. A parsing of the Roaming Agreement document converted into text is carried out, removing undesired characters.
2. The parsed text is divided into articles, which in turn are divided into sub-articles.
3. The sub-articles are used to establish the degree of similarity concerning the reference represented by the GSMA template.
4. In the case that from the similarity analysis it is determined that the sub-article is a variation, then we proceed to look for the respective variables within the variations.

### Analysis of Similarities
Similarity analysis, in this project, consists of comparing the sub-articles of the Roaming Agreement with the sub-articles used as reference. The similarity analysis is based on Jaccard’s similarity [5], which has been selected because of its simplicity of implementation for this stage of the project. However, the way the code of this project has been developed allows using other similarity types such as cosine similarity. Expression (4) also constitutes an object of the list of objects returned by Jaccard similarity when the sub-article 1.1 is compared with one Roaming Agreement concerning the sub-article present in the GSMA template.

Expression (4):
{‘id’: ‘1.1’, ‘similarity’: 0.7380952380952381}

#### Populate the file with the classification of articles/sub-articles

Once the determination of the variables is performed, the subsequent similarity analysis to classify sub-articles into standard clauses, variations, and customized texts and the existing variables within the variations have been identified, further processing is carried out to populate the file with the classification of articles/sub-articles.

### Chaincode Implementation lifecycle
**Figure xxx**  illustrates part of the set of methods that make up the chaincode life cycle. The invocation of these methods establishes the transition between the different states of the chaincode. This transition takes place at three application levels as shown in **Table xxx**. The following section focuses on providing details of the different modules that make up the chaincode and that make it possible to carry out the above-mentioned interactions.

<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram3.PNG">
<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Table2.PNG">

#### Chaincode implementation details
The chaincode implementation consists of 6 modules which are described below:
1. **Proxy**: This module receives the interactions from the off-chain side and routes them to the different points within the chaincode.
2. **Organization**: This module contains all the interactions related to organizations, allowing to create a new organization, querying existing organizations, etc.
3. **Agreement**: This module contains all interactions related to the Roaming Agreement, allowing users to add and update articles by specifying the articles variables values, variations selection and any proposed custom text. Also, this module handles article state transactions (e.g., proposed-to-accepted) and the possible proposed changes.
4. **Identity**: This module is inserted inside the proxy and allows identity verification using the Client Identity Chaincode Library (cid).
5. **Util**: This module contains common functionalities for the rest of the modules, e.g., UUID generation.
6. **Models**: This module contains the definitions of variables, structures and data types supported by the chaincode. In addition, different error types are defined for proper error handling.

The integration between the different modules takes place in each of the methods defined for the HFB chaincode. Considering that the chaincode methods were defined in **Table XXX**, we will now focus on a single method to analyze how the integration between modules takes place. The selected method is proposeAgreementInitiation, which has been defined as the proposal to initiate the Roaming Agreement drafting by one of the two participating MNOs, causing the transition from the initial state to the started_ra as shown in **Figure XXX**:

<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram10.PNG">

**Figure XXX** below shows the sequence diagram illustrating the relationship between the modules defined above.

<img src="https://github.com/sfl0r3nz05/Report/blob/main/images/Diagram5.PNG">

In this way, a registered MNO enables the drafting of a Roaming Agreement. Thus, the Proxy Module enables interactions with other modules. Firstly, the Identity Module allows verifying the MNO Identity. The Organization Module verifies whether the MNO exists, i.e. has been previously registered. Considering that the names of the two participating organizations and the Roaming Agreement name constitute the input arguments, the Agreements Module performs the following functionalities:

1. Generation of the unique identifier for the list of Articles: *articlesId*
2. Generation of the unique identifier for the Roaming Agreement: *RAID*.
3. The *started_ra* event is emitted.
4. The Status for the Roaming Agreement Negotiation is set as *started_ra* and contained as part of the emitted event.
5. The Status for the Articles Negotiation is set as init.

The main conclusion we can reach is that each method involves the verification, update, or generation of states, which are stored as parts of the data structures established for the chaincodes and traced thanks to the events emitted from each of the methods.

### Integration with Hyperledger Mentoring Programs.
One of the most remarkable points of this project is the integration with other Open Source projects belonging to the Hyperledger Mentoring program. In particular, it has used the Filebeat agent created within the framework of the project "Analyzing Hyperledger Fabric Ledger, Transactions, and Logs using Elasticsearch and Kibana" [6] to display on a Kibana dashboard the transactions executed on our network.

## Future works
1. The Natural Language Processing phase has been carried out from the construction of a NLP engine, so a future line of work is the construction of a Model based on open source libraries such as Spacy.
2. A drafting library in JavaScript, packaged and published as an NPM package.

## References
  1. I. Tanaka, “Volte roaming and interconnection standard technology”, NTT Docomo Technical Journal, vol. 15, no. 2, pp. 37–41, 2013.
  2. GSMA, “Direct Wholesale Roaming Access Agreement Version 2.7 08 December 2017,” London, 2019.
  3. ROCCO Research, "The International Roaming Agreement", online available: https://www.roccoresearch.com/portfolio-items/the-roaming-agreement/, 2017.
  4. Shamit Bhat, "Blockchain for Wholesale Roaming Initiative", online available: https://www.gsma.com/newsroom/wp-content/uploads//GSMA-Blockchain-for-Wholesale-Roaming-MVP-Report.pdf, October 2021.
  5. S. Gupta, “Overview of Text Similarity Metrics in Python,” May 15, 2018, 2018. [Online]. Available: https://towardsdatascience.com/overview-of-text-similarity-metrics-3397c4601f50. [Accessed: 24-Jul-2021].
  6. Balazs Prehoda and Salman Baset, "Analyzing Hyperledger Fabric Ledger, Transactions, and Logs using Elasticsearch and Kibana", 2019, Online]. Available: https://wiki.hyperledger.org/display/INTERN/Analyzing+Hyperledger+Fabric+Ledger%2C+Transactions%2C+and+Logs+using+Elasticsearch+and+Kibana.