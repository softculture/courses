## Создание карты функционального зонирования. Landuse

Файлы для занятия находятся в архиве `Файлы для занятий.zip` в конце оглавления курса. Для работы используйте слой `landuse-polygon.shp` из папки `Basemap/RU-MOW-510738-20180718-ru`.

Готовый запрос для выборки дополнительных категорий Landuse:  
"AMENITY" IN ('college','education','hospital','kindergarten','school','university') OR "LEISURE"='park'

Текст запроса для калькулятора полей:  
CASE  
WHEN "AMENITY" IS 'school' THEN 'Education'  
WHEN "AMENITY" IS 'college' THEN 'Education'  
WHEN "AMENITY" IS 'university' THEN 'Education'  
WHEN "AMENITY" IS 'kindergarten' THEN 'Education'  
WHEN "AMENITY" IS 'hospital' THEN 'Hospital'  
WHEN "LEISURE" IS 'garden' THEN 'Green area'  
WHEN "LEISURE" IS 'park' THEN 'Green area'  
ELSE 'Others'  
END

[video](https://player.softculture.cc/embed/online/GIS/GIS_10.10.12_L3-6_Landuse)