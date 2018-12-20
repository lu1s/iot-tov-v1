# A Crypto-warranty and Transfer of Value Interface for Connected Devices
## Disclaimer about this document
```txt
(c) Copyright 2018,2019. [es-mx: Derechos Reservados 2018,2019.]
Author nickname: lu1s.
The author and company holds and reserves the rights of the content of this document.
All public repositories and documents will be published at https://github.com/lu1s/iot-tov-v1 unless
otherwise expressed in a future version of this document.

K_DOCUMENT_TITLE: "+LKNC$: Crypto warranty and transfer of value interface for connected devices."

lkn.sign.201811120000916590000.e3434.
```

## IETF key words disclaimer
In many standards track documents several words are used to signify the requirements in the specification.

These words are often capitalized.  This document defines these words as they should be interpreted in IETF documents.

Authors who follow these guidelines should incorporate this phrase near the beginning of their document:

_The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in RFC 2119._

The arrange of capital letters "US" is not related and do not mean the United States of America country within this document, and it is meant to be interpreted as the ecosystem provider or implementator or as described in the RFC derived from this work or otherwise expressed in a future version of this document.

The citizenship of the author or authors is classified yet it will be declassified.

## Preamble
In recent years the global growth in matter of many topics including and emphasizing the technological ones has been circumnstantially big, and as a natural and also circumnstantial effect it has also created bigger challenges for the leaders of public and private organizations for them to enable and share those technological achievements of the human kind, with their own ecosystems and entities, and with the ones whom they relate with.

The work presented here is a compilation of efforts, ideas, code bases, business models, terms, conditions, privacy policies, licenses and other informations that as a whole they represent secure technology for a fair enhancement of health and wellness of an economy. 

Within this document, a State or Country is any Sovereign Entity that with the appropiate terms, conditions, privacy policies, licenses and a Currency Emissor Approved Assembly (CEAA), or an Entity which serves as so; it is capable of building and maintaining a fair and stable ecosystem and thus a healthier and more fairly distributed economy.

As an example, and in the particular case of México (the Country; as a whole Set of Connected States), the CEAA is today[1] the "Bank of Mexico" (also known as "Banco de México" or "BoM"). The BoM is the Entity in charge of all the currency emission, recycling and control within the country and for the countrie's interests.

_\[1\] Today as of 201812100002136190000, and invalidated if wrong._

The following projects are the first demonstrations of MVV of multiple integrated MVPs that comply with the MRQ each of them so that at the end the full CoVA the ToV can be demonstrated in "real time" by a complete and conciliated set of PoAVs between the SIO and the SEUs providing sufficient MRS for the prevention and detention of misuse of the described crypto warranties.

## Broad concepts and entities

_The key words listed here are unordered and presented in form of a draft_

