# CivicClaw Demo Walkthrough

This document explains how to review the CivicClaw proof of concept.

## 1. Start with the incoming ticket

Open:

```text
data/incoming_ticket.txt
This file contains the new fictional incident report. It describes several school staff members being unable to access the School Learning Portal after password resets.

2. Review the historical incidents

Open:

data/incident_history.csv

This file contains fictional previous incidents. CivicClaw uses this information to identify similar patterns.

The most important matching examples are:

Previous incidents where multiple staff were affected
Incidents linked to password reset issues
Incidents previously resolved by the Identity team
Incidents previously treated as P2
3. Review the knowledge base

Open:

data/knowledge_base.md

This contains existing support guidance.

The demo intentionally includes only general password reset guidance. It does not include a strong article for multiple users being affected after password resets. This allows CivicClaw to identify a knowledge base gap.

4. Review the safety policy

Open:

data/security_policy.md

This file defines what the assistant can safely do, what needs human approval and what must be blocked.

This is an important part of the project because CivicClaw is designed for public-sector IT environments where data protection, approval and auditability matter.

5. Review the agent prompt

Open:

prompts/agent_prompt.md

This prompt tells the AI assistant how to behave, what files to read and what outputs to create.

It also tells the assistant not to use real data, not to send messages externally and not to pretend that live systems were changed.

6. Review the generated outputs

Open the files in:

outputs/

The output pack includes:

File	What it shows
incident_summary.md	The recommended category, priority and next action
evidence_pack.md	Why the assistant recommended P2
user_update.md	A plain-English update for affected users
resolver_notes.md	Technical notes for the IT resolver team
post_incident_report.md	A draft post-incident report
kb_gap_analysis.md	Missing knowledge base guidance and a draft article
risk_audit_log.json	Safe actions, approval-required actions and blocked actions
7. Key idea

CivicClaw is not designed to replace IT analysts.

It is designed to support them by preparing structured, safe and evidence-based incident response materials.

The human remains responsible for approving live actions such as sending updates, changing incident priority, escalating to another team or publishing knowledge base content.

8. Main value

CivicClaw demonstrates how an AI agent could help with:

faster incident triage
better duplicate detection
clearer user communication
safer AI-assisted workflows
knowledge base improvement
auditability and human approval
9. Demo limitation

This is a proof of concept using fictional local files.

It does not connect to live ITSM systems, real council systems or real user data.