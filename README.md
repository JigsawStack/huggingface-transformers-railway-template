---
title: Hugging Face Transformer
description: A Hugging Face Transformer Railway Template
tags:
  - transformer
  - fastapi
  - hypercorn
  - python
---

# Hugging Face Transformer Example

This example starts up a [FastAPI](https://fastapi.tiangolo.com/) server which runs the [Hugging Face Transformers](https://huggingface.co/docs/transformers/en/index).

This example runs an embedding model on the CPU which works great with railway as resources can scale per requests.

Note: This won't work for GPU work flows and will crash.

## ⬆️ Deploy

Install the [Railway CLI](https://docs.railway.com/guides/cli), then run `railway up`

## ✨ Features

- Transformers
- FastAPI
- Hypercorn
- Python 3.11

Uses [Nixpacks](https://nixpacks.com/docs/providers/python) to deploy on railway which runs Python 3.11 by default.

## 💁‍♀️ How to use locally

- Clone locally and install packages with pip using `pip install -r requirements.txt`
- Run locally using `hypercorn main:app --reload`

## 🧩 Background

The team at [JigsawStack](https://docs.railway.com/guides/cli) is launching a embedding model and we're experimenting with different infrastructure for scalable and affordable CPU usage. Check out the [embedding model here](https://jigsawstack.com/blog/introducing-multimodal-multilingual-embedding-model-for-images-audio-and-pdfs-in-alpha)