---
layout:     post
title:      "Verta - An LLM Chatbot"
author: "Nishith"
catalog: true
header-img: "img/verta-bg.jpg"
header-mask: 0.4
tags:
  - LLMs
  - MLOps
---

# Verta - An LLM Chatbot 
*This project is done as part of the course IE7374 - Machine Learning Operations*

The Verta Chatbot **[featured as the top project for Fall 2024](https://www.mlwithramin.com/MLOps/projects)** is a sophisticated AI-driven solution designed to enhance user interactions with product information. Deployed as a serverless **FastAPI's API** on Cloud Run, it serves users by answering questions about products, leveraging both metadata and user reviews for context. The chatbot utilizes a multi-agent workflow, with distinct agents performing specialized roles. A **Metadata Agent** is responsible for summarizing product descriptions, while a Retriever Agent fetches relevant data from a vector store containing user reviews. This allows the chatbot to answer a wide range of user inquiries, drawing on both product details and feedback from other customers.

The database for this solution is hosted on PostgreSQL in **Google Cloud Platform (GCP)**, ensuring scalable, reliable storage. The project utilizes **CI/CD pipelines** via GitHub Actions, automating code deployment and ensuring seamless integration and delivery. Additionally, the system incorporates **LLM-as-Judge** to generate synthetic test questions for a set of products, while bias detection algorithms analyze potential biases in the chatbot's responses to ensure fairness and accuracy.

Experiment tracking is managed through **MLflow**, which captures model performance and experiment metadata, while Langfuse is used for tracing user interactions and gathering feedback to continuously improve the system. For monitoring and alerting, **GCP Logs** are utilized with notifications configured to send alerts to a Teams channel for real-time system health checks.

The chatbot’s data orchestration is powered by **Apache Airflow**, while **FaisDB** is used as the vector store for storing product reviews and context. The system integrates three LLMs — **GPT-4o-Mini**, **Llama 3.1-70B**, and **Llama 3.1-8B** — running on four nodes to support its operations. The chatbot’s multi-agent flow is managed using **LangGraph**, a framework for orchestrating complex workflows. For ease of use, the chatbot is also available as a **Streamlit web app**, with integration capabilities for custom frontends via API, secured using **Auth Bearer Tokens**.

[Link to GitHub Repo - LLM Part](https://github.com/eCom-dev5/eCom-Chatbot)

[Link to GitHub Repo - UI Part](https://github.com/eCom-dev5/eCom-Chatbot-UI)
