# Zero Hunger — Twitter Discussion Analytics (SDG 2)

A text-mining/NLP analysis of Twitter discussions around **UN Sustainable Development Goal 2: Zero Hunger**, focused on uncovering the **main themes**, **sentiment shifts over time**, and **dominant emotions** in public conversation. :contentReference[oaicite:5]{index=5}

## Project outputs
- 📓 Notebook: `21883191_BUS5PR1_Assignment2.ipynb`
- 📄 Report: `21883191_BUS5PR1_Assignmnt2_Report.pdf` (recommended for full detail)

---

## What I did (methods)
- **N-grams (uni/bi/tri-grams)** on a preprocessed `text_lemmatized` column (lowercased, stop-words removed, lemmatized) to surface recurring terms and phrases. :contentReference[oaicite:6]{index=6}  
- **Tweet count over time** using the `Day` column (datetime) to identify engagement spikes and link them to key moments/events. :contentReference[oaicite:7]{index=7}  
- **Sentiment over time** (positive/negative/neutral) to track how public mood shifts across the timeline. :contentReference[oaicite:8]{index=8}  
- **Topic modelling (LDA)** using tokenized tweets and a BoW/TF-IDF representation to uncover dominant discussion topics. :contentReference[oaicite:9]{index=9}  
- **Emotion detection (Hugging Face)** with `mrm8488/t5-base-finetuned-emotion` (joy, sadness, anger, fear, surprise, love) to measure emotional distribution. :contentReference[oaicite:10]{index=10}

---

## Key insights (high impact)
- **Core discussion themes** are strongly centered on *food security*, *hunger*, *malnutrition*, *agriculture*, and links to *climate change* and *sustainable agriculture*. :contentReference[oaicite:11]{index=11}  
- **Engagement spikes in 2024 (especially July 2024)**, consistent with major global events like the **High-Level Political Forum (HLPF) July 8–17, 2024**, which likely drove increased online discussion. :contentReference[oaicite:12]{index=12}  
- **Sentiment** is mostly **neutral**, suggesting much of the conversation is informational/educational, with noticeable positive spikes around major events and negative dips during crisis-related news. :contentReference[oaicite:13]{index=13}  
- **Topic modelling** highlights **food security + sustainable agriculture** as dominant, with overlap into **malnutrition/world hunger** and strong emphasis on **global partnerships/policy action**. :contentReference[oaicite:14]{index=14}  
- **Emotion detection** shows **joy as the most common emotion**, followed by **sadness and fear**, reflecting both campaign positivity and concern about hunger/poverty and future food security. :contentReference[oaicite:15]{index=15}  

---

## Visual summary (from the notebook)

| Tweet activity over time (tcount) | Sentiment over time |
|---|---|
| ![Tweet count over time](images/tcount.png) | ![Sentiment](images/sentiment.png) |

| Unigram frequency | Bigram frequency |
|---|---|
| ![Unigram](images/unigram.png) | ![Bigram](images/bigram.png) |

| Trigram frequency | Topic modelling (LDA) |
|---|---|
| ![Trigram](images/trigram.png) | ![Topic model](images/topicmodel.png) |

| Emotion distribution (Hugging Face) |
|---|
| ![HuggingFace emotions](images/huggingface.png) |

---

## Recommendations (from findings)
- Align major campaign pushes and policy announcements with **high-attention windows** (e.g., global forums) to maximise engagement. :contentReference[oaicite:16]{index=16}  
- Prioritise **sustainable agriculture** and climate-resilient practices, reflecting how often these themes co-occur in discussion. :contentReference[oaicite:17]{index=17}  
- Use positive messaging (success stories) while translating negative emotions (sadness/fear) into practical support and action. :contentReference[oaicite:18]{index=18}  

---

## Author
Ishan Khanijo — BUS5PR1 (The Hustle) / Team: rookie.ai :contentReference[oaicite:19]{index=19}
