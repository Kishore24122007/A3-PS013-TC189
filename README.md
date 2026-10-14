# CyberTrace — Digital Forensics Timeline Analyzer

**AIORI-3 Hackathon | Problem Statement PS-013**

**Team Name:** Team Ignite  
**Team Code:** `A3-PS013-TC189`  
**Institution:** Karunya Institute of Technology & Science

---

## 1. Project Overview

CyberTrace is a proposed Python-based digital forensic timeline analysis tool designed to help small investigation teams analyze cybersecurity incidents, organize digital evidence, and understand incident timelines more clearly.

When a cybersecurity incident occurs, investigators need to understand what happened, when it happened, and how different events are connected. However, relevant information is often scattered across different log files, computer systems, and evidence sources.

CyberTrace aims to simplify this process by organizing digital evidence, processing supported log files, arranging events chronologically, and helping investigators analyze the sequence of events during a cybersecurity incident.

Our goal is to make digital forensic investigations simpler, faster, more organized, and more reliable for small investigation teams.

## 2. Problem Statement

**PS-013: Incident Timeline and Evidence Collection for Small Teams**

Small investigation teams face several challenges when investigating cybersecurity incidents:

- **Scattered evidence:** Information is distributed across different log files, computer systems, and evidence sources.
- **Manual analysis:** Collecting and analyzing information manually can be time-consuming and confusing.
- **Timestamp inconsistencies:** Different systems may use different timestamp formats and time zones, making it difficult to determine the correct sequence of events.
- **Evidence integrity:** Investigators need to ensure that collected evidence has not been accidentally modified.
- **Missed events:** Manual analysis may overlook important events, making it difficult to reconstruct an incident accurately.
- **Difficult event correlation:** Understanding how events from different sources are connected can be challenging.

These challenges highlight the need for a simple and organized approach to digital forensic investigation.

## 3. Proposed Solution

CyberTrace aims to provide a structured workflow for collecting, organizing, and analyzing digital evidence.

The proposed tool will process supported log files, arrange important events in chronological order, and help investigators understand the sequence of events during a cybersecurity incident.

It aims to use SHA-256 hashing to verify evidence integrity, normalize timestamps into a consistent format, correlate events from different sources, and generate structured investigation reports.

By bringing these capabilities into one workflow, CyberTrace aims to reduce manual effort and improve the clarity, transparency, and reliability of digital forensic investigations.

## 4. Key Features

The following features are proposed for CyberTrace:

### 4.1 Digital Evidence Organization
Organize collected digital evidence and relevant information from supported sources to make investigation workflows easier to manage.

### 4.2 Log File Processing
Process supported log files to extract important events and information for further analysis.

### 4.3 Evidence Integrity Verification
Use SHA-256 hashing to help detect changes to collected evidence and support integrity verification.

### 4.4 Timestamp Normalization
Standardize timestamps into a consistent format to make chronological analysis easier. Timestamp information should be handled carefully when time zones or offsets are unknown.

### 4.5 Incident Timeline Reconstruction
Arrange important events in chronological order to help investigators understand the sequence of activities during a cybersecurity incident.

### 4.6 Cross-Source Event Correlation
Help investigators identify potentially related events from different sources and understand how those events may be connected.

### 4.7 Investigation Report Generation
Generate structured investigation reports containing relevant events, evidence details, and analysis results.

## 5. Proposed Workflow

CyberTrace is designed around the following workflow:

1. **Collect:** Gather relevant digital evidence and supported log files from authorized sources.
2. **Preserve:** Maintain original evidence and calculate SHA-256 hashes for integrity verification.
3. **Process:** Parse supported log files and extract important event information.
4. **Normalize:** Standardize timestamps where sufficient time-zone information is available.
5. **Correlate:** Identify potentially related events across different sources.
6. **Analyze:** Arrange events chronologically to reconstruct the incident timeline.
7. **Report:** Generate structured reports containing relevant events, evidence details, and analysis results.

## 6. Proposed System Architecture

The planned CyberTrace architecture consists of the following logical components:

- **Evidence Sources:** Supported log files and authorized systems.
- **Evidence Collection:** Collects relevant logs and evidence metadata.
- **Evidence Integrity:** Uses SHA-256 hashing to support verification of collected files.
- **Log Processing:** Parses supported records and extracts relevant events.
- **Timestamp Processing:** Normalizes timestamps where possible.
- **Correlation Engine:** Identifies potentially related events across sources.
- **Timeline Analyzer:** Organizes events chronologically for investigation.
- **Reporting Component:** Produces structured investigation reports.

