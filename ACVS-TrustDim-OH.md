---

marp: true
theme: default
title: "Unpacking Public Trust"
backgroundImage: url('')
paginate: true
--------------

# Unpacking Public Trust

## Computational and Qualitative Insights from Australians' Open-Ended Explanations

**Osbern Huang**
School of Government and International Relations, Griffith University
Australian Society for Quantitative Political Science, 2025

<!-- notes:
Welcome everyone. This presentation draws from work on understanding why Australians trust or distrust their politicians and government agencies, using a mix of open-ended responses and machine learning tools. -->

---

## Theoretical Background

* Political trust: confidence that rulers act in the public interest
* Dimensions: competence, integrity, benevolence【14†L9-L14】
* Easton (1975):

  * **Diffuse trust**: faith in system
  * **Specific trust**: trust in current officeholders
* Citizens differentiate trust in **politicians** vs **public agencies**【14†L22-L26】

<!-- notes:
We begin with classic theory: Easton, Mayer, Levi. Emphasize that political trust is not monolithic. -->

---

## Drivers of Political Trust

* Partisanship effects: governing party advantage【20†L85-L93】
* Identity & marginalisation: trust gaps by ethnicity, class【20†L115-L124】
* Performance feedback: scandals, policy failure = trust shocks【14†L50-L58】
* Trust as a reservoir: maintains legitimacy in hard times【14†L62-L70】

<!-- notes:
Set up empirical drivers: group-based trust, situational shocks. -->

---

## Why a Bottom-Up Approach?

* Closed-ended trust questions limit respondents to fixed frames【22†L375-L384】
* May conflate intensity with reason (e.g. "how much" trust without "why")
* Open-ended responses let people define trust on their terms
* Qualitative research: betrayal, broken promises dominate distrust【22†L402-L410】

<!-- notes:
Justify our method: open-ends give richer, inductive view of what trust means. -->

---

## ACVS 2023: Survey Design

* N=1200 representative Australian adults

* Open-ended module:

  1. Name a politician you trust & why (*C*)
  2. ...distrust & why (*CC*)
  3. Name a gov agency you trust & why (*D*)
  4. ...distrust & why (*DD*)

* Each response tagged with type (trust/distrust, pol/agency)

<!-- notes:
These items form the empirical basis for both supervised and unsupervised work. -->

---

## Coding Framework: 8 Dimensions

* Responses scored 0.00 to 4.00 on each dimension:

  1. **Reliability**
  2. **Honesty & integrity**
  3. **Benevolence / duty**
  4. **Competence / performance**
  5. **Transparency**
  6. **Responsiveness**
  7. **Accountability**
  8. **Values alignment**【23†L8-L16】

* Allows fine-grained scoring per response using LLM-assisted classification

<!-- notes:
Supervised scoring gives dimensionality to otherwise qualitative data. -->

---

## Unsupervised Discovery Pipeline

* Compute embeddings (OpenAI) → cluster (K-means, HDBSCAN)
* Identify K using elbow method [placeholder: figure_k_elbow_plot]
* Label clusters with LLM summaries + manual review
* Cluster–dimension alignment aids interpretation

<!-- notes:
Parallel approach: let data speak. Supports or challenges theory-driven coding. -->

---

## [prelim] Cluster Themes

* **Politician distrust**: dishonesty, self-interest, broken promises
* **Agency distrust**: poor performance, impersonal service
* **Politician trust**: community focus, honesty, duty
* **Agency trust**: competence, reliability, procedural fairness

[placeholder: cluster_heatmap]

<!-- notes:
Mark as preliminary but compelling. We see strong themes emerging organically. -->

---

## [prelim] Supervised Scores

* Trust in **politicians**:

  * High scores on *Honesty*, *Benevolence*, *Alignment*
* Trust in **agencies**:

  * Higher *Competence*, *Accountability* scores
* Distrust shows inverse pattern (e.g. dishonest vs incompetent)

[placeholder: supervised_dimension_scores_table]

<!-- notes:
Preliminary, but shows how score profiles distinguish actor types. -->

---

## Comparing Trust Targets

* Politicians: judged on **values**, **motives**, **character**【13†L108-L114】
* Agencies: judged on **delivery**, **process fairness**【13†L115-L124】
* Distrust asymmetry: moral failure vs service failure【13†L156-L165】

<!-- notes:
Trustworthiness means different things for different actors. Qual data makes that clear. -->

---

## Implications for Theory & Measurement

* ABI triad (Ability, Benevolence, Integrity) may be too narrow【27†L127-L131】
* Need to measure *duty/service*, *promise-keeping*, *alignment*
* Use open-ends for validity checks and construct exploration
* Mix supervised and unsupervised coding for scalability

<!-- notes:
Suggest improvements to trust batteries. Open-ended responses aren't just noise—they reveal hidden structures. -->

---

# Next Steps

* Finalise unsupervised cluster labels
* Score full sample on 8 dimensions
* Validate results across actors, parties, subgroups
* Build interactive dashboard for public use

<!-- notes:
Mention where this goes next: dissemination, dashboard, additional modelling. -->

---

# Thanks

**[osbern.huang@griffith.edu.au](mailto:osbern.huang@griffith.edu.au)**
Griffith University | Australian Society for Quantitative Political Science 2025

[placeholder: logo or image]

<!-- notes:
End with thanks and contact. -->
