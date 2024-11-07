## Постобработка в Photoshop. Render Elements

Рендеры можно экспортировать в Photohop послойно с помощью блока _Render Elements_: разные слои изображения сохраняются отдельными файлами.

Блок _Render Elements_ находится в верхнем левом углу _Frame Buffer_. Кроме стандартных каналов можно отдельно настроить те, которые вам нужны:

_V-Ray Asset Editor_ → _Render Elements_ → выбрать необходимые каналы в раскрывающемся списке.

![](/img/SVR_15/1686161703_1.png#birdered)  

### Настройки Render Channels

![](https://study.softculture.cc/img/SVR_15/1686161717_2.png)

1. _Material Random Color_, _MultiMatte Object_ — цветовая раскраска по различным выборкам цвета(номер материала, номер группы и т.д.) Полезна для удобного выделения в Photoshop.
2. Дополнительный настройки сцены, например: _Light Analisis_ — анализ света (выгружает плановость модели) или _Light Mix_ — выгружает все источники света.
3. Свойства материалов: _Background_/_Фон_, _GI_/ _Настройки освещения_, _Refractions_/_Отражение_, _Reflections_/_Преломление_ и т.д. — выгружает эффекты атмосферы.
4. _Diffuse_ и _Shadows_ / _Текстуры_ и _Тени_.

В этом списке можно выбрать все необходимые каналы — они отобразятся во _Frame Buffer_. Экспортировать каналы:

_Frame Buffer_ → _Save_ → _Save all Channels to Separate Files_.

Необходимый минимум каналов рендера из _Render Elements_:

- _Material_ , _Random Color_ , _Render ID_

- _Light Mix_

- _Atmosphere_

- _Diffuse_, _Matter Shadows_
