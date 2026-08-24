  # Jaya Arora
  
  **Fine-tuning transformers · Search reranking · LLM evaluation · Real-time CV**

  [![Portfolio](https://img.shields.io/badge/Portfolio-mission--universe.vercel.app-0E75B6?style=flat-square&logo=vercel&logoColor=white)](https://mission-universe.vercel.app)
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jaya-arora-6892a93a0/)
  [![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:jayaarora2402@gmail.com)
  [![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Jaya242)
  [![LeetCode](https://img.shields.io/badge/LeetCode-FF8C00?style=flat-square&logo=leetcode&logoColor=white)](https://leetcode.com/u/Jaya_242/)
  [![Codeforces](https://img.shields.io/badge/Codeforces-1F8ACB?style=flat-square&logo=codeforces&logoColor=white)](https://codeforces.com/profile/jayaarora242)
  [![CodeChef](https://img.shields.io/badge/CodeChef-5B4638?style=flat-square&logo=codechef&logoColor=white)](https://www.codechef.com/users/jaya_242)
  [![GeeksforGeeks](https://img.shields.io/badge/GeeksforGeeks-2F8D46?style=flat-square&logo=geeksforgeeks&logoColor=white)](https://www.geeksforgeeks.org/user/jayaaros8q1/)
  
  ---

  ## About
  
  Hey — I'm a 3rd-year Mechanical Engineering student at MNNIT Allahabad. I fine-tune deep learning models and ship them end-to-end: training loops, evaluation harnesses, and live demos on Streamlit /
  HuggingFace Spaces.

  My work sits at the intersection of **NLP retrieval**, **search reranking**, and **LLM evaluation** — with a bias toward systems where the ranking is inspectable and the failure modes are named. Currently
  exploring ML engineering internships (Dec 2026 target).

  ---
  
  ## Projects

  ### [`Signal`](https://github.com/Jaya242/crisis-search) — Crisis-Aware Search Reranker
  [![Live Demo](https://img.shields.io/badge/Live%20Demo-Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)](https://crisis-search.streamlit.app)
  
  - **Dynamic-weight news reranker** — MiniLM bi-encoder for relevance, **hybrid credibility** (`0.6 × publisher-prior + 0.4 × DistilBERT classifier`), exponential freshness decay. Mode-aware weight-flipping
   (Standard 0.75/0.10/0.15 → Emergency 0.45/0.25/0.30) triggered by a keyword-based crisis detector.
  - **Fine-tuned DistilBERT** on LIAR2 fact-checking — **75.72% val accuracy** on 12,520 samples with AdamW + linear warmup/decay on Apple Silicon MPS.
  - **70-outlet publisher trust table** blended with the classifier — fixed a real LIAR2 domain gap where the pure classifier ranked NPR below BuzzFeed on the same query.
  - **Deployed on Streamlit Community Cloud** (free CPU tier); 250MB checkpoint served from GitHub Release with cold-start auto-download.
  
  `Python` `PyTorch` `DistilBERT` `sentence-transformers` `Streamlit` `Gradio`

  ---
  
  ### [`Grounding Harness`](https://github.com/Jaya242/grounding-harness) — Hallucination Evaluation for LLM Citations
  
  - **Evaluation harness** that verifies whether each claim in an LLM answer is entailed by its cited source — turns "hallucination-free" into a single trackable number.
  - **5-type fabrication taxonomy** across 25 hand-labeled claims spanning 5 arXiv abstracts; v2 (sentence-level retrieval + NLI cross-encoder) hit **F1 = 0.811** and **100% fabrication recall (15/15)**.
  - **Repeatable regression check** with per-claim outputs and failure-mode analysis; open-sourced as a reusable eval tool.
  
  `Python` `PyTorch` `sentence-transformers` `NLI cross-encoder` `FAISS` `HuggingFace` `arXiv API`
  
  ---

  ### [`Traffic Analytics`](https://github.com/Jaya242/traffic_detector) — Real-Time Vehicle Detection & Multi-Object Tracking
  [![Live Demo](https://img.shields.io/badge/Live%20Demo-HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)](https://huggingface.co/spaces/Ctrlescflyy/traffic-analytics)
  
  - **YOLOv8-nano + ByteTrack pipeline** — real-time vehicle detection with persistent IDs across 2,208 frames.
  - **Dual-line crossing counter** with per-vehicle dedup via Python set operations — **96.2% accuracy, 100% recall** on manually annotated ground truth.
  - **End-to-end deployment** — raw video → annotated MP4 + per-event CSV log, served via Gradio on HuggingFace Spaces with a matplotlib analytics dashboard.
  
  `Python` `PyTorch` `YOLOv8` `ByteTrack` `OpenCV` `Gradio` `HuggingFace Spaces` `matplotlib`

  ---
  
  ### [`Emotion Classifier`](https://github.com/Jaya242/emotion_classifier) — Facial Emotion Recognition with GradCAM
  [![Live Demo](https://img.shields.io/badge/Live%20Demo-HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)](https://huggingface.co/spaces/Ctrlescflyy/emotion-classifier)
  
  - **ResNet18 transfer learning** — fine-tuned ImageNet-pretrained ResNet18 on FER2013 across 7 emotion classes; **68.7% test accuracy** on 7,178-image held-out split (beats published baseline of 60–65%).
  - **GradCAM interpretability layer** — heatmap overlays showing which face regions (eyes, mouth, eyebrows) drove each prediction; integrated as a toggle in the live demo.
  - **Gradio app** — webcam capture + image upload + per-class probability breakdown, deployed on HuggingFace Spaces free CPU tier with `git-lfs` for the 43MB checkpoint.
  
  `Python` `PyTorch` `ResNet18` `GradCAM` `Gradio` `HuggingFace Spaces`
  
  ---

  ## Achievements

  | | Competition | Year |
  |---|---|---|
  | 🥇 | 1st Prize — Marketing Mavericks, GTM Strategy Competition (Renaissance 2025, E-Cell MNNIT) | 2025 |
  | 🥈 | Silver Medal — Taekwondo (Spardha 2025, Annual Sports Fest, IIT BHU Varanasi) | 2025 |
  
  ---

  ## Stack
  
  
  Languages       Python  C++  C  TypeScript  JavaScript  HTML/CSS
  ML core         PyTorch  HuggingFace Transformers  DistilBERT  Transfer Learning  NumPy  Pandas
  NLP / Retrieval sentence-transformers  MiniLM (bi-encoder)  NLI cross-encoders  FAISS
  Vision          YOLOv8 (Ultralytics)  ByteTrack  OpenCV  ResNet18  GradCAM
  Deployment      Streamlit  Streamlit Community Cloud  Gradio  HuggingFace Spaces  Docker  Vercel  GitHub Releases
  Interests       Search reranking  LLM evaluation  RAG  Computer Vision  NLP  MLOps  DSA
  CP              400+ problems solved on LeetCode & CodeChef

  
  ---
  
  <sub>📫 jayaarora2402@gmail.com · [linkedin.com/in/jaya-arora-6892a93a0](https://www.linkedin.com/in/jaya-arora-6892a93a0/) · [github.com/Jaya242](https://github.com/Jaya242)</sub>

  ---
