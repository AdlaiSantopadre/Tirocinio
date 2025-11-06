# Tirocinio

## Journal 4 Novembre

## Journal 3 Novembre

## Journal 30 Ottobre (72/150)

**Confronto tra vantaggi e svantaggi delle soluzioni 
1-Hyperledger Fabric  (with std PKI)
2-Hyperledger Fabric with SSI
3-Quora ( Ethereum ) with SSI**


*ref.*
https://www.lfdecentralizedtrust.org/blog/sunsetting-tessera-and-simplifying-hyperledger-besu

**Approfondimento sull'ambito di studio**

Un biofilm è una comunità di microrganismi (come batteri, funghi e alghe) che si attaccano a una superficie e sono incapsulati in una matrice protettiva autoprodotta di sostanze polimeriche extracellulari (come zuccheri e proteine). Questi aggregati si possono formare su superfici inerte, come i dispositivi medici, o su superfici viventi, come i denti. La struttura del biofilm fornisce una maggiore resistenza agli agenti antimicrobici, al sistema immunitario e ad altre condizioni ambientali rispetto ai microrganismi che vivono in forma libera ("planktonica")

*ref.* 
Front. Microbiol., 22 July 2025
Sec. Antimicrobials, Resistance and Chemotherapy
Volume 16 - 2025 | https://doi.org/10.3389/fmicb.2025.1570334
Assessment of the anti-biofilm effect of UV-C irradiation (254 nm) against healthcare associated infections related microorganisms

Introduction: Biofilm-related Multidrug Resistance (MDR) is a major problem in healthcare-associated infections (HAI). Hospital surface decontamination is essential to ensure the safety of patients and to eliminate the dissemination of MDR pathogens. New eco-friendly decontamination technologies, such as UV-C irradiation, are only gaining popularity now, but their use against the biofilm of common microorganisms causing HAI has not been properly assessed. We aimed to assess the efficacy of UV-C irradiation (254 nm) in a 2-phase study by assessing its anti-biofilm effect against sessile cells from microorganisms of hospital interest.


B. Casini, M. Scarpaci, F. Chiovelli, S. Leonetti, A.L. Costa, M. Baroni, M. Petrillo, F. Cavallo,

Antimicrobial efficacy of an experimental UV-C robot in controlled conditions and in a real hospital scenario,