| Acronym        | Name                                    | Description                                                              |
|----------------|-----------------------------------------|--------------------------------------------------------------------------|
| FSF            | Free Software Foundation | 
| GNU            | The FSF GNU Operating System | 
| GNUFL          | The GNU Fortran Language | 
| COBOL          | The Common Business Oriented Language | 
| COBOLIT        | The Open Source Alternative to the COBOL | 
| KLANG          | The K Programming Language |
| ABM            | Asociacion de Bancos Mexicanos |
| IETFMX         | Internet Engineering Task Force in MEXICO | 
| IETF           | Internet Engineering Task Force | 
| RFC            | Request For Comments (IETF) |
| RFCNR          | Request For Comments Not Requested | The RFCNR is a set of one or more conversation threads 
| DRFCE          | Draft of RFC with Errata | 
| DRFCC          | Draft of RFC that is Clean (without Errata) |
| PRFC           | Published RFC (Internet Standard) |
| DoH            | DNS-over-HTTPS | Standarized format and protocol for sending Domain Name System (DNS) queries through HTTP rather than the traditional DNS protocol (RFC-8484). 
| PoK            | Proof of Knowledge | The PoK is a valid proof that certain expected knowledge is conceived by one or more individual entities.
| RPoHC          | Real Proof of Human Consent | The RPoHC is a valid proof that enforces respect of human rights within the ecosystem and that consists of the human actor being concious about the decisions that she is capable of making regarding something in particular. 
| EFF            | Electronic Frontier Foundation | 
| ToS            | Terms of Service | The ToS are a set of organized informations that describe in a detailed and understandable manner how a particular interaction that can be also called a service would work in the case that the same informations are accepted and agreed to function in a determined period.
| IoT            | Internet of Things | 
| IoH (IoTH)     | Internet of Humans | An IoT device that is installed in a human being with its consent and knowledge by their respective RPOHC, and PoK of the ToS, conditions and privacy policies.
| IoA (IoTA)     | Internet of Animals| An IoT device that is installed in an living being that is not human and that is not listed as a restricted IoA living being and that its oficially responsible Human has already provided consent and Proof of Knowledge of the Terms and Conditions and Privacy Policy of its Service.
| IoV (IoTVe)    | Internet of Vehicles | An IoT device that is Installed (kev:cinstall) in a Vehicle and that if other IoT devices are also installed in the same vehicle then it is the one that serves as the main controller or conciliator device for the proper communication of the vehicle with the Internet and that its Owner (KIAM), or Device Responsible Entity (KDRE) has already provided consent and Proof of Knowledge of the Terms and Conditions and Privacy Policy of its Service. For a vehicle to be considered as so for an installation and functioning of an IoV, it must be a device or artifact that complies with the laws, legislations, terms and conditions, privacy policies, corporate and civil agreements and human rights common sense considerations of the States in which it is pretended to be functioning.
| IoTv (IoTTv)   | Internet of Televisions | An IoT device that is embedded or is part or is a Television device and that the persons who are watching it while it is displaying content and connected to the Internet or Network at the same time is subject to the terms, conditions and privacy policies specially created for that matter and are not invasive nor violative of human rights.
| IoMD (IoTMD)   | Internet of Medical Devices | An IoT device that is embedded or installed in a LNCMD and that complies with all the regulations and MRQ previously needed to be a LKMD that works within the +LKNC$ ecosystem; and that by definition it must include a IoMD. All the LKMD must include a IoMD to be considered a LKMD.
| LNCMD (LNKMD)  | Lucky Network `KClassifiedCertified` Medical Device |The `LNCMD` (Lucky Network Certified and Classified Medical Device), also named `LNKMD` (Lucky Network K Medical Device) is a `K grade` certified secure device that processes, stores, transmits and receives `Medical Data`. The processing, storing, transmitting and receiving of medical data is also known in the +LKNC$ ecosystem as `"MedKData"`. All the `MedKData` must comply with the MRQ of the same, and must comply with `HIPAA`, `PCI` and the current `"most strict"` `"worldwide"` medical data handling regulations. The LNSCT and LNSCTVA will always work in efforts to bringing the highest standards of security to the `MedKData` `protocol`.
| MedKData       | `MedKData protocol` | CLASSIFIED TERM THAT CONSISTS OF A SECURE AND CLASSIFIED PROTOCOL OF DATA TRANSMISSION. 
| ToV            | Transfer of Value | CLASSIFIED TERM THAT CONSISTS OF TRANSMITING OR TX OR RX VALUE OR THE CLASSIFIED K ATOM.
| UoV            | Unit of Value | This is the most atomic unit of the +LKNC$ that can be used for Transfer of Value. The UoV can not be changed in an existing working $KLNC$ ecosystem. If a radical change like replacing the original UoV then a whole new +LKNC$ ecosystem would need to be enabled for the new UoV to start functioning, and the past +LKNC$ in which the old UoV used to live shall gradually and in an optimal way migrate to the new +LKNC$ through one or more LKNCTEs.
| EUoV           | External Unit of Value | An EUoV is any other currency or unitary value representation of ponderation which is different from the UoV of the +LKNC$ ecosystem but that can interact with the +LKNC$ through a LKNCTE. For example, if the UoV of the +LKNC$ "Zion" is "Euro", and a LKNCTE offers entrance to the +LKNC$ with "Sterlin Pounds", then the "Sterlin Pound" is considered as a EUoV while the "Euro" is considered as the UoV.
| CoToV          | Contract of Transfer of Value | CLASSIFIED TERM THAT CONSISTS OF A K CONTRACT OR SMART CONTRACT OR CONTRACT OR SET OF TERMS, CONDITIONS, PRIVACY POLICIES, ACCEPTATION AGREEMENT AND PROOF OF KNOWLEDGE OF AN AUTHORITATIVE AND SIGNED CLASSIFIED KLUCK SMART CONTRACT.
| ToToV          | Timestamp of Transfer of Value
| KSTATE         | The K State | All and every Device that interacts with the +LKNC$ weather it is enabled to transact or only to read, exists and is on one and only one of the States that are part of the set of States of he +LKNC$ Finite State Ecosystem.
| KFSES          | +LKNC$ Finite State Ecosystem State Set | The State Set of the +LKNC$ Sinite State Ecosystem includes all and every possible KSTATE that the Device can "be in". "Being in" a State is an abstract concept and in the case scenario of the $LKNC$ ecosystem only the Devices that are able to transact (the KIoT devices) can "be in" a State. All other Devices or devices that in a way interact with the +LKNC$ can be in a state and will be identified as so but they will not have the ability either to "be in" a State or to transact within the +LKNC$ ecosystem. Instead, those Devices or devices will be only able to read the +LKNC$ transactions and to interact in the Public +LKNC$ Pool that is fully separated from the ToV +LKNC$ ecosystem. The Devices or devices that are not able to "be in" a State, will be able to transact within the ToV +LKNC$ ecosystem only through a LKNCTE.
| LKNCTE         | +LKNC$ Certified Trusted Exchange | A LKNCTE allows non-SEU users to "interact" via a third party entity with the +LKNC$. The LKNCTE is totally independent from the +LKNC$ and all the interactions that ocurr between an LKNCTE and the +LKNC$ including the transactions are tied to the Terms, Conditions and Privacy Policies of such interactions and are limited and restricted to such said laws. The LKNCTEs can never be an instrument of gambling, money laundering, fraud, extorsion, war, terrorism, piracy, traffiking, speculation, ponzy schemes, pyramidal structures, microcontrolling nests, conspiracy, intellectual or industrial property violation, human rights violations or any other kind of damage. LKCTEs are highly monitored and need to comply all the time with strict protocols to warranty a healthy and secure way to enable foreign users to interact and enjoy the benefits of the +LKNC$ ecosystem in a symbiotic and harmonic way. The interactions between the +LKNC$ are based on respect.
| KIPC           | K Ingreso Per Capita | The K Ingreso Per Capita is the average amount +LKNC$ unitary values that every SEU receives every twenty four hours as exchange for the added value to the +LKNC$ economy. The K Ingreso Per Capita is very important not to be confused with the State or Country regular Ingreso Per Capita or Average Income Amount, because this value only applies for the SEUs that are also Value Adders into the +LKNC$. Other SEUs that are not Value Adders are not considered into this metric altought they are considered to receive the UBI.
| UBI            | Universal Basic Income | The UBI is the minimum amount of +LKNC$ unitary values preset at its minimum considered dimensional values that are warrantied to be transfered from the Single Initial Origin to the Secured End User of all the +LKNC$-enabled Network every twenty four hours.
| IoPP           | Internet of People | The Internet as a "whole", where the "whole" is a state in the context of the  "State Machine" of the implemented Internet technology. This Internet can also be a partial Internet or an Intranet or any other kind of Network in which the IoT and other Network-enabled devices like IoT, IoH, IoA, IoV and its subsets of its kind, and  that they work within at least one +LKNC$-enabled Network.
| MVV            | Minimum Viable "Victory", or "Successful Implementation with Ok ROI (SIOR)"
| MMV            | Minimim Mastered Vehicle | The "Minimum Mastered Vehicle" is the Qualified Product that can be put into production at a certain point in time to be part of the MVPP.
| MVPP           | Measured Verifiable Pilot Put (the original is a Mexican terminology that quotes "Medible Veritas Prueba Piloto" and means "Measurable Trustworthy Pilot Test").
| MVP            | Minimum Viable Product | 
| MRQ            | Minimum Required Qualifications | 
| CoVA           | Chain of Value Adders | 
| PoA		 | Proof of Asset |
| PoVAA          | Proof of Value Added to Asset | 
| IPoRA          | Iternational Proof of Reserve of Assets |
| PoAV           | Proof of Added value | 
| PoK            | Proof of Knowledge | 
| SIO            | Secured Initial Origin | 
| SEU            | Secured End User | 
| MRS		 | Minimum Required Stability (branches health and bug controls) |
| ROI            | Return of Investment | 
| COC            | Certificate Of Completion | 
| "common sense" | Common sense, or the common agreement of an Idea. |
| "Will"         | Common sense will where the common sense is relative to the context.
| "Product done. -signed." | Done, or an MVV with the proper achieved MRQs to obtain a COC. |
| "Product not done. -signed." | Not done, or an attempt of MVV without the proper achieved MRQs to obtain a COC. |
| "K Grade"      | Highest grade of certification of security | A "K" grade is commonly used in the +LKNC$ ecosystem to denote a "certification grade". There are cases where an extra level of security in the devices must be achieved, and usually those terms include the K grade or a "Certified" grade. In both cases, that certification is commonly talked or spoked as a "K" grade device or service.

