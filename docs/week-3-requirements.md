# Week 3 – Requirements Elicitation

## MedTalk Clinical Note Accuracy & Verification Engine

**Role:** Requirements Lead  
**Jira:** MVE-3, MVE-12, MVE-13

## 1. Introduction

The MedTalk Clinical Note Accuracy and Verification Engine is designed to support the review of AI-generated clinical notes by comparing them with the original consultation transcript. The purpose of the requirements elicitation process is to identify what clinicians and other stakeholders need from the verification system before detailed design and implementation begin.

The system is expected to identify important differences between a consultation transcript and an AI-generated clinical note, including missing information, contradictions, and unsupported information. Particular attention is required for clinically important information such as medications, dosages, diagnoses, numerical values, and timelines.

## 2. Elicitation Methods Used

To understand the requirements of the MedTalk Verification Engine, two main elicitation methods were used: document review and observation. These methods helped identify the current clinical documentation problem, stakeholder needs, and the expected behaviour of the proposed verification system.

### 2.1 Document Review

The existing MedTalk project brief and available project documentation were reviewed to understand the purpose and scope of the system. The review identified the need to compare AI-generated clinical notes with consultation transcripts and detect possible omissions, contradictions, unsupported information, and errors in important clinical details.

The document review also helped identify important verification areas such as medications, dosages, diagnoses, numerical values, and timelines.

### 2.2 Observation

Observation was used to understand the general workflow of clinical note verification. The workflow was considered from the point where a consultation transcript and an AI-generated clinical note are provided to the system through to the point where detected differences are presented for clinician review.

## 3. Stakeholder Identification

The main stakeholders for the MedTalk Verification Engine were identified based on their involvement in creating, reviewing, managing, or protecting clinical information.

### 3.1 Clinicians

Clinicians are the primary users of the verification engine. They need the system to clearly identify possible errors, omissions, contradictions, and unsupported information in AI-generated clinical notes so they can review the results before relying on the notes.

### 3.2 Healthcare Organisation

The healthcare organisation needs the system to support accurate and reliable clinical documentation. The organisation also requires the system to reduce risks associated with incorrect AI-generated clinical information.

### 3.3 System Administrators

System administrators are responsible for maintaining and managing the verification system. They require appropriate system access, security controls, monitoring, and reliable system operation.

### 3.4 Patients

Patients are indirect stakeholders because their consultation information is processed by the system. Their clinical information must be handled securely and their privacy must be protected.

### 3.5 Development and Security Team

The development and security team is responsible for implementing, testing, and maintaining the verification engine. They need clearly documented requirements so that the system can be developed and tested against the expected functionality.

## 4. Stakeholder Requirements

Based on the elicitation activities and stakeholder identification, the following stakeholder requirements were identified for the MedTalk Verification Engine.

### 4.1 Clinician Requirements

- SR-01: Clinicians need to provide a consultation transcript and an AI-generated clinical note for verification.
- SR-02: Clinicians need the system to identify missing information in AI-generated clinical notes.
- SR-03: Clinicians need the system to identify contradictions between the transcript and the generated clinical note.
- SR-04: Clinicians need the system to identify unsupported or potentially incorrect information.
- SR-05: Clinicians need verification results to be presented clearly so that detected issues can be reviewed efficiently.

### 4.2 Healthcare Organisation Requirements

- SR-06: The organisation needs the system to support accurate and reliable clinical documentation.
- SR-07: The organisation needs the system to reduce the risk associated with inaccurate AI-generated clinical notes.
- SR-08: The system should support a consistent clinical note verification process.

### 4.3 System Administrator Requirements

- SR-09: Administrators need appropriate access controls to manage the verification system.
- SR-10: Administrators need the ability to monitor the operation of the system.
- SR-11: The system needs to provide appropriate logging to support monitoring and troubleshooting.

### 4.4 Patient and Privacy Requirements

- SR-12: Patient information must be protected from unauthorised access.
- SR-13: Clinical information must be handled securely during the verification process.
- SR-14: The system should only process information required to perform clinical note verification.

### 4.5 Development and Security Requirements

- SR-15: The development team needs clearly defined requirements that can be implemented and tested.
- SR-16: The system must support testing of different verification scenarios, including omissions, contradictions, and unsupported information.
- SR-17: Security controls must be considered throughout the design and development of the verification engine.

## 5. Initial Functional Requirements (MVE-13)

The following functional requirements describe the main functions that the MedTalk Verification Engine should provide.

- FR-01: The system shall allow a consultation transcript to be provided for verification.
- FR-02: The system shall allow an AI-generated clinical note to be provided for comparison.
- FR-03: The system shall compare the AI-generated clinical note with the consultation transcript.
- FR-04: The system shall identify information that is present in the transcript but missing from the clinical note.
- FR-05: The system shall identify contradictions between the transcript and the clinical note.
- FR-06: The system shall identify information in the clinical note that is not supported by the consultation transcript.
- FR-07: The system shall check important clinical information such as medications, dosages, diagnoses, numerical values, and timelines.
- FR-08: The system shall present detected issues clearly for clinician review.
- FR-09: The system shall classify or prioritise detected issues according to their importance.
- FR-10: The system shall record appropriate verification activity for monitoring and troubleshooting.

## 6. Initial Non-Functional Requirements (MVE-13)

The following non-functional requirements describe the expected quality, security, performance, and usability characteristics of the MedTalk Verification Engine.

### 6.1 Security and Privacy

- NFR-01: The system shall protect clinical and patient information from unauthorised access.
- NFR-02: The system shall use appropriate access controls for authorised users.
- NFR-03: Sensitive clinical information shall be handled securely during processing and storage.
- NFR-04: The system shall maintain appropriate logs for security monitoring and auditing.

### 6.2 Performance

- NFR-05: The system should complete clinical note verification within a reasonable response time.
- NFR-06: The system should remain responsive while processing supported clinical notes and transcripts.

### 6.3 Reliability

- NFR-07: The system should provide consistent verification results for the same input.
- NFR-08: The system should handle invalid or incomplete input without unexpected system failure.

### 6.4 Usability

- NFR-09: Verification results should be clear and understandable for clinicians.
- NFR-10: Detected issues should be presented in a way that allows clinicians to identify important problems efficiently.

### 6.5 Maintainability

- NFR-11: The system should be designed in a modular manner to support future maintenance and improvement.
- NFR-12: System components and requirements should be documented clearly to support future development and testing.

## 7. Assumptions and Constraints

### 7.1 Assumptions

- The consultation transcript provided to the system is accurate and complete.
- The AI-generated clinical note is available in a format that can be processed by the verification engine.
- Authorised clinicians and administrators will use the system appropriately.
- The verification engine will support clinicians in reviewing notes rather than replacing clinical judgement.

### 7.2 Constraints

- The system must protect sensitive clinical and patient information.
- The accuracy of verification may depend on the quality and completeness of the provided transcript and clinical note.
- The system must operate within the technical resources available to the project.
- Development must follow the agreed project scope and assessment timeline.

## 8. Conclusion

The requirements elicitation process identified the main stakeholders and their needs for the MedTalk Verification Engine. Document review and observation were used to understand the proposed verification workflow and expected system behaviour.

The identified stakeholder, functional, and non-functional requirements provide an initial foundation for the design and development of the system. These requirements will also support later system specification, implementation, security assessment, and testing activities.
This helped identify the need for clear verification results and appropriate prioritisation of important clinical errors while avoiding unnecessary alerts.

