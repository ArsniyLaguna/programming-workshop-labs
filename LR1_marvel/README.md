# Лабораторная работа № 1 — Marvel

Основной файл работы — [`LR1_marvel.ipynb`](LR1_marvel.ipynb). Исходные данные — [`marvel.csv`](marvel.csv). Ноутбук выполняет постановку задачи, первичный анализ данных и разделение на обучение и тест. При запуске он создаёт четыре CSV-файла в каталоге `splits/`.

## Запуск на macOS и Linux

Требуется Python 3.12.5. Из каталога проекта:

```bash
python3.12 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m ipykernel install --user --name lr1-marvel --display-name "Python (LR1 Marvel)"
jupyter lab
```

В Jupyter выберите ядро `Python (LR1 Marvel)` и запустите ячейки сверху вниз.

## Запуск на Windows

```powershell
py -3.12 -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
.\.venv\Scripts\python.exe -m ipykernel install --user --name lr1-marvel --display-name "Python (LR1 Marvel)"
.\.venv\Scripts\python.exe -m jupyterlab
```

## Данные и ограничения

Файл `marvel.csv` предоставлен в материалах задания. Его структура соответствует [UCI Energy Efficiency](https://archive.ics.uci.edu/dataset/242/energy+efficiency), но учебная копия содержит пропуски и изменённые названия двух столбцов. Единицы измерения нагрузок в предоставленных метаданных не указаны. Разделение в этом варианте лабораторной — случайное, 80/20 с `random_state=42`; близкие конфигурации могут попасть в обе части. Проверка качества на новых типах зданий потребует отдельного эксперимента.

Имя участника в ноутбуке оставлено для заполнения студентом.