These components describe the proposed design. The final architecture will depend on the implementation.

## 7. Proposed Technology Stack

| Component | Technology / Approach |
|---|---|
| Programming Language | Python |
| Log Processing | Python-based processing and log analysis |
| Evidence Integrity | SHA-256 hashing |
| Timestamp Handling | Timestamp normalization |
| Event Analysis | Chronological timeline reconstruction |
| Event Correlation | Cross-source event correlation |
| Reporting | Structured investigation reports |

Additional technologies may be incorporated as development progresses. Only technologies actually integrated should be described as implemented.

## 8. Expected Benefits

CyberTrace aims to provide the following benefits:

- Reduce manual effort during digital forensic investigations.
- Organize digital evidence in a structured manner.
- Make incident timelines easier to understand.
- Help investigators identify connections between events from different sources.
- Support evidence integrity verification.
- Improve the consistency of timestamp handling.
- Generate structured reports for investigation and documentation.
- Make digital forensic workflows more accessible to small investigation teams.

## 9. Scope and Limitations

The proposed scope focuses on helping small investigation teams process supported logs, organize evidence, reconstruct incident timelines, and generate reports.

The accuracy and usefulness of the results will depend on the quality of the available evidence, supported log formats, timestamp information, and implemented correlation methods.

SHA-256 hashing can help detect changes to a file after its hash has been recorded. It does not, by itself, establish the authenticity of the evidence before collection.

CyberTrace is intended to support forensic analysis and does not replace professional investigative procedures or comprehensive security monitoring platforms.

## 10. Evaluation Plan

The planned evaluation will examine whether CyberTrace can process supported logs and reconstruct incident timelines reliably.

Potential evaluation activities include:

- Testing log processing with sample datasets.
- Checking whether timestamp normalization produces expected results.
- Verifying whether deliberate file modifications are detected through hash comparisons.
- Assessing the accuracy of reconstructed timelines against known test events.
- Examining whether related events can be correlated across supported sources.
- Reviewing the completeness and clarity of generated reports.

Evaluation results will be documented after the relevant functionality has been implemented and tested.

## 11. Project Presentation

The presentation for the AIORI-3 Hackathon is available here:

**[View CyberTrace Hackathon Presentation](./CyberTrace-Hackathon-Presentation.pdf)**

The presentation explains the problem statement, proposed solution, existing challenges, planned features, system architecture, workflow, evaluation plan, and references.

## 12. Team Introduction Video

Our team introduction video presents our understanding of the problem statement, the challenges faced by small investigation teams, and our proposed solution.

The video also introduces our team members and their contributions to CyberTrace.

**YouTube Video:** [[Video Link](https://youtu.be/WXXLueNYNnc?si=X8q-Do0OOJeo-DgF)]

## 13. Team Members

**Team Name:** Team Ignite  
**Team Code:** `A3-PS013-TC189`

| S. No. | Team Member | Contribution |
| 1 | Kishore Parasuraman | Technical development, Python-based processing, log analysis, timestamp normalization, and evidence integrity verification. |
| 2 | Jabez Gabrilraj | Contributing to the development of CyberTrace. |

Both team members aim to build a practical and reliable solution for digital forensic investigations.

## 14. Development Status

CyberTrace is being proposed and developed as part of the AIORI-3 Hackathon.

The repository will contain the project's source code, documentation, presentation, and other relevant resources as development progresses.

Planned features will be updated to reflect actual implementation and testing results.

## 15. References

1. **NIST SP 800-86:** Guide to Integrating Forensic Techniques into Incident Response.  
   https://csrc.nist.gov/pubs/sp/800/86/final

2. **OWASP Logging Cheat Sheet:** Guidance on security logging and log protection.  
   https://cheatsheetseries.owasp.org/cheatsheets/Logging_Cheat_Sheet.html

3. **Wazuh Documentation:**  
   https://documentation.wazuh.com/

4. **Velociraptor Documentation:**  
   https://docs.velociraptor.app/

5. **Timesketch:**  
   https://timesketch.org/

6. **Plaso (log2timeline) Documentation:**  
   https://plaso.readthedocs.io/

---

**AIORI-3 Hackathon | Team Ignite | PS-013 | CyberTrace**

*From Scattered Logs to an Evidence-Backed Incident Timeline.*
