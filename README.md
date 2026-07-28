# Music Data Mining Portfolio

![Music Data Mining project overview](docs/assets/portfolio-overview.svg)

Портфолио-проект по факультативу **"Вычислительное музыковедение: модели и методы Music Data Mining"**.

Репозиторий собирает пять тематических разделов в один законченный AI/MIR-кейс: от озвучки нот и базовой обработки аудиосигнала до классификации жанров, нейросетевых экспериментов и генерации музыки.

**Витрина:** [ilyadenisov88.github.io/MIR_music_data_mining](https://ilyadenisov88.github.io/MIR_music_data_mining/)  
Если страница еще не открывается, нужно включить GitHub Pages: `Settings -> Pages -> Deploy from a branch -> main / docs`.

## Витрина

Витрина проекта устроена как медиагалерея по разделам:

- **Раздел 1:** воспроизведение музыки и визуализация сигналов: WAV, C-E-G, гармоники, MIDI.
- **Раздел 2:** акустические признаки и pitch detection: спектрограммы, MFCC, ZCR, FFT, AMDF и итоговые оценки pitch для piano/violin/flute.
- **Раздел 3:** классификация жанров GTZAN через openSMILE, PCA, SVM, Logistic Regression и Decision Tree.
- **Раздел 4:** MIR-система: onset detection, tempo estimation, beat tracking, транскрипция и генерация.
- **Раздел 5:** нейросетевая классификация жанров на PyTorch с графиками обучения и confusion matrix.

## История проекта

Цель проекта - показать, что я умею работать с музыкальными данными как с полноценным AI-доменом:

1. Анализировать аудиосигналы и MIDI.
2. Извлекать спектральные, мел-спектральные, MFCC и openSMILE-признаки.
3. Реализовывать классические MIR-алгоритмы: pitch detection, onset detection, beat tracking.
4. Обучать модели классификации музыкальных жанров на GTZAN.
5. Проводить нейросетевые эксперименты в PyTorch и сохранять чекпоинты.
6. Исследовать генеративные модели: Pop2Piano, MusicGen, c-RNN-GAN.

## Разделы

| Раздел | Тема | Что показано |
| --- | --- | --- |
| Раздел 1 | Работа со звуковыми сигналами | Синтез звука, гармоники, чтение MIDI, генерация простой мелодии |
| Раздел 2 | Акустические признаки и pitch detection | Спектрограммы, mel-spectrogram, MFCC, ZCR/FFT/autocorrelation/AMDF |
| Раздел 3 | Классическое ML для жанров | GTZAN, openSMILE, PCA, k-NN, Logistic Regression, SVM, Decision Tree |
| Раздел 4 | MIR-системы | Onset detection, tempo estimation, beat tracking, Pop2Piano, MusicGen |
| Раздел 5 | Нейросети для музыкальных данных | PyTorch, графики обучения, метрики, confusion matrix, checkpoint-и |

## Главное

- **Полный AI-пайплайн:** обработка сигнала, признаки, feature engineering, supervised learning, нейросети и генерация.
- **Медиавитрина:** синтез нот, графики из расчетов, аудиоартефакты и примеры сгенерированной музыки.
- **Датасет:** GTZAN, 1000 треков, 10 жанров, по 30 секунд, 22050 Hz mono WAV.
- **Извлечение признаков:** спектрограммы, mel-spectrogram, MFCC и openSMILE descriptors.
- **Классическое ML:** k-NN, Logistic Regression, SVM, Decision Tree и эксперименты с PCA.
- **Нейросети:** PyTorch-модели, метрики, confusion matrix и сохраненные checkpoint-и.
- **Генерация:** Pop2Piano, MusicGen и c-RNN-GAN.

## Структура

```text
.
├── docs/
│   ├── assets/
│   │   ├── audio/
│   │   ├── images/
│   │   └── portfolio-overview.svg
│   └── index.html
├── _sources/
│   └── ВычМуз/
│       └── исходные ноутбуки, MIDI, аудио, checkpoint-и и материалы презентаций
├── requirements.txt
└── README.md
```

## Данные и артефакты

- **GTZAN:** 1000 аудиотреков, 10 жанров, по 30 секунд, 22050 Hz mono WAV.
- **Кэш признаков:** openSMILE descriptors для классификации жанров.
- **Checkpoint-и:** сохраненные PyTorch-модели из нейросетевых экспериментов.
- **Generated MIDI:** MIDI-фрагменты из экспериментов с генерацией.
- **Audio examples:** piano, C-E-G, гармоники, MIDI-мелодия, violin, flute, vocal и c-RNN-GAN.

## Стек

Python, NumPy, pandas, matplotlib, librosa, openSMILE, scikit-learn, PyTorch, torchmetrics, Hugging Face `datasets`, transformers, Comet ML.

## Как смотреть

Репозиторий удобно смотреть в двух режимах:

1. **GitHub Pages** - основная витрина для проверяющего: аудио, графики и краткая логика разделов.
2. **GitHub README** - быстрый обзор проекта и контекст.

Исходные ноутбуки лежат в `_sources/ВычМуз/` как материалы проекта, но основной сценарий просмотра - живая витрина.

Чтобы включить витрину на GitHub:

1. Открыть настройки репозитория.
2. Перейти в `Pages`.
3. Выбрать `Deploy from a branch`.
4. Указать ветку `main` и папку `/docs`.
5. Открыть `https://ilyadenisov88.github.io/MIR_music_data_mining/`.

## Почему это AI-портфолио

Проект показывает полный цикл работы с неструктурированными данными:

- обработка временных рядов и аудио;
- feature engineering;
- supervised learning;
- dimensionality reduction;
- метрики качества и confusion matrix;
- deep learning experiments;
- генеративные модели для музыки.
