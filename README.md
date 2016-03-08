reformagkh
==========

##Что это?
* Скрипт-граббер для сайта Реформа ЖКХ (http://www.reformagkh.ru), сохраняет данные в формате CSV.
* Данные выкачанные для Москвы в 2014 и 2016 (32 тыс. домов).

##Как запускать

1. Находим идентификатор региона, который нужно скачать. Может быть любой из уровней, скачиваться будут в т.ч. все подуровни.
2. Убеждаемся, что рядом со скриптом присутствует файл atd.csv (его можно либо скачать тут же, либо сделать самому запустив другой скрипт `get_reformagkh_atd.py`)
3. Запускаем скрипт.

ND: Для работы скрипта, кроме Python 2.7.x нужен модуль ![progressbar](https://pypi.python.org/pypi/progressbar)

```bash
pip install progressbar
```

```bash
python get_reformagkh_data-v2.py 2280999 data/housedata.csv -o html
```

![Example3](/img/running.png)

##Таблица с результатами (фрагмент)
![Example1](/img/table.png)

##Веб-карта с результатами
Демо: http://demo.nextgis.ru/ngw/resource/243/display
![Example2](/img/map.png)

##Caveats

* Пока поддерживаются не все параметры представленные на основном сайте
