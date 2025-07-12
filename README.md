# AI-Based Defect Classification System (DCS)

## Executive Summary
Automated root cause classification system for battery cell defects using multi-class image classification and integrated equipment log data. Reduced manual analysis time by 60%, saving $300K annually per line. Delivered real-time dashboards to QA engineers.

---

## 1. Business Problem & Objective

In high-volume battery manufacturing, defect identification relies on binary OK/NG judgments from vision inspection systems without specific defect classification. Manual review of NG images and upstream sensor data was time-consuming and inconsistent.

**Business Objectives:**
- Automate defect type classification to reduce manual inspection time and resource use.
- Eliminate the need for repetitive image downloads, defect sorting, and root cause manual analysis.
- Improve accuracy and efficiency in identifying core-related defects such as TAB misalignment, Core length issues, and external pressure deformities.

**Pain Points Addressed:**
- Manual root cause analysis took approximately 4 hours per defect batch.
- Engineers manually checked SPC logs, image downloads, and defect types repeatedly.
- High labor resource cost and risk of inconsistent analysis.

**Process Before vs. After DCS Implementation**

```mermaid
graph LR
  A[Problem Identification (Defect Increase)] --> B[Defect Type Classification]
  B --> C[Image Download + SPC Analysis]
  C --> D[Root Cause Analysis]
  D --> E[Production Team Request]

  subgraph Before DCS
    A --> B
    B --> C
    C --> D
    D --> E
  end

  subgraph After DCS
    A -->|Automated| F[Defect Classification Output]
    F --> G[Visualization + Email Notification]
    G --> H[Production Team Request]
  end
