---
title: 'Case Study: Gaze Aware Immersive Space to Think'
date: 2025-09-10
permalink: /post/2025/09/case-study-gist/
tags:
  - ux
  - research
---

## Introduction
When users have to browse a lot of information about a single or mutiple topics that are interconnected with each other, the process can be mentally exhausting. This project investigates ways to alleviate this demand with the synergistic power of Mixed Reality and Artificial Intelligence.

## Cross-functional Partners
- Principal Investigator (PI) - 3D Interaction and User Experience
- Co-PI - Visualization and Semantic Interaction
- Industry Sponsor — Consumer (Analyst) Behavior Analysis
- Consultants — Eye tracking and Human-AI Collaboration Paradigm
- Consumer — Feedback on demo

## My Role
**Lead Researcher**
- Studied prior work, developed the research pathway, implemented the 3D applications, and ran the studies
- N=115; 5 studies in a room-scale 3D environment; 60-120 minutes per session; quantitative + qualitative analysis
- Weekly stakeholder meetings; translated findings into design guidelines

## Research Question
**Primary RQ:** How to alleviate the users' cognitive load during sensemaking tasks?  

## Approach: Identify the Problems
### Resources Available:
* 100+ hours video of people solving complex sensemaking tasks in the 3D environment
* 30+ research papers on sensemaking in small 2D displays, large 2D displays, and immersive 3D spaces
* Weekly catchups with the stakeholder to validate interpretations from the videos and papers

### Outcome
We identified the following two key problems:
* **Not enough space for data:** Users struggle with fitting the large amount of information in the space available to them.
* **Exhaustive browsing:** Users need to store too many information in their mind while trying to find new related information at the same time.

## Solution Proposal
**Not enough space?** Use 3D environment to see the whole dataset at once, offering spatial memory, and embodied interaction.
**Overloaded mind with information?:** Train an AI to monitor user's gaze to anticipate their perception of the data, and offer personalized visual cues to browse the data more efficiently.

## Study 1: Validating the effect of Human-AI Collboration
**Research Question:** Can an AI alleaviate user's load by automating parts of their sensemaking task?

### Experiment Design
* **Participants:** Within-subjects (N=27)
* **Task:** Organizing a set of flash cards into meaningful clusters.
* **Conditions:**
  * Semi-Automated clustering: AI looks for cards in proximity and clusters them for the user
  * User-controlled clustering: User makes their own clusters
  * Control: There are no explicit clusters
* **User Experience:** 
  * Virtual room with a passthrough portal to the real world for access to the keyboard.
  * Controller interaction.
  * Varjo XR-3 tethered to a PC. 
* **Data Collection:** NASA TLX, SUS, UEQ, Semi-structured interview, Interaction Logs.

### Findings
> Users preferred automated appraoch because of the ease, comfort, and performance enhancement it offered. \\
> Users were concerned about losing control when the AI did not provide rationales behind its actions.

## Study 2: Validating the use of Gaze
**Research Question:** How to turn raw gaze data into a predictor for users' intent during sensemaking?

**Key Challenge:** In sensemaking, user has to make sense of multiple documents, each about single topics, but has implicit connections between them. For single topic documents, we can measure user's attention from just fixation duration and/or fixation count. But for sensemaking with multiple documents, they introduce frequency bias and length bias. So, we introduced **GazeScore** to address these biases and ran a study to validate the feasiblity of using this new metric.

### Experiment Design
* **Participants:** 12 Participants
* **Task:** Solve a sensemaking puzzle encompassing 2 different plots entwined in the same dataset.
* **User Experience:** 
  * Virtual elements (documents, notes, and labels) overlaid on the real world.
  * Hand gesture interactions.
  * HoloLens 2 with eye-tracking enabled. 
* **Data Collection:** NASA TLX, Self-reported topic relevance, Semi-structured interview, Interaction Logs, Eye-tracking logs.

### Findings
> Users' self-reported relevance aligned strongly with GazeScore-suggested relevance of the topics. \\
> Users wished to include the GazeScore-derived suggestions within their sensemaking pipeline.

## Impact

## Design Guidelines (Selected)

## Timeline
