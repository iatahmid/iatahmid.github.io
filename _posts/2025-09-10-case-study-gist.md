---
title: 'Case Study: Gaze Aware Immersive Space to Think'
date: 2025-09-10
permalink: /post/2025/09/case-study-gist/
tags:
  - ux
  - research
feature_row_guidelines:
  - title: '<i class="fas fa-seedling" aria-hidden="true"></i> Invest in the start'
    excerpt: "Curate or bootstrap an initial evidence set (expert or agent) so gaze-aware cues amplify a solid baseline rather than compensate for poor priors."
  - title: "Reduce, then enrich"
    excerpt: "Use global, interpretable signposts during foraging; layer local, relationship-focused cues on demand during synthesis."
    icon: "fas fa-layer-group"
  - title: "Prioritize trust and clarity"
    excerpt: "Attach brief explanations: contributing terms, one-line summary, and a confidence indicator to speed fit judgments."
    icon: "fas fa-check-circle"
  - title: "Preserve agency"
    excerpt: "Offer accept/dismiss/defer/undo; maintain spatial stability and change layout only when requested."
    icon: "fas fa-user-shield"
  - title: "Keep assistance in situ"
    excerpt: "Provide previews, lightweight filters, and context-aware actions near the content to reduce keyboard-based search."
    icon: "fas fa-magic"

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

### Key Findings
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

### Key Findings
> Users' self-reported relevance aligned strongly with GazeScore-suggested relevance of the topics. \\
> Users wished to include the GazeScore-derived suggestions within their sensemaking pipeline.

## Design Approach
It is not enough to just predict the user's perception, we need ways to convey that information to the user with meaningful and intuitive visual cues. We need to maintain the following criteria for these visual cues.

* Detect Relevant Information
* Quantify the Relevance
* Readability of the Relevant Information
* Readability of the Irrelevant Information
* Preserving the Spatial Relation

We investigated the following visual cues and analyzed their effectiveness in achieving the criteria.

* Size (more relevant => bigger document)
* Background Color (more relevant => darker color)
* Border Color (more relvant => darker color)
* Orientation (less relevant => tilt the document)
* Animation (brings more relevant documents closer)
* Depth (pushes less relevant documents further from the user)

<!-- Table: Evaluation of the visual cues for document relevance representation -->
<table style="width:100%; border-collapse:collapse;">
  <thead>
    <tr>
      <th style="text-align:left;">&nbsp;</th>
      <th style="text-align:center; width:7rem;">Size</th>
      <th style="text-align:center; width:11rem;"><strong>✅ Background Color</strong></th>
      <th style="text-align:center; width:11rem;">Border Color</th>
      <th style="text-align:center; width:9rem;">Orientation</th>
      <th style="text-align:center; width:9rem;">Animation</th>
      <th style="text-align:center; width:7rem;">Depth</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Detect Relevant Documents</strong></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#fff4e5; color:#8a4b00;">~ Depends on border thickness</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
    </tr>
    <tr>
      <td><strong>Quantify Relevance</strong></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#ffeef0; color:#8a1a1a;">✗ No</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#ffeef0; color:#8a1a1a;">✗ No</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#ffeef0; color:#8a1a1a;">✗ No</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
    </tr>
    <tr>
      <td><strong>Readability for Relevant Documents</strong></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#fff4e5; color:#8a4b00;">~ Depends on color gradient</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#ffeef0; color:#8a1a1a;">✗ No</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
    </tr>
    <tr>
      <td><strong>Readability for Irrelevant Documents</strong></td>
      <td style="text-align:center;"><span class="badge" style="background:#ffeef0; color:#8a1a1a;">✗ No</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#ffeef0; color:#8a1a1a;">✗ No</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
    </tr>
    <tr>
      <td><strong>Preserving Spatial Relation</strong></td>
      <td style="text-align:center;"><span class="badge" style="background:#ffeef0; color:#8a1a1a;">✗ No</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#ffeef0; color:#8a1a1a;">✗ No</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#ffeef0; color:#8a1a1a;">✗ No</span></td>
    </tr>
  </tbody>
</table>
<p><em>Evaluation of the visual cues for document relevance representation.</em></p>

Based on the evaluation, we chose **background color** as the visual cue to represent the user's perceived relevance.

## Evaluating GazeScore-Derived Visual Cues
**Research Question:** Can the users' gaze-derived visual cues help users offload their thought process?

### Experiment Design
* **Two Part Experiment:**
  * *Experiment with Professional Analyst (N=4):* Solves a sensemaking puzzle efficiently but does not write down their approach. The AI monitors their gaze and annotates the documents with the visual cues.
  * *Experiment with Novice Analyst (N=40):* Follows the professional's approach solely based on their gaze-derived visual cues.
* **User Experience:** 
  * Virtual elements (documents, notes, and labels) overlaid on the real world.
  * 6-DOF controller interactions.
  * Meta Quest Pro with eye-tracking enabled. 
* **Data Collection:** NASA TLX, User Engagement Questionnaire, Trust in AI Questionnaire, Semi-structured interview, Interaction Logs, Eye-tracking logs.

### Key Findings
> Gaze-aware AI, with the visual cues, helps users to follow the professional analyst's approach to the puzzle. \\
> Gaze-aware AI, with the visual cues, reduces the physical demand of the user.

## Final Design Guidelines (Selected)
{% include feature_row id="feature_row_guidelines" type="left" %}

## Impact
* **Academic:** First step towards AI-mediated immersive sensemaking by leveraging eye-tracking data.
* **Industry:** Design guidelines directly impacts professional analysts whose regular responsibilities require them to perform sensemaking.

