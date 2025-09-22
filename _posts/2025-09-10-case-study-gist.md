---
title: 'Case Study: Gaze Aware AI for Immersive Analytics'
date: 2025-09-10
permalink: /post/2025/09/case-study-gist/
classes: wide
toc: true
toc_sticky: true

# Optional page header hero
# header:
#   overlay_image: images/teasers/logan_cropped.jpg
#   overlay_filter: 0.35
#   caption: "Prototype visuals sanitized for portfolio use"

# Quick, scannable highlights (uses Minimal Mistakes feature_row)
feature_row:
  - title: '<i class="fas fa-bullseye" aria-hidden="true"></i> Problem'
    excerpt: "Sensemaking across many interconnected documents overwhelms users’ working memory."
  - title: '<i class="fas fa-vr-cardboard" aria-hidden="true"></i> Solution'
    excerpt: "Mixed Reality workspace + gaze-aware AI cues to guide foraging and synthesis."
  - title: '<i class="fas fa-chart-line" aria-hidden="true"></i> Evidence'
    excerpt: "5 studies (N=115); alignment between self-reported relevance and GazeScore; lower workload signals."
---

<div class="notice--info" markdown="1">
**Audience:** UX Designer & UX Researcher recruiters.  
**My role:** End-to-end research + prototyping in MR; eye-tracking–driven AI cues; multi-study validation.
</div>

{% include feature_row %}

## Introduction
When users must browse large amounts of **interconnected** information, the process can be mentally exhausting. This project investigates how **Mixed Reality (MR)** and **Artificial Intelligence (AI)** can reduce that demand by guiding attention and supporting synthesis.

## Cross-functional Partners
- **Principal Investigator (PI)** — 3D Interaction & User Experience  
- **Co-PI** — Visualization & Semantic Interaction  
- **Industry Sponsor** — Consumer (Analyst) Behavior Analysis  
- **Consultants** — Eye Tracking; Human–AI Collaboration  
- **Consumers/Analysts** — Feedback on demo

## My Role
**Lead Researcher**
- Surveyed prior work, defined the research pathway, implemented MR applications, and ran the studies.
- **N=115** across **5 studies** in room-scale MR; **60–120 min** sessions; quantitative + qualitative analysis.
- Weekly stakeholder readouts; translated findings into design guidelines.

## Research Question
**Primary RQ:** How can we **alleviate cognitive load** during sensemaking tasks?

## Approach: Identify the Problems
### Resources Available
- **100+ hours** of videos: people solving complex sensemaking tasks in MR.
- **30+ papers** across small 2D, large 2D, and immersive 3D displays.
- Weekly stakeholder check-ins to validate interpretations.

### Outcome (Key Problems)
- **Not enough space for data.** Users struggle to arrange and revisit large information sets.
- **Exhaustive browsing.** Users juggle too much in working memory while searching for new, related items.

## Solution Proposal
- **Not enough space?** Use a **3D environment** to show the dataset at once, leveraging spatial memory and embodied interaction.  
- **Overloaded mind?** Train an **AI that monitors gaze** to anticipate perceived relevance and provide **personalized visual cues** to browse more efficiently.

---

## <i class="fas fa-clipboard-check" aria-hidden="true"></i> Study 1: Validating Human–AI Collaboration
**RQ:** Can AI alleviate user load by automating parts of the sensemaking process?

### Experiment Design
- **Participants:** Within-subjects (**N=27**)
- **Task:** Organize flash cards into meaningful clusters
- **Conditions:**
  - **Semi-automated clustering:** AI clusters nearby cards
  - **User-controlled clustering:** User creates clusters manually
  - **Control:** No explicit clusters
- **User Experience:** Virtual room with a passthrough portal to keyboard; controller interaction; **Varjo XR-3** (tethered)
- **Data:** **NASA-TLX**, **SUS**, **UEQ**, semi-structured interview, interaction logs

### Key Findings
> Users preferred the **semi-automated** approach for **ease, comfort, and performance**.  
> Users wanted **rationales** to avoid feeling a loss of control when AI acted.

---

## <i class="fas fa-clipboard-check" aria-hidden="true"></i> Study 2: Turning Gaze into Intent
**RQ:** How do we convert raw gaze into a reliable predictor of user **intent** during sensemaking?

**Key Challenge:** In multi-document sensemaking, simple metrics (fixation time/count) suffer **frequency** and **length** biases. We introduced **GazeScore** to address these biases and tested its feasibility.

### Experiment Design
- **Participants:** **N=12**
- **Task:** Solve a sensemaking puzzle with **two entwined plots**
- **User Experience:** Virtual documents/notes/labels **overlaid on the real world**; hand gestures; **HoloLens 2** with eye tracking
- **Data:** **NASA-TLX**, self-reported topic relevance, interviews, interaction + eye-tracking logs

