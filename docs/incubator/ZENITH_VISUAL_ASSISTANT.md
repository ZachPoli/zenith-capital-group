# Zenith Visual Assistant — Founding Specification

**Planned repository:** `ZachPoli/zenith-visual-assistant`  
**Working prototype codename:** Jarvis  
**Status:** Incubating — not an active full development project until FamiliarVoice reaches its release/monetization gate.

## Founding Question

Can Zenith make visual context feel like a natural part of an ongoing AI conversation so a person can simply ask for help with what they are seeing?

## Product Thesis

> **A conversational visual assistant that can understand camera or screen context while the user talks naturally, then describe, explain, locate, guide, or assist without forcing the user through a stop-and-upload workflow.**

The accessibility use case is foundational: help blind and low-vision users access more information about the physical and digital world.

The broader opportunity is universal: hands-free help, gaming assistance, repair/troubleshooting, cooking, shopping, travel, learning, object identification, screen understanding, and other situations where showing is easier than explaining.

## Core Experience

A user should eventually be able to say things such as:

- "What is in front of me?"
- "Where is the door handle?"
- "Read that sign."
- "Help me find my keys."
- "Which button should I press?"
- "What am I doing wrong in this game puzzle?"
- "Tell me when I point the camera at the right part."

The interaction should feel continuous and conversational rather than like repeatedly submitting photos.

## Prototype Architecture Hypothesis

Initial architecture should favor existing model/platform capabilities rather than building vision models from scratch.

```text
Camera / Screen Capture
        |
        v
Context Sampler
(frame selection / scene change / user-triggered capture)
        |
        +-----------> AI vision context
        |
Microphone ----------> Realtime conversation layer
        |
        v
Assistant reasoning / response
        |
        v
Spoken guidance
```

The prototype may simulate continuous visual understanding through intelligent frame sampling rather than requiring raw video-model input.

## First Prototype Goal

The first serious prototype should prove one low-risk loop:

1. user starts a live camera or screen session;
2. user speaks naturally;
3. application sends current visual context when useful;
4. assistant answers based on what is actually visible;
5. conversation continues without the user manually attaching images each turn.

A gaming/screen-capture mode is a useful low-risk test environment before relying on the product for real-world mobility or safety-critical guidance.

## Accessibility Requirements

From the beginning:

- voice-first operation where practical;
- important state communicated audibly, not only visually;
- minimal precision tapping required;
- clear uncertainty language;
- easy repeat/re-describe command;
- privacy indicator when camera/context is being shared;
- user controls when visual data is captured or transmitted;
- do not imply safety-critical reliability that has not been demonstrated.

## Safety Boundary

Early versions are **assistive context tools**, not autonomous mobility systems.

Do not market an early prototype as a replacement for a cane, guide dog, trained orientation/mobility techniques, medical device, or certified navigation aid.

High-stakes navigation features should require much stronger validation and may need multiple data sources beyond AI vision alone.

## Commercial Possibilities

Potential future models:

- consumer subscription;
- accessibility-focused plan;
- premium realtime usage tier;
- family/caregiver plan;
- enterprise accessibility licensing;
- rehabilitation / institutional partnerships;
- wearable/device partnerships;
- API/SDK licensing for contextual vision workflows.

Pricing should reflect inference cost while preserving reasonable access for people who rely on the capability.

## Non-Goals for the Founding Stage

- custom foundation model training;
- autonomous driving or safety-critical navigation;
- building proprietary camera hardware immediately;
- medical diagnosis;
- replacing FamiliarVoice as the current flagship;
- broad feature development before the core conversational visual loop is proven.

## Activation Gate

This repository becomes an active Zenith engineering project only after an explicit company decision following FamiliarVoice's release/monetization milestone.

Until then, allowed work is limited to:

- product notes;
- user-problem research;
- architecture research;
- API/platform feasibility experiments;
- accessibility interviews/observations;
- low-cost throwaway prototypes that do not derail FamiliarVoice.

## Long-Term Role in Zenith

Zenith Visual Assistant represents the **Perceive** layer of the company thesis:

> **Perceive -> Understand -> Act**

Its purpose is to make the visual world more available to an AI assistant and therefore more understandable to the user.
