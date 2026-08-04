---
layout: page
title: English-to-ASL Translation
description: NLP pipeline translating English text into ASL gloss, mapped to sign videos
img:
importance: 6
category: ai
---

Semester-long NLP + computer vision project translating English sentences into American Sign Language (ASL) gloss and mapping the output to corresponding sign videos.

A multi-stage pipeline handles dataset preprocessing and tokenization, then fine-tunes a text-to-gloss model on **ASLG_PC12**, with optional gloss-to-video alignment against **WLASL2000**. Runs end to end either as a single notebook or as modular Python scripts.

**Stack:** Python, PyTorch, Hugging Face, Jupyter

**Status:** Complete

**Code:** [github.com/awais-de/asl](https://github.com/awais-de/asl)
