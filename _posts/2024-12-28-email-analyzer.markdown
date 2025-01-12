---
layout:     post
title:      "E-mail/Text Tone Analyzer"
author: "Nishith"
catalog: true
header-img: "img/email-bg.png"
header-mask: 0.4
tags:
  - Natural Language Processing
  - LLMs
  - Web Application
---

The email tone analyzer integrates **sentiment analysis** and **LLM**s to identify the formality level of an email or text. To improve the LLM's ability to tell whether an email is categorized as formal or informal, LLM used is fine tuned using a dataset that contains a mixture of emails with positive, negative, neutral, formal, and informal texts. Overall, this study tells the potential of sentiment analysis and LLMs like **llama**, **gemini**. The findings could be beneficial for anyone who is writing an email and wants to get suggestions on the tone of the email.

With the increasing use of emails, text messages, and other digital communication, it’s important to be mindful of the tone we use when sending messages. In academic and professional settings, an inappropriate tone can lead to misunderstandings or serious issues. For example, if you are a new business owner reaching out to a supplier, sending an informal email could leave a poor impression, potentially harming your business relationships and affecting your company’s success.

To address this challenge, an innovative application designed to provide both overall and sentence-level tone analysis for emails and text messages is developed. This tool empowers users to identify and improve potential tone issues in their communications, ensuring clarity and professionalism. The development of this application involved a strategic combination of transformer models like **RoBERTa** and **Llama 3.2**.  Firstly, **weak supervision methods** are employed, leveraging **transformers** and the LlaMA model to efficiently label a large corpus of emails. Weak supervision allows us to generate high-quality labels for the data with minimal manual intervention, significantly reducing the time and effort required for annotation. This labeled dataset is then finally used to fine-tune the **Gemini LLM** to perform the tone classification.

[Link to GitHub Repo](https://github.com/Nishith-Reddy/email_sentiment-tone_analyzer)
