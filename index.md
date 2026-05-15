# **StanceEval-2026**: Stance Detection in Arabic Language Shared Task

### Hosted with [Arabic Natural Language Processing Conference (ArabicNLP 2026)](https://arabicnlp2026.sigarab.org)

## 1. Overview
**StanceEval-2026** is a shared task on Arabic stance detection using the Mawqif-v2 dataset. Given an Arabic tweet and a target, participants classify the stance as **Favor**, **Against**, or **None**. The task evaluates both seen and unseen targets:

- **Track 1**: Seen Targets (COVID-19 vaccine, digital transformation, women empowerment)
- **Track 2**: Unseen Targets (trimester system, e-cars, women driving)

💰 **Total Prize Pool: $1,600** ($800 per track)

## 2. Task Description
The dataset includes multi-label annotations (stance, sentiment, sarcasm). Track 2 evaluates generalization beyond training topics.

| Track | Targets | Status |
|-------|---------|--------|
| Track 1 | COVID-19 vaccine, Digital transformation, Women empowerment | Seen (training) |
| Track 2 | Trimester system, E-cars, Women driving | Unseen (test only) |

## 3. Dataset — Mawqif-v2

| Split | Tweets | Source |
|-------|--------|--------|
| Training | 3,502 | 3 seen targets |
| Development | 619 | 3 seen targets |
| Test (Track 2) | 996 | 3 unseen targets |

Annotations: Stance (Favor/Against/None), Sentiment, Sarcasm. Each tweet labeled by 3 annotators.

## 4. Evaluation
- **Primary Metric**: Favg2 — macro-average F1 over Favor and Against labels
- **Secondary Metric**: Favg3 — macro-average F1 over all three labels

### Baseline Results (Development Set)

| Model | Track 1 Favg2 | Track 2 Unseen Favg2 |
|-------|-------------|-------------------|
| AraBERT-twitter | 83.90 | 60.93 |
| Qwen 2.5 (72B, zero-shot) | 84.25 | 74.75 |
| JAIS (70B, zero-shot) | 83.37 | 69.10 |

## 5. Tentative Timeline
- **May 16, 2026**: Release of task website, training/dev data, and evaluation scripts
- **July 20, 2026**: Registration deadline and release of blind test data
- **July 30, 2026**: Final results released
- **August 22, 2026**: Camera-ready system description papers due
- **September 1, 2026**: Shared task overview papers due
- **October 24–29, 2026**: ArabicNLP 2026 / EMNLP 2026, Budapest, Hungary

## 6. Organizers' Details
- **Rasha Albalawi**, KFUPM, Saudi Arabia — g202521490@kfupm.edu.sa
- **Nuha Albadi**, KFUPM / SDAIA-KFUPM JRC for AI — nuha.badi@kfupm.edu.sa
- **Hamzah Luqman**, KFUPM / SDAIA-KFUPM JRC for AI — hluqman@kfupm.edu.sa
- **Saad Ezzini**, KFUPM — saad.ezzini@kfupm.edu.sa
- **Maram Kurdi**, KFUPM — maram.kurdi@kfupm.edu.sa
- **Asma Yamani**, KFUPM — g201906630@kfupm.edu.sa
- **Ahmad Ashraf**, KFUPM — g202411740@kfupm.edu.sa
- **Maged S. Al-Shaibani**, KFUPM / JRCAI — majed.alshaibani@kfupm.edu.sa
- **Nora Alturayeif**, HUMAIN, Saudi Arabia — nalturayeif@humain.com

## 7. Participation Guidelines
- 📋 **Register here**: [StanceEval-2026 Registration Form](https://forms.gle/w4KsiSHswVRDJzWd7)
- For participation guidelines, see [Participation Guidelines](guidelines.md).
- For paper submission guidelines, see [Paper Submission Guidelines](PAPER.md).
- Previous edition: [StanceEval 2024](https://sites.google.com/view/stanceeval/home)

---

### Logistics and Support
- **Website**: GitHub Pages | **Submission**: Codabench | **Support**: Email + Discord channel

### Anti-Harassment Policy
We uphold the [ACL Anti-Harassment Policy](https://www.aclweb.org/adminwiki/index.php?title=Anti-Harassment_Policy).
