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


## 🚀 Инструкция по запуску

### 1. Клонирование репозитория
git clone https://github.com/Fiseldisel/hackathon-object-detection.git
cd hackathon-object-detection

# Установка необходимых библиотек
pip install -r requirements.txt


### 3. Подготовка данных
python data_preparation/prepare_data.py


### 4. Обучение модели
python training/train.py

### 5. Инференс модели
python inference/inference.py


