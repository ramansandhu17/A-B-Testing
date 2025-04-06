# A/B Testing Project: Snapchat Discover Feed Layout Optimization

## Overview

This project explores whether changing the **Snapchat Discover feed layout** from a traditional **list format** to a **grid layout** can improve user engagement. The key metric used for evaluation is the **Tap-Through Rate (TTR)** — the percentage of content impressions that result in a user tap.

---

## Project Statement

### Objective  
Evaluate whether a **grid layout** of the Discover feed increases **Tap-Through Rate (TTR)** compared to the existing **list layout**.

### Background  
Snapchat’s Discover tab is central to its content strategy. The layout in which stories and videos are displayed may influence how users engage with them. This A/B test simulates a layout change to understand its potential effect on user behavior.

### Experiment Design  
Users are randomly assigned to one of two groups:

- **Control Group**: List layout (current design) - The usual group that gets nothing new and are exposed to the generic layout
- **Test Group**: Grid layout (new design) - The new group where the layout is different

Each user is exposed to multiple Discover stories. For each, we track:
- `impressions`: Number of stories shown
- `taps`: Number of stories tapped

We compute **Tap-Through Rate (TTR)**:


### Hypotheses

- **Null Hypothesis (H₀)**: There is **no difference** in TTR between the grid and list layouts.
- **Alternative Hypothesis (H₁)**: The **grid layout** has a **higher TTR** than the list layout.

---

### Goal

Determine whether the grid layout leads to a **statistically significant** increase in TTR and if the layout change should be rolled out to all users.