## Vehicles
For a vehicle to be considered by the LNSCTC and LNSCTC for a possible MMV through 
one or more MVPs and a subsequent MVV for a MVPP product success, the IoV must have
the MRQ. A Vehicle is considered as any device that can transport something between
two physical locations either via air, ground, underground, on water or under water.
Vehicles, among other categories, fall into two main ones: 

* Transportation which includes mobility of humans or animals.
* Transportation which do not include mobility of humans or animals.

## Particular currencies and units of value

_The units of value shown here are just for demonstrative purposes until this message is removed._

```txt
* $MXN: Mexican Peso (Peso Mexicano)
        CoO:  ESTADOS_UNIDOS_MEXICANOS
        BoO:  BANCO_DE_MEXICO (TBD: $$INDEX.O$$)
        VoO:  1
        SoO:  MX, MXN, MEX, MEXICO, Mexico, México
        IPoRA_LKSOID: 
* $EUR  Euro (Euro)
        CoO:  EUROPE_UNION
        BoO:
        VoO:  1
        SoO:  
        IPoRA_LKSOID: 








* $USD  United States Dollar
        CoO:  UNITED_STATES_OF_AMERICA
        BoO:  THE_FEDERAL_RESERVE (TBD: $$INDEX.O$$)
        VoO:  1
        SoO:  USA, USS, EUA
        IPoRA_LKSOID:
```

