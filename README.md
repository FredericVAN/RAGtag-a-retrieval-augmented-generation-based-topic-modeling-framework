
---

# 🧠 RAGtag: Retrieval-Augmented Topic Modeling Framework

> 🔗 Official Project Repository for the paper:
>
> **"RAGtag: A Retrieval-Augmented Generation-Based Topic Modeling Framework"**
>
> 📍 *National Key Laboratory of Data Space Technology and System, AIBD, Beijing*
>
> ✍️ *Zhuofan Shi, Shuyang Nie, Shiqi Ning, Fan Li, Kun Liu, Tong Huo*
>
> 🗓️ DMBD (2024)

---

## 🚧 Project Status

🎉 **Coming Soon!**

We’re actively preparing the official implementation of  **RAGtag** , and will release the codebase, datasets, and API demos shortly. Stay tuned!

---

## 📌 Introduction

**RAGtag** is a novel topic modeling framework that combines **Retrieval-Augmented Generation (RAG)** with **Large Language Models (LLMs)** to generate, assign, and merge topics across document corpora — overcoming limitations of existing models like LDA, BERTopic, and TopicGPT.

🌟 **Highlights:**

* 🚫 No need for predefined topic templates or fixed context windows
* 🔍 Enhanced interpretability and topical coherence
* 📊 Superior performance across multilingual datasets (EN + ZH)
* 🧠 Supports topic generation, clustering, and database merging

---

## 🧱 Architecture Overview

RAGtag comprises several key modules:

```
[Document Corpus] 
      ↓
[LLMLingua Compression] 
      ↓
[Generate Topic via RAG] 
      ↓
[Merge with Database Topics] 
      ↓
[Cluster by Topic Proximity] 
```

💡 Internally, RAGtag leverages:

* **RAG service** : Hybrid vector+keyword retrieval with reranking
* **Generator LLM** : Qwen2 7B or Mistral 7B
* **Reflection agents** : Actor + Critic-based topic merging
* **Chain-of-Thought prompts** for enhanced reasoning



---

## 📊 Performance Summary

RAGtag was evaluated on three datasets (📄 BBC News, 🏛️ U.S. Bills, 📰 TouTiao CN), and compared to:

* 🟠 **TopicGPT** (prompt-based LLM)
* 🔵 **BERTopic** (embedding + TF-IDF clustering)

📈 **Key Metrics:**

* Normalized Mutual Information (NMI)
* Adjusted Rand Index (ARI)
* Purity Score

🧪 RAGtag consistently outperformed or matched baselines across clustering accuracy and topic diversity.

---

## 🧪 Example Use Cases

* 💼 Industrial document sorting
* 📚 Academic literature categorization
* 📰 News topic tagging (Chinese & English)
* 📊 Custom corpus labeling & exploration

---

## 🧾 License

This project will be released under the  **Apache 2.0 License** .

---

## 📖 Citation

If you use this framework in your work, please cite:

```bibtex
@article{shi2024ragtag,
  title={RAGtag: A Retrieval-Augmented Generation-Based Topic Modeling Framework},
  author={Shi, Zhuofan and Nie, Shuyang and Ning, Shiqi and Li, Fan and Liu, Kun and Huo, Tong},
  journal={To appear, 2024}
}
```

---

## 📬 Contact & Acknowledgement

📧 Contact: shizhuofan@stu.pku.stu.cn

🏢 Affiliations: National Key Lab of Data Space Technology and System, AIBD, Beijing

🙏 Thanks to the open-source communities of Qwen, Mistral, LangChain, LLM-Lingua, and Reflexion!
