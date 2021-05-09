# :mortar_board: AUTOMATION SERVICE CHOREOGRAPHY

[:rewind:back](../README.md)

Editing Status: :heavy_check_mark: (discussed + published)

Last Modification: 09.05.2021

---

## :zero: Motivation

### Introduction

My motivation is primarily to develop pragmatic solutions for practice using scientific methods. However, this alone is not enough for a doctorate. The last 15 years, in which I have already been working in the field of process control engineering, have shown me that the process industry is facing increasing change. The pressure on companies in the process industry to become more efficient and faster in the development and production of new products is continuously increasing [1]. This development of the market endangers the profitability of the manufacturing industry in the future.

### Chronology

In order to work against this trend at an early stage, a first eu-funded project was launched in 2009 with the F3 Factory Project, which focused on the development of more efficient processes in the chemical industry. F3 is an acronym for "Flexible, Fast and Future Factory". The focus of this project was the investigation and development of a new production technology according to a modular plug and play approach [2]. The knowledge gained in this project with regard to the automation of such a plug and play capable production plant ultimately resulted in a Namur Recommendation NE148, which was published in 2013 [3]. Already in 2014, a consortium consisting of the company Wago and the two universities TU Dresden and Helmut-Schmidt-University Hamburg presented a first approach for the implementation of such a plug and play mechanism for industrial process plants [4]. After a successful presentation of the concept at the 77th Namur Main Meeting in 2014, the concept was handed over into the joint hands of NAMUR and ZVEI. Under the joint governing body of both organizations, a landscape of several task forces was created that has been developing the VDI/VDE/NAMUR 2658 [5] series of standards for many years in collaboration with the VDI/VDE-GMA Technical Committee 5.16 (Future Architectures of Automation). The modular production community has grown steadily in recent years [6]. The standard series defines runtime interfaces and semantic models for the implementation of plug and play capable production modules for the modular process industry.


The origin of my research originates from the work and participation in this community of modular production in the context of the standard series [5]. In the next section there is a short presentation of this and a second guideline in the environment of modular process plants as well as the motivation derived from it.

### Standardization

For standardization in the field of modular production, reference can currently be made to two series of standards - the VDI 2776 [7] standard specifies the process engineering part of a modular production plant, while the VDI/VDE/NAMUR 2658 standard defines the automation engineering principles in a manufacturer-neutral manner. VDI 5201 [8] is also mentioned at this point. This guideline introduces the two terms flexibility and adaptability. Both terms are relevant for my further work.


Part 4 of the standard series VDI/VDE/NAMUR 2658 [5] specifies a generic service concept based on a state-based and a continuous interface. The state-based interface "ServiceControl" [9] is used for procedural coordination from the higher-level system. The continuous interface is formed by the two interfaces of the "Process Value Output" and the "Process Value Input". Both interfaces exist for binary (BOOL), integer (DINT) and fractional numbers (REAL) as well as character strings (STRING). The higher-level system, called the Process Orchestration Layer, is the central coordination system and has the task of implementing both the procedural coordination and the data exchange for the continuous process value interconnection.

The standard series VDI 2776 [7] specifies a kind of physical model of a modular plant, in analogy to IEC 61512 [10]. The following four levels are specified from top to bottom - Modular Plant (MP), Process Equipment Assembly (PEA), Functional Equipment Assembly (FEA), Component (COMP). The adaptability of a modular production plant depends primarily on the possibilities of forming the actual plant from the three lower levels of the model.

In the next section, four practical use cases are described with regard to the adaptability of modular plants. The aim of these use cases is to make the aspect of the adaptability of a modular plant more concrete.

## :hash: References

No. | Publication
--- | ---
1 | Small-Scale Flexible Plants - Towards a More Agile and Competitive EU Chemical Industry; v. Kranenburg, Sofra, Verdoes, de Graaff; 2015; [Link](https://repository.tudelft.nl/view/tno/uuid%3A492dadff-af9d-4059-a41e-2b77270197b2)
2 | Chemieanlage der Zukunft: das F3 Factory-Project; Liebl; 2010; [Link](https://www.chemietechnik.de/anlagenbau/chemieanlage-der-zukunft-das-f3-factory-projekt.html)
3 | Namur Recommendation NE148 - Automation Requirements relating to Modularisation of Process Plants; NAMUR; 2013; [Link](https://www.namur.net/de/empfehlungen-und-arbeitsblaetter/aktuelle-nena.html?no_cache=1&tx_nena_pi1%5Bda%5D=377&cHash=9de1d4ebf7033ec8090a9a28b26334c1)
4 | Referenz - Mit DIMA zur Smarten Produktion; WAGO; 2020; [Link](https://www.wago.com/de/digitalisierung/wandlungsfaehigkeit/dima)
5 | Richlinien-Reihe VDI/VDE/NAMUR 2658 - Automation engineering of modular systems in the process industry; Beuth Verlag; [Link](www.vdi.de/2658)
6 | Sonderschau Modulare Produktion auf der HMO 2019 - Modularisierung erhöht Flexibilität von Prozessanlagen erheblich; ZVEI; 2019; [Link](https://www.zvei.org/presse-medien/pressebereich/sonderschau-modulare-produktion-auf-der-hannover-messe-2019-modularisierung-erhoeht-flexibilitaet-von-prozessanlagen-erheblich/)
7 | Richtlinien-Reihe VDI 2776 - Process engineering plants - Modular plants; Beuth Verlag; [Link](www.vdi.de/2776)
8 | Richtlinie VDI 5201 - Adaptability - Description and measurement of the adaptability of manufacturing companies: Beuth Verlag; [Link](www.vdi.de/5201)
9 | Bloch H.., Hensel S., Hoernicke M., Katharina S., Menschner A., Fay A., Urbas L., Knohl T., Bernhausen J., (2018), State-based control of process services within modular process plants, 51st CIRP Conference on Manufacturing Systems, 1088-1093, [Link]()
10 | IEC 61512 //TODO