# Music Data Mining Portfolio

Портфолио-проект по факультативу **"Вычислительное музыковедение: модели и методы Music Data Mining"**.

Репозиторий собирает пять лабораторных работ по факультативу **"Вычислительное музыковедение: модели и методы Music Data Mining"** в один законченный AI/MIR-кейс: от базовой обработки аудиосигнала до классификации жанров, нейросетевых экспериментов и генерации музыки.

## Dashboard

Открыть витрину проекта:

[docs/index.html](docs/index.html)

Dashboard показывает:

- карту всех 5 лабораторных работ;
- pipeline проекта: `audio -> features -> ML/DL -> generation`;
- ключевые датасеты и артефакты;
- интерактивное сравнение этапов, навыков и результатов.

## Project Story

Цель проекта - показать, что я умею работать с музыкальными данными как с полноценным AI-доменом:

1. Анализировать аудиосигналы и MIDI.
2. Извлекать спектральные, мел-спектральные, MFCC и openSMILE-признаки.
3. Реализовывать классические MIR-алгоритмы: pitch detection, onset detection, beat tracking.
4. Обучать модели классификации музыкальных жанров на GTZAN.
5. Проводить нейросетевые эксперименты в PyTorch и сохранять чекпоинты.
6. Исследовать генеративные модели: Pop2Piano, MusicGen, c-RNN-GAN.

## Labs

| Lab | Topic | Main Result |
| --- | --- | --- |
| [ЛР1](ВычМуз/ЛР1/lab1_signal_processing.ipynb) | Работа со звуковыми сигналами | Синтез звука, гармоники, чтение MIDI, генерация простой мелодии |
| [ЛР2](ВычМуз/ЛР2/lab2_acoustic_features_pitch_detection.ipynb) | Акустические признаки и pitch detection | Спектрограммы, mel-spectrogram, MFCC, ZCR/FFT/autocorrelation/AMDF |
| [ЛР3](ВычМуз/ЛР3/lab3_genre_classification_ml.ipynb) | Классическое ML для жанров | GTZAN, openSMILE, PCA, k-NN, Logistic Regression, SVM, Decision Tree |
| [ЛР4](ВычМуз/ЛР4/lab4_mir_systems_generation.ipynb) | MIR-системы | Onset detection, tempo estimation, beat tracking, Pop2Piano, MusicGen |
| [ЛР5](ВычМуз/ЛР5/lab5_neural_networks.ipynb) | Нейросети для музыкальных данных | PyTorch MLP, разные конфигурации сети, логирование, checkpoint-и |

## Repository Structure

```text
.
├── docs/
│   └── index.html
├── ВычМуз/
│   ├── ЛР1/
│   ├── ЛР2/
│   ├── ЛР3/
│   ├── ЛР4/
│   ├── ЛР5/
│   ├── GAN.pptx
│   ├── GAN 2.0 Денисов Илья.pptx
│   ├── GAN текст.docx
│   └── c-rnn-gan-sample11.mp3
├── requirements.txt
└── README.md
```

## Data And Artifacts

- **GTZAN**: 1000 audio tracks, 10 genres, 30 seconds per track, 22050 Hz mono audio.
- **Feature cache**: `ВычМуз/ЛР3/smile_features.npy`.
- **Neural checkpoints**: `ВычМуз/ЛР5/models/basic.pth`, `ВычМуз/ЛР5/models/batch_size8.pth`.
- **Generated MIDI**: `ВычМуз/ЛР4/composers/midi_result1.mid` ... `midi_result21.mid`.
- **Audio examples**: piano, violin, flute, vocal and generated c-RNN-GAN sample.

## Tech Stack

Python, NumPy, pandas, matplotlib, librosa, openSMILE, scikit-learn, PyTorch, torchmetrics, Hugging Face `datasets`, transformers, Comet ML.

## Why This Fits An AI Portfolio

Проект показывает полный цикл работы с неструктурированными данными:

- обработка временных рядов и аудио;
- feature engineering;
- supervised learning;
- dimensionality reduction;
- метрики качества и confusion matrix;
- deep learning experiments;
- генеративные модели для музыки.


