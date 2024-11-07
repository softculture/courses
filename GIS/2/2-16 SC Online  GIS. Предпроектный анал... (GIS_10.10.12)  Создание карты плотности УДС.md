## Создание карты плотности УДС

Файлы для занятия находятся в материалах для прохождения курса. Для работы используйте слой автодорог из папки `Basemap/RU-MOW-510738-20180718-ru`  и слой с кварталами из папки `Basemap`.

Формула для выборки дорог:

`“HIGHWAY” IN ('living\_street', 'primary', 'residential', 'secondary', 'tertiary', 'unclassified')`

Расчёт длины дорог согласно типу:

`if (“calc\_type” = 'ext', $length\*0.5, $length)`

Расчёт плотности УДС:

`( "Lcalc\_sum" \*0.001)/($area\*0.000001)`

[video](https://player.softculture.cc/embed/online/GIS/GIS_10.10.12_L2-14_Road_Network)