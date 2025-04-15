# Распознавание болезней культурных растений с помощью AutoML

## Описание проекта

Данный проект посвящен автоматизации распознавания болезней культурных растений с помощью AutoML-фреймворков. Целью исследования является сравнение производительности моделей, созданных с помощью AutoKeras, lightAutoML, кастомной модели и кастомной модели с использованием Keras-tuner на задаче классификации изображений растений по состоянию их листьев.

Проект включает:
* Предобработку данных из изображений или формата .npz.
* Обучение моделей с использованием AutoML-фреймворков и кастомных подходов.
* Сравнение точности предсказаний различных моделей.

## Используемые инструменты

* Python 3.8+
* AutoKeras
* lightAutoML
* TensorFlow
* Scikit-learn
* OpenCV

## Данные 

Данные представляют собой изображения листьев растений, разделенные на 4 категории:
* Blight
* Common Rust
* Gray Leaf Spot
* Healthy

Данные могут быть предоставлены в двух форматах:
* Папка с изображениями, разделенными по категориям.
* Архивированный файл .npz с предварительно обработанными массивами.

Данные, которые использовались для проекта: [Corn or Maize Leaf Disease Dataset](https://www.kaggle.com/datasets/smaranjitghose/corn-or-maize-leaf-disease-dataset).

## Установка 

1. Клонируйте репозиторий: 

```
git clone https://github.com/Gennod/kursovaya.git cd ваш-репозиторий
```

2. Установите зависимости:

```
pip install -r requirements.txt
```

## Запуск

Обработанные данные:

* small (64x64) https://drive.google.com/file/d/1gAc3R9iSRGME9scB2aCj3FkWK52fjYTt/view?usp=sharing
* medium (128x128) https://drive.google.com/file/d/1VrMftJvF3VuUt-k3yNPCChR9qi0GcKKe/view?usp=sharing
* big (255*255) https://drive.google.com/file/d/1G2iGRaYnffXltUB-Fh-L5Z5sL2we3zeZ/view?usp=sharing

### Тестирование модели

Запустите файл test_models.py:

```
python test_models.py
```

Скрипт выполнит следующие шаги:
* Загрузит и обработает данные.
* Протестирует кастомную модель.
* Выведет результаты сравнения точности моделей.

## Остальные модели

Keras-Tuner: https://drive.google.com/file/d/1OKa9gNoVn49RMHALE177Fl4FNjcbGk1_/view?usp=sharing
lightAutoML: https://drive.google.com/file/d/1zvizShFlmKLG5DOxI37M4o84A1vpTCnX/view?usp=sharing
AutoKeras: https://drive.google.com/file/d/1apgBqN9Uls9yqxdG0v14q416j3Ods0n4/view?usp=sharing

## Структура проекта


```
├── data/                           # Папка с данными
├── models/                         # Сохраненные модели и пайплайны
│   ├── corn_disease_classifier.keras
├── code/
│   ├── requirements.txt            # Зависимости проекта
│   ├── test_models.py              # Основной скрипт для тестирования
│   ├── notebook.ipynb              # Google Colab ноутбук
└── README.md                       # Описание проекта
```

## Автор

* Студент группы 23ПМИ(м)ГОГИИ Бледнов Иван Андреевич
