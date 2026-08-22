# Zenith Computer Agent — Founding Specification

**Planned repository:** `ZachPoli/zenith-computer-agent`  
**Status:** Incubating — not an active full development project until FamiliarVoice reaches its release/monetization gate.

## Founding Question

Can Zenith make a computer operable primarily through natural intent, so a user can say what they want accomplished without having to visually navigate every menu, button, window, and application?

## Product Thesis

> **A conversational computer agent that understands the user's screen and applications, carries out bounded tasks, asks for confirmation when appropriate, and clearly reports what happened.**

The accessibility origin is important: traditional screen/mouse/keyboard interfaces can create severe barriers for blind, low-vision, motor-impaired, or otherwise access-limited users.

The broader opportunity is universal. The same interface could save time for anyone doing repetitive digital work or trying to operate a computer hands-free.

## Example Experience

A user should eventually be able to say:

- "Open my email and find the message about tomorrow's appointment."
- "Read it to me."
- "Draft a reply saying I'll be there at ten, but don't send it yet."
- "Find the invoice John sent last week and put the total in this spreadsheet."
- "Open my calendar and tell me what I have Friday afternoon."
- "Why won't this setting work? Show me where to change it."

The product should translate **intent -> observable computer actions** while keeping the user in control.

## Product Boundary

The goal is not to build a new operating-system kernel.

"AI-operated computer OS" is the long-term experience vision: an AI interaction layer that sits above existing operating systems and applications and lets the user control them conversationally.

The first product should therefore behave more like an **AI accessibility/automation shell or agent layer** than a replacement for Windows/macOS/Linux.

## Prototype Architecture Hypothesis

```text
User voice / text intent
        |
        v
Conversation + task planner
        |
        +----> Screen / UI state understanding
        |
        +----> Approved computer tools/actions
        |
        v
Action executor
        |
        +----> verification / recovery
        |
        v
Spoken + visual status to user
```

Potential implementation components may eventually include:

- screen capture / UI understanding;
- accessibility APIs where available;
- operating-system automation interfaces;
- browser automation;
- application-specific connectors;
- file/email/calendar tools;
- voice interface;
- action confirmation and audit trail.

## First Prototype Goal

Prove a small, safe workflow before attempting general computer control.

Example first prototype:

1. user asks the agent to inspect a simple desktop/browser state;
2. agent explains what is visible;
3. user asks it to perform one bounded action;
4. agent shows or states the intended action;
5. user confirms if the action is consequential;
6. agent performs the action;
7. agent verifies the result and reports success/failure.

## Accessibility Requirements

From the beginning:

- voice-first operation where practical;
- full status available without relying on visual-only feedback;
- keyboard-accessible fallback controls;
- minimal precision mouse interaction required;
- clear focus/application context;
- repeatable spoken summaries of current state;
- predictable confirmation behavior;
- easy cancel/stop command;
- recovery path when the agent gets confused.

## Trust and Safety Requirements

Computer control creates a large trust surface.

Early architecture should distinguish between:

### Low-risk actions
- open/read/search;
- navigate;
- summarize;
- draft without sending;
- copy information.

### Consequential actions
- send messages;
- submit forms;
- make purchases;
- delete files;
- change security/account settings;
- install software;
- financial actions.

Consequential actions should generally require explicit confirmation and should be logged clearly.

The agent should never hide uncertainty or falsely claim an action succeeded.

## Privacy and Security

A product that can see and operate a computer may encounter extremely sensitive information.

Requirements will include:

- least-privilege access;
- explicit permission boundaries;
- clear indicators of what the agent can access;
- secure credential handling;
- no unnecessary capture/storage of screen content;
- auditability of actions;
- safe handling of untrusted on-screen content and prompt-injection attempts.

## Commercial Possibilities

Potential future models:

- consumer subscription;
- accessibility-focused plan;
- productivity/pro tier;
- business/enterprise licensing;
- managed accessibility deployments;
- application-specific connectors/integrations;
- API/SDK licensing.

## Non-Goals for the Founding Stage

- replacing Windows/macOS/Linux;
- unrestricted autonomous computer control;
- financial automation without strong safeguards;
- supporting every application immediately;
- building a general enterprise RPA suite;
- replacing FamiliarVoice as the current flagship.

## Activation Gate

This repository becomes an active Zenith engineering project only after an explicit company decision following FamiliarVoice's release/monetization milestone.

Until then, allowed work is limited to:

- product notes;
- accessibility workflow research;
- architecture/security research;
- small feasibility experiments;
- identifying high-value first workflows;
- interviews/observations that clarify real user barriers.

## Long-Term Role in Zenith

Zenith Computer Agent represents the **Act** layer of the company thesis:

> **Perceive -> Understand -> Act**

The long-term ambition is a computer experience where users can express intent naturally and technology handles more of the interface burden while preserving human control.
