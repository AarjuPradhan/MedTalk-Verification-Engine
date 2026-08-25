# Feasibility Study 

This part analyzes the technical, economic, and legal feasibility of creating the Clinical Note Accuracy & Verification Engine prototype.  

**1.1 Technical Feasibility**

In terms of software architecture, a system solely based on rules is insufficient since it cannot process implicit clinical context or terms that mean the same thing. Hence, it is quite feasible and necessary to create a hybrid pipeline. "Conventionally, regular programming (regex) is suitable for dealing with strict constraints (for example, lab values), whereas language technologies devise an assessment of semantic discrepancies." The latest publication by Ben Abacha et al. elaborates on the incapability of traditional evaluation method towards the automated generation of medical notes, proving this is a compelling reason for the need for a smart hybrid verification system from technical point of view.  

**1.2 Economic Feasibility** 

The MedTalk platform enhances the efficiency of the clinic by significantly decreasing time spent on administration. On the other hand, mistakes made by AI may result in serious financial losses and a loss of reputation. The economic efficiency of developing a safety measure is justified, since it minimizes and limits the manual verification carried out by doctors. 

**1.3 Legal Feasibility**

In order to comply with laws on data privacy (like the Australian Privacy Act), the scope of the project narrows the nature of the verification engine so that it does not connect to the actual MedTalk system and to the real patient databases in order to ensure that all development and testing takes place exclusively on synthetic conversations, thus eliminating all legal risks associated with patient confidentiality. 

# Risk Register 

Below we describe the main risks related to the use of the AI verification engine and the corresponding mitigation strategies designed to provide reliable operation of the system. 

**Risk 1**: Alert fatigue (false positives). The notifications about every little discrepancy in conversation will lead to alert fatigue on the part of the clinicians. Mitigation: The engineers will develop a scoring system with three levels of severity of alerts: critical, high, and medium. 

**Risk 2**: AI hallucinations and misses (false negatives). Language models are often known to produce erroneous facts, and this makes it difficult for safe implementation of clinical software. In case the system fails to pick up the erroneous diagnosis, lives might be at risk. Mitigation: The evaluation system will be oriented to ensure maximum recall in quantitatively severe cases. 

**Risk 3**: Entrapment of Synthetic Dataset Bias. It is possible that verification mechanisms could become anchored to a limited number of synthetic datasets, failing to hold when confronting challenging real-world cases.  

**Mitigation**: The group will conduct extensive peer review of all pairs of tested instances in order to include varied situations in the test collection.  

# Cybersecurity Evaluation  

Positioning itself within the realm of standard IT project risk mitigation techniques, the cybersecurity aspect in regard to the prototype presupposes total isolation of the setup, as well as the employment of fundamental threat models.  

System Isolation: The prototype will be completely ‘sandboxed’. Since it processes only synthetic data and is not connected to the working environment, the possibility of infiltration of medical data will be avoided.  

Threat Modeling and Vulnerability Analysis: The prototype for the reporting dashboard will feature principles of traditional software security practices, including secure configuration and preventing leakage of any cleartext information during processing.  

AI-Specific Risks: The machine itself acts as a safeguard against cybersecurity problems, functioning as means of securing the integrity of information. It detects misleading statements and incorrect information, acting as an automated verifier of the accuracy of outputs of the LLM. 

