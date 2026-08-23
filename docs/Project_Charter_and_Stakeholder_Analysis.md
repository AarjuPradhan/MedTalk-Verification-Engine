# Project Overview

Title: Clinical Note Accuracy & Verification Engine

Partner: FAZ Australia

Team members: Aarju Pradhan, Hassan Mohammad, Muhammad Daud Shafique, Avash Gharti Magar

Project Supervisor: Assoc. Prof. John Ayoade 

Date: 23 August 2026

# Project background
FAZ Australia is a health technology company based in Canberra, Australia. The primary product of the organization, which is Medtalk acts as an artificial intelligence (AI) medical scribe that automatically generates structured clinical notes by processing audio from doctor’s consultations. This will reduce administrative burdens but AI generated content is bound to have some critical errors such as hallucination (fabricating details), omissions (leaving out crucial information) or contradictions (recording incorrect facts). In order to make sure clinical safety and practitioner trust are achieved, the company requires an automated verification engine that compares the AI generated note against the original transcript before final physician approval which aligns with standard IT project risk mitigation strategies (Skulmoski, 2022).

# Project Objectives
- Design a verification engine capable of automatically comparing an AI generated clinical note against the original consultation transcript.
- Develop a system that flags discrepancies (omissions, contradictions and hallucinations) and assign a rating to each identified issue.
- Formulate a testing plan using synthetic conversation transcripts and notes which data has some deliberate errors to evaluate the engine capabilities.

# Scope
In Scope
- Development of a verification engine prototype and a reporting dashboard/interface.
- Utilization of fake consultation transcripts and AI generated notes for all testing and validation processes.
- Implementation of scoring system to identify match, omission, contradiction or unsupported statement.

Out of Scope
- Connecting the verification engine prototype with the live MedTalk system or real patient database.
- Implementing automatic correction of the generated clinical notes as the system is strictly limited to flagging identified issues.
- Any form of clinical decision making or assessment of clinical correctness beyond text comparison.

| Stakeholder | Role | Interest | Influence |
| :--- | :--- | :--- | :--- |
| FAZ Australia (Atif Nisar) | Client | High | High |
| Medical Practitioners | End Users | High | Medium |
| Assoc. Prof. John Ayoade | Project Supervisor | High | High |
| Project Team | Development Team | High | High |

# Success criteria
- The verification engine successfully runs synthetic transcript and note pairs from end-to-end.
- The system accurately identifies and classified planted errors with appropriate severity ratings.
- A functional report or dashboard clearly displays the total number of flagged issues into category and their severity.
