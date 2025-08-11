# Решение для хакатона по детекции объектов (людей) с использованием RT-DETR

Этот репозиторий содержит решение для задачи по обнаружению людей на изображениях. В качестве основной модели используется **RT-DETR (Real-Time DEtection TRansformer)**, реализованная через фреймворк Ultralytics.

![Пример работы модели](https://github.com/user-attachments/assets/742f3368-d442-4e76-b38a-84cd034a63ab )

---

## 🛠️ Стек технологий

*   **Python 3.9+**
*   **PyTorch** — основная библиотека для глубокого обучения.
*   **Ultralytics** — фреймворк для запуска и обучения моделей, включая RT-DETR.
*   **OpenCV** — для обработки изображений.
*   **NumPy / Pandas** — для работы с данными.

---

## 📂 Структура проекта
.
├── data/                     # Папка для данных (не отслеживается Git)
│   ├── train/
│   └── test/
├── data_preparation/         # Скрипты для подготовки данных
│   └── prepare_data.py
├── training/                 # Скрипты для обучения
│   └── train.py
├── inference/                # Скрипты для инференса
│   └── inference.py
├── weights/                  # Папка для весов модели (например, best.pt)
├── requirements.txt          # Список зависимостей
└── README.md                 

---

## 🚀 Инструкция по запуску

### 1. Клонирование репозитория

```bash
git clone https://github.com/ВАШ_НИК/hackathon-object-detection.git
cd hackathon-object-detection

### 2. Установка зависимостей
# Создание виртуального окружения (опционально, но рекомендуется )
python -m venv venv
source venv/bin/activate  # Для Windows: venv\Scripts\activate

# Установка необходимых библиотек
pip install -r requirements.txt


### 3. Подготовка данных
python data_preparation/prepare_data.py


### 4. Обучение модели
python training/train.py

### 5. Инференс модели
python inference/inference.py