Journal of Hospital Infection,
Volume 156,
2025,
Pages 72-77,
ISSN 0195-6701,
https://doi.org/10.1016/j.jhin.2024.11.010.
(https://www.sciencedirect.com/science/article/pii/S019567012400389X)

## Journal 29 Ottobre (64/150)

**Approfondimento Documentazione ufficiale Fabric**

Peers,Orderers,Chaincode,Ledgers, Organizations,Applications,Fabric Gateway,Identity,Membership Service Providers,Policies,Transactions lifecycle,

## Journal 28 Ottobre (56/150)

**Approfondimento dell`ecosistema LF Hyperledger con studio del capitolo 14 del testo Mastering Blockchain**
https://www.hyperledger.org
Mastering Blockchain, Fourth Edition

Chapter 14, Hyperledger, presents a discussion about the Hyperledger project from the Linux Foundation, which includes different blockchain projects introduced by its members.

## Journal 27 Ottobre

**Approfondimento sul contesto**

Casini, B.; Tuvo, B.; Scarpaci, M.; Totaro, M.; Badalucco, F.; Briani, S.; Luchini, G.; Costa, A.L.; Baggiani, A.
Implementation of an Environmental Cleaning Protocol in Hospital Critical Areas Using a UV-C Disinfection Robot.
Int. J. Environ. Res. Public Health 2023, 20, 4284. 
https://doi.org/10.3390/ijerph20054284

## Journal 25 Ottobre ()

**Indagine sugli utilizzi e gli aspetti tecnici della DLT Blockchain in ambito IOT**

*ref*
Shikha Mathur, Anshuman Kalla, Gürkan Gür, Manoj Kumar Bohra, Madhusanka Liyanage,
A Survey on Role of Blockchain for IoT: Applications and Technical Aspects,

(https://www.sciencedirect.com/science/article/pii/S1389128623001718)
Abstract: In recent times, IoT has emerged as a new paradigm for the interconnection of heterogeneous, resource-constrained, and communication-capable smart devices. It has been anticipated as a key enabler for various domains of applications such as health care, automotive, agriculture, industrial operations, automation, energy, and the next generation of living. However, the current IoT applications face significant challenges in terms of the huge amount of collected data, intensive data exchange, security, privacy, centralized processing, and interoperability. To mitigate many of these issues, blockchain has been identified as a promising innovative technology. Blockchain, in conjunction with smart contracts, has received significant attention both from the industry and academia and offers features such as irreversibility, non-repudiation, proof of provenance, fault tolerance, pseudonymity, decentralized operations and decision-making, and distributed ledger. The integration of blockchain with IoT requires essential insights concerning the application areas, scalability, security, privacy, data college and storage, performance, and governance. Thus, this paper intends to expound on the opportunities and key aspects of using blockchain in the IoT landscape. Specifically, this paper surveys the utilization of blockchain for various IoT applications. Besides, the paper distinguishes different technical aspects and presents the associated research challenges. At last, future research directions are discussed depending on the lessons learned.
Keywords: Blockchain; Smart contracts; DLT; Internet of Things (IoT)

## Journal 25 Ottobre (48/150)

**Implementazione di una rete di peers privata secondo il Framework Besu con algoritmo di consenso QBFT**

-Configure and run a private QBFT(POA) Besu Network 

-Deploy and configure a new validator node

-Deploy and explore analitics tools

*ref*
https://besu.hyperledger.org/public-networks/concepts/node-clients

What's a full node?
...
Ethereum's Proof of Stake (PoS) protocol leverages two separate P2P networks supporting separate clients. Execution clients gossip transactions over their network, enabling them to manage their local transaction pool. Consensus clients gossip blocks over their network, enabling consensus and chain growth. A validator node also runs the validator client.
...
(Ethereum Merge node)
As as result of the 2022 Merge, Ethereum Mainnet transitioned from Proof of Work (PoW) to PoS consensus.
Execution and consensus clients
Under PoS, a full Ethereum Mainnet node is a combination of an execution client (previously called an Eth1 client client) and a consensus client (previously called an Eth2 client). The consensus client uses the Engine API to communicate with the execution client.
Execution clients

Execution clients, such as Besu, manage the execution layer, including executing transactions and updating the world state. Execution clients serve JSON-RPC API requests and communicate with each other P2P.

Besu is an execution client that you can run with:

    Any consensus client on Mainnet.
    Any consensus client on a testnet.
    Teku on Mainnet.
    Teku on a testnet.

Consensus clients

The consensus client (also known as the beacon node, CL client or, formerly, the Eth2 client) implements the PoS consensus algorithm, which enables the network to achieve agreement based on validated data from the execution client. Consensus clients serve REST API requests and communicate with each other P2P.

Consensus clients, such as Teku contain beacon node implementations. The beacon node is the primary link to the Beacon Chain (i.e. the consensus layer). A consensus client can run without the (bundled) validator to keep up with the head of the chain, allowing the node to stay synced.
Validator clients

To operate a validator node, node operators must also run a validator client and deposit the required ETH into the deposit contract. The validator client handles attestations and block proposal — i.e. performs validator duties on the consensus layer. The validator client may either be run in the same process as the beacon node or separately.

Validators earn rewards for performing validator duties, and fee recipients also earn rewards for the inclusion of execution layer transactions.

## Journal 18 Settembre (40/150)

**La Blockchain e le primitive di sicurezza di cui fa uso**
*registrazione su Bleanded Uniurb della lezione 01/04 del 21 Maggio 2025 tenuta dal Prof.Aldini nell`ambito dell`insegnamento Sicurezza Informatica**

**Approfondimento su modelli di autenticazione , access control e scalabilità**

*ref*
M Kokila, Srinivasa Reddy K,
Authentication, access control and scalability models in Internet of Things Security–A review,
Cyber Security and Applications,
Volume 3,
2025,
100057,
ISSN 2772-9184,
https://doi.org/10.1016/j.csa.2024.100057.

"It is necessary to make the necessary adjustments to the architecture of IoT applications to accomplish end-to-end security in IoT environments.
...

Security aspects such as authentication, authorization, privacy, confidentiality, availability, and integrity form the basis for information exchange in a trusted environment.
...

Keyless Signature Infrastructure (KSI) is a globally distributed system that uses hash-function cryptography and a blockchain-like technology to provide immutable and time-stamped digital signatures for data. Unlike traditional Public Key Infrastructure (PKI), KSI 
does not rely on the secure management of private keys for verification, as it creates a 
secure, timestamped record of data’s state by chaining hashes together in a time-ordered manner. This makes it useful for verifying the integrity and authenticity of data across an 
information supply chain without needing to establish trust between all parties in advance. 
...
OAuth and token-based authentication provide secure mechanisms for authorizing device 
access to services and resources without sharing passwords, using standards like OAuth 
for access delegation and tokens (e.g., JSON Web Tokens, JWT) for managing sessions and 
information transmission securely."



## Journal 12 Settembre (32/150)

**Permissive / Non permissive Blockchain
Public /Private Blockchain

Algoritmi di consenso:Pratical ByzantineFaultTolelance PBFT

Hyperledger Fabric (ecosistema)**



Mastering Blockchain
@book{bashir2023mastering, title = {Mastering Blockchain: Unlocking the World of Cryptocurrencies, Smart Contracts, and Decentralized Applications}, author = {Bashir, Imran}, edition = {4}, year = {2023}, publisher = {Packt Publishing} }

## Journal 11 Settembre (24/150)

**Unified Modeling language-
Applicazione di diagrammi UML alla analisi dei requisiti per il modello DCMS""

Diagramma concettuale del modello
Diagramma dei casi d'uso
Diagramma sequenziale

## Journal 10 Settembre (16/150)

**Analisi dei requisiti non-funzionali**

Non-functional requirements
"In systems engineering and requirements engineering, a non-functional requirement (NFR) is a requirement that specifies criteria that can be used to judge the operation of a system, rather than specific behaviours ....The plan for implementing non-functional requirements is detailed in the system architecture, because they are usually architecturally significant requirements"

quote wikipedia

Definizioni

Availability 
Security
Usability
Scalability
Reliability

## Journal 9 Settembre (8/150)

**Progetto Sanichain/Analisi dei requisiti funzionali del sistema di Disinfection and Cleaning Management System**

Contesto Analisi dei metodi di igienizzazione tradizionale,dei punti carenti della disinfezione operata da personale ,delle prospettive di nuovi prodotti ,nuove tecniche,e della introduzione e di metodi di trattamento con luce UV in modo automatico.Documento non conclusivo del 2016

JM Boyce, Modern technologies for improving cleaning and disinfection of environmental surfaces in hospitals., in Antimicrobial resistance and infection control, vol. 5, 2016, p. 10, DOI:10.1186/s13756-016-0111-x, PMC 4827199, PMID 27069623.

