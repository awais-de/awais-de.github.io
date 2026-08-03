---
layout: page
title: Neural Audio Codec
description: Low-latency neural speech codec, rate-distortion research (M.Sc. thesis)
img:
importance: 2
category: research
---

Low-latency neural speech codec, rate-distortion research for my M.Sc. thesis at TU Ilmenau — supervised by **Prof. Gerald Schuller** (TU Ilmenau) and co-supervised by **Andreas Brendel** (Fraunhofer IIS, Erlangen).

A causal transformer encoder/decoder with residual vector quantisation (RVQ), targeting 8–16 kbps for real-time speech. Run as an eight-phase controlled curriculum rather than a hyperparameter sweep, including a deliberate counter-experiment (D-VAE) designed to fail. Quality plateaued at 3 bits per codebook, locating the ceiling in latent entropy rather than quantiser resolution.

Known limitations — including a `torch.triu`/`torch.tril` bug that invalidated one attention-window phase — are disclosed in full in the repo.

**Stack:** Python, PyTorch, torchaudio, causal transformers, RVQ, autoregressive models, librosa, PESQ, STOI

**Status:** In progress

**Code:** [github.com/awais-de/audio_cod](https://github.com/awais-de/audio_cod)
