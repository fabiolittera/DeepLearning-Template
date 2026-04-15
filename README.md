<p align="center">
  <img src="assets/DL_logo.png" alt="Project Logo" width="200"/>
</p>

<h1 align="center">Nome del Progetto</h1>

<p align="center">
  <b>Corso di Deep Learning — A.A. 2025/2026</b><br>
  Università degli Studi di Cagliari
</p>

<p align="center">
  <a href="https://link-alle-slides"><img src="https://img.shields.io/badge/📊_Slides-Presentazione-blue?style=for-the-badge" alt="Slides"/></a>
  <a href="https://link-al-video"><img src="https://img.shields.io/badge/🎬_Video-Teaser-red?style=for-the-badge" alt="Video"/></a>
  <a href="https://huggingface.co/spaces/username/nome-progetto"><img src="https://img.shields.io/badge/🤗_Demo-Gradio-orange?style=for-the-badge" alt="Demo Gradio"/></a>
</p>

---

## Video Teaser

<p align="center">
  <video src="assets/video.mp4" controls width="600"></video>
</p>

---

## Requisiti

```bash
pip install -r requirements.txt
```

## Struttura del Repository

```
project-name/
├── README.md
├── requirements.txt
├── config/
│   └── config.yaml                  # Configurazione iperparametri
├── data/
│   ├── raw/                         # Dati grezzi (o link per il download)
│   └── processed/                   # ← generato da preprocessing.ipynb
├── notebooks/
│   ├── preprocessing.ipynb          # Preprocessing e analisi esplorativa → data/processed/
│   ├── experiments.ipynb            # Addestramento modelli → experiments/exp_*/
│   └── results.ipynb               # Valutazione e confronto → results/
├── experiments/
│   └── exp_YYYYMMDD_HHMMSS/        # Record di ogni esperimento
│       ├── iperparametri.json
│       ├── plot/                    # Grafici del training (loss, metriche, ...)
│       └── models/                  # Pesi dei modelli salvati
├── results/                         # ← generato da results.ipynb
│   ├── figures/
│   ├── tables/
│   └── predictions/
├── demo/
│   └── app.py                       # Demo Gradio
└── assets/
    ├── logo.png
    ├── slides.pptx
    └── video.mp4
```

## Riproduzione degli esperimenti

```bash
# 1. Clonare il repository
git clone https://github.com/[username]/[repo-name].git
cd [repo-name]

# 2. Installare le dipendenze
pip install -r requirements.txt

# 3. Eseguire i notebook in ordine
#    preprocessing.ipynb → experiments.ipynb → results.ipynb

# 5. Lanciare la demo
python demo/app.py
```

---

## Note

- Il progetto rispetta le norme dell'[ACM Code of Ethics](https://www.acm.org/code-of-ethics).