### Key Findings
> **Self-reported relevance** aligned strongly with **GazeScore-suggested** topic relevance.  
> Participants wanted **GazeScore-derived suggestions** integrated into their workflow.

---

## <i class="fas fa-palette" aria-hidden="true"></i> Design Approach
It’s not enough to predict perception; the system must **communicate relevance** via intuitive visual cues while preserving task flow.

**Cue goals**
- Detect relevant information
- Quantify relevance
- Maintain readability (relevant & irrelevant)
- Preserve spatial relations

**Cues tested**
- **Size** (more relevant → larger)
- **Background color** (more relevant → darker)
- **Border color** (more relevant → darker)
- **Orientation** (less relevant → tilt)
- **Animation** (bring relevant closer)
- **Depth** (push less relevant farther)

<!-- Your existing styled table preserved -->
<table style="width:100%; border-collapse:collapse;">
  <thead>
    <tr>
      <th style="text-align:left;">&nbsp;</th>
      <th style="text-align:center; width:7rem;">Size</th>
      <th style="text-align:center; width:11rem;"><strong>Background Color</strong></th>
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
      <td style="text-align:center;"><span class="badge" style="background:#fff4e5; color:#8a4b00;">~ Depends (thickness)</span></td>
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
      <td><strong>Readability (Relevant)</strong></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#fff4e5; color:#8a4b00;">~ Depends (contrast)</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#ffeef0; color:#8a1a1a;">✗ No</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
    </tr>
    <tr>
      <td><strong>Readability (Irrelevant)</strong></td>
      <td style="text-align:center;"><span class="badge" style="background:#ffeef0; color:#8a1a1a;">✗ No</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#ffeef0; color:#8a1a1a;">✗ No</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
    </tr>
    <tr>
      <td><strong>Preserve Spatial Relations</strong></td>
      <td style="text-align:center;"><span class="badge" style="background:#ffeef0; color:#8a1a1a;">✗ No</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#ffeef0; color:#8a1a1a;">✗ No</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#e6ffed; color:#036200;">✓ Yes</span></td>
      <td style="text-align:center;"><span class="badge" style="background:#ffeef0; color:#8a1a1a;">✗ No</span></td>
    </tr>
  </tbody>
</table>
<p><em>Evaluation of visual cues for representing document relevance.</em></p>

**Decision:** We selected **background color** as the primary relevance cue.

---

## <i class="fas fa-clipboard-check" aria-hidden="true"></i> Evaluating GazeScore-Derived Cues
**RQ:** Can gaze-derived cues help users **offload** parts of their thought process?

### Experiment Design
- **Two-part study**
  - **Professional analysts (N=4):** Solve the puzzle efficiently (without writing their approach). AI monitors gaze and annotates documents via visual cues.
  - **Novice analysts (N=40):** Follow the professional’s approach guided **only** by the gaze-derived cues.
- **User Experience:** Virtual documents/notes/labels overlaid on the real world; **6-DoF** controllers; **Meta Quest Pro** with eye tracking
- **Data:** **NASA-TLX**, **User Engagement Questionnaire**, **Trust in AI** questionnaire, interviews, interaction + eye-tracking logs

### Key Findings
> Gaze-aware AI + cues helped novices **follow expert approaches**.  
> Gaze-aware cues **reduced physical demand**.

---

## <i class="fas fa-list-check" aria-hidden="true"></i> Final Design Guidelines (Selected)
- <i class="fas fa-seedling" aria-hidden="true"></i> **Invest in the start.** Ensure early exposure to **essential** information so gaze-aware AI learns from a solid baseline instead of compensating for poor priors.
- <i class="fas fa-layer-group" aria-hidden="true"></i> **Reduce, then enrich.** Begin with **minimal, global signposts** during foraging; progressively layer **local, relationship-focused cues** as synthesis begins.
- <i class="fas fa-check-circle" aria-hidden="true"></i> **Prioritize trust and clarity.** Attach brief explanations to each suggestion (key terms, one-line summary, confidence) so users can judge fit without breaking flow.
- <i class="fas fa-user-shield" aria-hidden="true"></i> **Preserve agency.** Offer accept / dismiss / defer / undo; keep spatial stability; change layout only on user request.
- <i class="fas fa-map-marker-alt" aria-hidden="true"></i> **Keep assistance in situ.** Use previews, lightweight filters, and context-aware actions near the content to reduce keyboard-based search.

---

## <i class="fas fa-chart-line" aria-hidden="true"></i> Impact
- **Academic:** Early evidence for **AI-mediated immersive sensemaking** using gaze-derived signals.  
- **Industry:** Actionable guidelines for analysts working with **high-volume, interconnected** data in MR.
