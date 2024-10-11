# Описание проекта
Проект посвящен решеню задачи предсказания цен на машины
https://www.kaggle.com/datasets/vijayaadithyanvg/car-price-predictionused-cars?resource=download

# Запуск
Для запуска проекта необходимо выполнить команды:
```
git clone https://github.com/Egor14112001/IIS_Lr_1
cd IIS_Lr_1
установка окружения - python -m venv .venv_proj
активация окружения - .venv_proj/scripts/Activate
установка зависимостей - pip install -r requirements.txt
```

# Исследование данных
В ходе исследования были проведены действия:
 * Очистка данных не производилась, так как после проверки все данные оказались валидын
 * Был создан новый признак - 'Driven_run' - уровень пробега автомобиля
 * Для столбцов 'Driven_kms', 'Year' изменен тип данных на int32
Закономерности, выявлены по графикам, которые могут быть полезны в дальнейшем для решния задачи:
 * В основном машины меньшего года выпуска стоят дешевле.
 * Дизельные автомобили стоят в основном дороже, что соответсвует правде.
 * Были продемонстрированы более дорогие модели машин.
 * Был сделан вывод, что машины с салона стоят дороже, чем с рук.
 * Стоимосить машины больше всего коррелирует с годом выпуска.

Обработанная выборка сохранена в файл `./data/clean_data.pkl`