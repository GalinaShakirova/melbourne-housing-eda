# Melbourne Housing Market - Exploratory Data Analysis

Разведочный анализ рынка недвижимости Мельбурна: цены, типы жилья, география, временные тренды продаж 2016–2017.

📊 **[Открыть ноутбук в nbviewer](https://nbviewer.org/github/GalinaShakirova/melbourne-housing-eda/blob/main/notebooks/melbourne-housing-market-eda.ipynb)**
— рекомендую этот путь для просмотра ноутбука.

🗺️ **[Открыть интерактивную карту районов Мельбурна](https://raw.githack.com/GalinaShakirova/melbourne-housing-eda/main/reports/maps/melbourne_suburbs_map.html)**
— folium-карта с распределением цен по районам и кластерами объектов недвижимости.

## Что внутри

- Распределение сделок по времени, дням недели, месяцам
- Анализ типов недвижимости (house / unit / townhouse)
- Связь цены с количеством комнат, площадью, расстоянием до центра
- Анализ площади недвижимости и прилегающей территории
- Анализ территориального расположения проданных объектов недвижимости
- География цен: интерактивная карта районов (folium + GeoJSON)
- Анализ метода продажи и риэлторов
- Анализ года постройки недвижимости и его влияние на стоимость

## Стек

`pandas`, `numpy`, `matplotlib`, `seaborn`, `folium`

## Данные

- `train.csv`, `test.csv` — из соревнования
  [Leopard Challenge: Regression](https://www.kaggle.com/competitions/leopard-challenge-regression)
  на Kaggle. В репо не коммитятся, нужно скачать самостоятельно и положить в `data/`.
- `data/geo/Melbourn_suburb.json` — границы районов Мельбурна (GeoJSON, упрощённый)
- `data/geo/australian_postcodes.json` — координаты по почтовым индексам
  (источник: [matthewproctor.com](https://www.matthewproctor.com/australian_postcodes))

## Запуск

Python 3.12, зависимости в `requirements.txt`. Данные нужно скачать с Kaggle
(см. раздел «Данные» выше) и положить `train.csv` и `test.csv` в `data/`.

```