## Details

### Oficial Unit of Value

This is a controversial term yet; but with "common sense" it then starts to make sense for the globalized economy and social ecosystems, which will empower their citizens in a fair manner, and add Value to their governments as well. The Currency Emissor Approved Assembly should enable full trust within all their participants.
In most of the countries which have gained enough international trust to consider them economically healthy, the most trusted entity to emit unitary particles of value is the so called Central Bank.

In the particular case of the +LKNC$ ecosystem, the entity which is the most trusted and the only one that has the authority, ability and need to emit unitary particles of value in the different dimensions of the same +LKNC$ ecosystem is the KUPE (K Unitary Particle Emissor).

In the particular case of the uncorrupted implementation of the +LKNC$ ecosystem in a dual (physical and digital) plane, any particle of value emitted by the KUPE could be used for unregulated or illegal activities by its native design. All other cases of such different uses of the particles of value would immediately self destruct the whole ecosystem and put immediate evidence and deanonymization of the participating entities, causing also immediate and imminent loss of all trust related to the attempt of the first MVV of the so called +LKNC$ ecosystem implementation.

For added security and risk reduction of the +LKNC$ ecosystem, by its same design and architecture, and by a correct implementation; any particle of value emitted by the KUPE could be used for unregulated or illegal activities and so the particular risk described before should not be a matter of concern.

### Vision
The vision of the +LKNC$ ecosystem is to be a healthy framework of transmission and storage of values and maintain it as pure as its core human original values.

### Mission

The Mission of the +LKNC$ ecosystem is to be and maintain it as pure and valuable as its original purity and valuation and demonstrate its core values and efforts as how empower every person to perform and live as desired as long as respecting other human beings in their same mission and to coexist with and bring other human beings that do not have or have lost an opportunity to continue enhancing their own lives to do so and to join and achieve the same state of the persons that are already enjoying those benefits.

### Core Human Original Values
```text
Love; 
Inclusion; 
Trust; 
Transparency;
Fairness;
Equality;
Freedom;
Wit;
```
## Key broad concepts

An "added value" is the value that is added to the "transfer of value".
The Added Value is a small bucket of valuable information that is added to the transaction and that lives with it as long as the micro warranty (or also understood as smart contract) is also alive.

An example of an Added Value could be a tax for that transaction that is intended to be put into a particular tax account. In MEXICO that added tax is called "Impuesto sobre el Valor Agregado" or "IVA", and its rate varies depending on the type of product or service that is being traded. The Added Value feature enables the +LKNC$ economy to keep a transparent signed accounting for each interaction.

The "transfer of value" implies always that the original value item or value representation will not exist anymore for the original value holder once that same value representation has being held by the entity that is acting as the receiver of the value representation. Any other attempt to transmit information or data that does not follow this pattern including all the sets of proof of work then the action itself  will be considered as a single copy in which the same arrange of data representing value could exist simultaneously in two places and it will be voided and its true value will not be considered as value within this protocol. So, within the transactionality of the +LKNC$ economy, all and any +LKNC$ value unit can only exist once in its atomicity and shall never exist as duplicate and shall never be cloned or multiply expended.

The investment is considered as a mix of money and time. For a ROI we consider the expected return for a particular injection and it does not mean that it is always the same output the injected substance what is expected as return. For your particular ROI and injection please contact our investment team so you can clarify all your questions before making a decision.

## Particular Groups
* LNSCTC:   Lucky Network Source Code Trust Commitee.
* LNSCTCVA: Lucky Network Source Code Trust Commitee Validation Association.

## Particular LKSO Terms and Abbreviations

```text
[ kev ]
k event.
The k event is an atomic and small action that occurs in time in a single event and can be put in time 
as an atomic and unique event.
A k event is mostly recorded or modeled for transactionality purposes of the ecosystem.

[ Éƒ$LKNC$ ]
ƒ atom.
The atomic ƒ is unique and atomic. It is classified yet its meta and source will be open.

[ +LKNC$ ]
+LKNC$ unit of value that is atomic.
The atomic unit of value of the ecosystem that is atomic and that its meta and source will be open.
```

## TBC. [To Be Continued]. WIP. Fin.
