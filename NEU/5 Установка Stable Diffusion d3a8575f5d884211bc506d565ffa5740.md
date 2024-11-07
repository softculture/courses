# Установка Stable Diffusion

### Список устанавливаемых программ и файлов

1. Stable Diffusion от AUTOMATIC 1111 — веб-интерфейс для работы с нейросетью SD / Stable Diffusion, версия от AUTOMATIC 1111
2. Дополнительная настройка Stable Diffusion
3. Кастомные модели Stable Diffusion
4. Модели LoRA
5. Расширение ControlNet
6. Расширение Photopea
7. Модели Embedding
8. Расширение Ultimate SD Upscale
9. Tiled Diffusion / multidiffusion
10. Дополнительные апскейлеры

### Требования к компьютеру

1. ОС Windows 7,8,10,11 / Mac OS 11.0 +
2. Процессор 4-х ядерный Intel / AMD, поддерживаются также Apple (M1, M2, M3)
3. Оперативная память не менее 8 ГБ
4. Для быстрой и эффективной генерации рекомендуется иметь видеокарту NVIDIA GTX1650 и выше
5. На установку всех компонентов понадобится около 40 ГБ дискового пространства
6. Скорость установки Stable Diffusion напрямую зависит от скорости и стабильности интернет соединения. Время установки Stable Diffusion занимает от 10 мин и выше.

### Stable Diffusion от AUTOMATIC 1111. Установка на Windows

Если вы работайте на Windows, то мы рекомендуем сперва попробовать поставить портативную версию Stable Diffusion, которая уже включает в себя все необходимые компоненты и не требует от пользователя большого количества действий.

1. Перейдите по ссылке: [serpotapov/stable-diffusion-portable](https://github.com/serpotapov/stable-diffusion-portable).
2. На странице нажмите на ссылку *Stable Diffusion Portable*. Откроется окно, в котором необходимо выбрать место для загрузки архива.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXeVX85DpA6ffrRZ6JFKILs2H2hOo4vO4Yd-bkBzlFhVPqFiONcavC_dP_XnF-X2AgCNCHPAbpaWiLrStJboSiqlLWjRkODfV39jPrH6HMOzMqYC8t1-2c2R-XXqdvIo46zWyhmjFfNgRFHmhuhbIC6vYlmy?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeVX85DpA6ffrRZ6JFKILs2H2hOo4vO4Yd-bkBzlFhVPqFiONcavC_dP_XnF-X2AgCNCHPAbpaWiLrStJboSiqlLWjRkODfV39jPrH6HMOzMqYC8t1-2c2R-XXqdvIo46zWyhmjFfNgRFHmhuhbIC6vYlmy?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. Далее скачанный архив необходимо распаковать. Распаковывать архив необходимо в корень диска, чтобы избежать кириллических символов в адресе к папке. Если у вас на компьютере есть два диска, то распаковывать архив лучше на диск, где ==не установлена== операционная система. Для распаковки зайдите внутрь архива и переместите папку `stable-diffusion-portable-main` в корень соответствующего диска. Избегайте задвоения папок, например: `E:\stable-diffusion-portable-main\stable-diffusion-portable-main`.
    
    Адрес должен получиться таким: `E:\stable-diffusion-portable-main`.
    
    [https://lh7-rt.googleusercontent.com/docsz/AD_4nXdnKqMZFLcYURWXafcH7mCI1Fl-5hDdeqXkOMUqAGQ9mUNPFondJUhqmhr7yoPJLlnoZmkWN9WGS7Vma1QKRtOyyqA56AnBSFNBbpyFXJm2MrkEQwTWZjQbkvVnNCKR1W2ZvGxRrEdTkUFp_Z--_saAFaJq?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdnKqMZFLcYURWXafcH7mCI1Fl-5hDdeqXkOMUqAGQ9mUNPFondJUhqmhr7yoPJLlnoZmkWN9WGS7Vma1QKRtOyyqA56AnBSFNBbpyFXJm2MrkEQwTWZjQbkvVnNCKR1W2ZvGxRrEdTkUFp_Z--_saAFaJq?key=-Dq4uzRdwdR6YvZS5hryuQ)
    
2. Если вы распаковали все верно, то должны увидеть следующий список файлов:

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXc89sgIP8txC4lANLah2vkQopsLxSGvi2Ss7GwXZOZTZTQH2VHGDuFM2FSVKaTit6fNFejaJ2aahUvkP0dW6vVSlwDx6e-3XzZEHtTBWvogkQaAp_utyzfbmlC4-1dQ_M6IrsTXphCiaA52EZzM-QOr0Asa?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc89sgIP8txC4lANLah2vkQopsLxSGvi2Ss7GwXZOZTZTQH2VHGDuFM2FSVKaTit6fNFejaJ2aahUvkP0dW6vVSlwDx6e-3XzZEHtTBWvogkQaAp_utyzfbmlC4-1dQ_M6IrsTXphCiaA52EZzM-QOr0Asa?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. Во время установки различные антивирусные программы могут блокировать интернет-подключение и не давать устанавливать необходимые компоненты, поэтому на время установки их необходимо отключить. Далее показан пример отключения встроенного в Windows 10 антивируса:
    
    a. Нажмите на меню *Пуск* и зайдите в *Настройки*
    
    [https://lh7-rt.googleusercontent.com/docsz/AD_4nXcUPO9qkGtcVswx41HX1DJJtV4No1n00RimvYfkXah2tCvGKkgtDwgZNteynnVyochyMpZem0Ki1FnxDXNnT_j0Bmvi7dMW3Q5nqKcdvqSz52cTnINq9G7dvp4ZojGcJzBMHkV-YUTOBgEx2e9puHMZe9Kr?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcUPO9qkGtcVswx41HX1DJJtV4No1n00RimvYfkXah2tCvGKkgtDwgZNteynnVyochyMpZem0Ki1FnxDXNnT_j0Bmvi7dMW3Q5nqKcdvqSz52cTnINq9G7dvp4ZojGcJzBMHkV-YUTOBgEx2e9puHMZe9Kr?key=-Dq4uzRdwdR6YvZS5hryuQ)
    
    b. В списке выберите *Обновление и безопасность*
    
    [https://lh7-rt.googleusercontent.com/docsz/AD_4nXfbkGT7et1fA7yz3LoS7TQsx1G0byWw5pXQEvhpNlj0o8K73a4A1U5tG_AHIH6usn4cfz6YRpiM9ITa9pkFkgXMaM92x4HB7ueeNz3Ca3mkfFMPTncsVavKoPvoCkNsVq2-w54xAwu6SMDDcsHhlhHbs7U?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfbkGT7et1fA7yz3LoS7TQsx1G0byWw5pXQEvhpNlj0o8K73a4A1U5tG_AHIH6usn4cfz6YRpiM9ITa9pkFkgXMaM92x4HB7ueeNz3Ca3mkfFMPTncsVavKoPvoCkNsVq2-w54xAwu6SMDDcsHhlhHbs7U?key=-Dq4uzRdwdR6YvZS5hryuQ)
    
    c. Далее *Безопасность Windows* и *Защита от вирусов и угроз*
    
    [https://lh7-rt.googleusercontent.com/docsz/AD_4nXeMtlw1HvUgjkhDCvCoRS3yJuEIEv05-vtbT18G8nB6t4_BDTl-vgPCK-8A1X57mthLSuNR0QGt2yI8GvyRHE2_qJlwA0sZlt_Px5VOyDkBuzDo-5KKCBYxVp5QO_a0Bh--24niO8tPAw6BrdG2CaVomBI1?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeMtlw1HvUgjkhDCvCoRS3yJuEIEv05-vtbT18G8nB6t4_BDTl-vgPCK-8A1X57mthLSuNR0QGt2yI8GvyRHE2_qJlwA0sZlt_Px5VOyDkBuzDo-5KKCBYxVp5QO_a0Bh--24niO8tPAw6BrdG2CaVomBI1?key=-Dq4uzRdwdR6YvZS5hryuQ)
    
    d. В появившемся окне нажмите на ссылку *Управление настройками* под разделом *Параметры защиты от вирусов и других угроз*
    
    [https://lh7-rt.googleusercontent.com/docsz/AD_4nXeBDTlkcQDOJl8PntqEnXpCC5YpZlmLAcmRRKyr7EIQm6TRcXRu1dDfyDJ-CtNMIsWDJdctNJwtnSY5Askklx0SqeiJZRs73zVb1HDfpmiQkQHUB4ab91SExDAyniHescyML9_NzgR4O1z2NNNhYNbmmYPn?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeBDTlkcQDOJl8PntqEnXpCC5YpZlmLAcmRRKyr7EIQm6TRcXRu1dDfyDJ-CtNMIsWDJdctNJwtnSY5Askklx0SqeiJZRs73zVb1HDfpmiQkQHUB4ab91SExDAyniHescyML9_NzgR4O1z2NNNhYNbmmYPn?key=-Dq4uzRdwdR6YvZS5hryuQ)
    
    e. Отключите ползунок раздела *Защита в режиме реального времени*
    
    [https://lh7-rt.googleusercontent.com/docsz/AD_4nXcjMXdI1qIzz78hD3yIzDvEVPsFhYRBCM9hJuBV6OgsyN9E_AOBkWYKjRjUHHyaGg9-TEMoltYIKJODc9NekKvll0rvUulW5aOYTogL64A1InfLsHdksCP3O6GPmwn6kHPbEf2bdup-fL6o83JqJvNbgDVo?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcjMXdI1qIzz78hD3yIzDvEVPsFhYRBCM9hJuBV6OgsyN9E_AOBkWYKjRjUHHyaGg9-TEMoltYIKJODc9NekKvll0rvUulW5aOYTogL64A1InfLsHdksCP3O6GPmwn6kHPbEf2bdup-fL6o83JqJvNbgDVo?key=-Dq4uzRdwdR6YvZS5hryuQ)
    
2. После отключения антивируса вернитесь в папку `stable-diffusion-portable-main` и запустите файл `webui-user-first-run.cmd`. Этот файл запустит автоматическую развертку Stable Diffusion. Развертка происходит в окне командной строки, при этом в ней будут отображаться статусы различных этапов установок. Самое главное — пройти первый этап, при котором создаются папки и файлы. Если в этот момент у вас происходит обрыв соединения, то придется удалить папку и начать заново с пункта 3. Этот этап занимает продолжительное время, при хорошей скорости интернета и современном ПК время развертывания составляет около 10 мин.
3. Как понять закончилась ли установка? По окончанию установки будет попытка автоматического запуска веб-интерфейса Stable Diffusion со стандартными настройками. Если у вас современный ПК с современной видеокартой NVIDIA, то у вас без проблем откроется веб-интерфейс. Если у вас отсутствует видеокарта NVIDIA или она уже устаревшая, то у вас будет статичное черное окно, где последней строчкой будет написано об ошибке (error), связанной с запуском Torch. Это нормальная ситуация, для ее решения перейдите к дополнительной настройке, описанной в следующем пункте 2.
    
    При работе со Stable Diffusion у вас также будет открываться и работать в фоновом режиме командная строка. В ней будут также отображаться все статусы обработки и работы программы. Чтобы завершить работу со Stable Diffusion просто закройте командную строку. В дальнейшем запуск Stable Diffusion следует осуществлять через файл `webui-user.bat`.
    

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXcG73xaqZ9K9HmM2Qenvih-3SyrsWYm1YhSvHjn9PQByIJHeW8Hu5gSVG5YbK8el9o1Rh_sLDP6ThZQifyxosZcHRuOr6nfOLvpxONN28ScUpG-bk00SiUPb7uU4T5AF1ZVlIui4aRLoXtaqqfKYPuGVS4?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcG73xaqZ9K9HmM2Qenvih-3SyrsWYm1YhSvHjn9PQByIJHeW8Hu5gSVG5YbK8el9o1Rh_sLDP6ThZQifyxosZcHRuOr6nfOLvpxONN28ScUpG-bk00SiUPb7uU4T5AF1ZVlIui4aRLoXtaqqfKYPuGVS4?key=-Dq4uzRdwdR6YvZS5hryuQ)

### Посмотреть версию Mac OS

Посмотреть версию своей системы можно нажав в левом верхнем углу на иконку *Яблоко*, а затем *Об этом Mac*.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdvvfK9F8JwE1m5dRZY_WtDvfwvo4yMF9U_yi_dTvh44PdjIeM16TWzB1PhVZQ4Y4iaX_-EyU6K7C1o5utmIZYnYMGamsBH-BhB075SZn6AWq3x1FBMLGd-2Qw0RhMqZ9J9AXA9R03SPCyJXJzMfiFSGxtR?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdvvfK9F8JwE1m5dRZY_WtDvfwvo4yMF9U_yi_dTvh44PdjIeM16TWzB1PhVZQ4Y4iaX_-EyU6K7C1o5utmIZYnYMGamsBH-BhB075SZn6AWq3x1FBMLGd-2Qw0RhMqZ9J9AXA9R03SPCyJXJzMfiFSGxtR?key=-Dq4uzRdwdR6YvZS5hryuQ)

Появится окно с информацией о системе.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXfV5gRoWUptlrli5Dh8R5j2dyHig-Yf4ZdlOfTtiSaeCKFyM62nBJRYRBrN-LvNBtpKKr1eN1JTSerB6iPmFiy6XwSblhKl3TtXgFFTIORhu4I2nMa7DtEGmb3i7IBCIwro8LwmWapkKILSCQhW1HPakHA8?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfV5gRoWUptlrli5Dh8R5j2dyHig-Yf4ZdlOfTtiSaeCKFyM62nBJRYRBrN-LvNBtpKKr1eN1JTSerB6iPmFiy6XwSblhKl3TtXgFFTIORhu4I2nMa7DtEGmb3i7IBCIwro8LwmWapkKILSCQhW1HPakHA8?key=-Dq4uzRdwdR6YvZS5hryuQ)

### Установка на Mac OS (Big Sur 11.0 и выше)

Если вы работайте на Mac OS Big Sur или новее, то вам необходимо будет проделать ряд действий для установки различных программ и самого веб-интерфейса Stable Diffusion.

1. Сперва необходимо запустить встроенную в mac OS командную строку, она называется *Терминал /* *Terminal*. Это можно сделать через Spotlight. Для этого нажмите сочетание клавиш **Command (Cmd) + Shift**, либо нажмите на иконку «Лупа» сверху справа и введите в строке «**Terminal**».

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXex_Ro6DsTtrCes_JN4r0hHhZHLh3HSE908KXIkvbuTHYBmVwqmmQJj_VQKSIJpxQfZ8DFOjhuSDC8mBtk6GA0tB5_YlE5o8nSnzPw2ci9p7DvlhBEl8rQl5ald2oLxLO2VKVyDtscd1_xZZWamIeqAnks1?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXex_Ro6DsTtrCes_JN4r0hHhZHLh3HSE908KXIkvbuTHYBmVwqmmQJj_VQKSIJpxQfZ8DFOjhuSDC8mBtk6GA0tB5_YlE5o8nSnzPw2ci9p7DvlhBEl8rQl5ald2oLxLO2VKVyDtscd1_xZZWamIeqAnks1?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. Теперь запустите браузер, например, Safari и введите в адресной строке - [https://brew.sh/](https://brew.sh/)

Этот сайт позволяет установить пакетный менеджер Homebrew, который в свою очередь поможет в автоматическом режиме скачать и установить весь необходимый софт.

Нажмите на иконку «**Скопировать**» справа от строки с командой.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXfRjqHYU9nmmuISH0XP4OL9aA9SlbNriw3bzwvuCWjGTzvQgOk0HK9HBl1mXiLdxLtvCYk_EEbm6j2oTUZ-1_o81GV0mqMNrNF1ZEQC7fzDHCYPPOsQQUTRAVWa3G_Sj81aWzmpP7dTr1ITUxf0aWtXITY?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfRjqHYU9nmmuISH0XP4OL9aA9SlbNriw3bzwvuCWjGTzvQgOk0HK9HBl1mXiLdxLtvCYk_EEbm6j2oTUZ-1_o81GV0mqMNrNF1ZEQC7fzDHCYPPOsQQUTRAVWa3G_Sj81aWzmpP7dTr1ITUxf0aWtXITY?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. Вернитесь в «Терминал» и вставьте скопированную с сайта команду. Просто нажмите правой кнопкой мыши по черному фону «Терминала» и в появившемся меню выберите пункт «**Вставить**» (**Paste**).

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXcTs_vua2EQ0xlel4rmPjQYXUwR7KU2Rn19q6tRe80NBv1v-Qp_3f4NP8466Nsdj_gIseV3QPrULYG6Q_CZt4C_nsOljrlLMG1o5T3OmlfJI0DeqLIyREHlZje3K-x0pwYnvhbb3QhM5cS_TdzOn2qT-goX?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcTs_vua2EQ0xlel4rmPjQYXUwR7KU2Rn19q6tRe80NBv1v-Qp_3f4NP8466Nsdj_gIseV3QPrULYG6Q_CZt4C_nsOljrlLMG1o5T3OmlfJI0DeqLIyREHlZje3K-x0pwYnvhbb3QhM5cS_TdzOn2qT-goX?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. Когда команда успешно появится в окне «Терминала», нажмите клавишу «**Enter**»**,** чтобы ****начать ее выполнение.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXc0aWfJyXsXOPm-tf0c8wyxZSBcRo8WkIz5rOoBZ5X68K-wfK7Wxb1nplgmp3aaGbLYjHlmPRd8uY55RlPdKeoMzBsgswW1TQLm7y7uqfLtaydbp_2RCvY3aCIgipRaCUDR8tizPAQbwvk8k09OYnmTSWIi?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc0aWfJyXsXOPm-tf0c8wyxZSBcRo8WkIz5rOoBZ5X68K-wfK7Wxb1nplgmp3aaGbLYjHlmPRd8uY55RlPdKeoMzBsgswW1TQLm7y7uqfLtaydbp_2RCvY3aCIgipRaCUDR8tizPAQbwvk8k09OYnmTSWIi?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. После нажатия на клавишу «Enter» появится сообщение с просьбой ввести пароль от учетной записи администратора. Соответственно это тот пароль, который вы вводите для входа в систему. Введите пароль и повторно нажмите «**Enter**», если пароля нет, то сразу «**Enter**».

(*Внимание! В целях безопасности «Терминал» не отображает символы при вводе пароля, тем ни менее считывает их. Поэтому не обращайте внимание, что при вводе символов, они не появляются на экране*)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdepwR2b1cRKVDJRBTy-SAo57wXyHFA2f5x2ED1ediDTbG87BMeKlmXAV6FyQl_0VeSEbaRvvDBqNa1r0HceAQMdpSNTJambM-I5fIBdSL07WGWO1zFaN8y5VaPVI_Pkarf23eEJAKlNE9sODuNtuuuBRI?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdepwR2b1cRKVDJRBTy-SAo57wXyHFA2f5x2ED1ediDTbG87BMeKlmXAV6FyQl_0VeSEbaRvvDBqNa1r0HceAQMdpSNTJambM-I5fIBdSL07WGWO1zFaN8y5VaPVI_Pkarf23eEJAKlNE9sODuNtuuuBRI?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. Когда пароль успешно введен, появится сообщение с информацией о том, какие скрипты будут установлены в процессе. Последней строкой будет сообщение: «*Нажмите клавишу «Enter», чтобы продолжить, либо любую другую клавишу для отмены*». Соответственно, необходимо еще раз нажать клавишу «**Enter**».
2. Дождитесь окончания установки всех компонентов. Об этом будет свидетельствовать курсор (вертикальная линия) на строке: *имя_пользователя@имя_вашего_мака ~ %*

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXe4djeeRIX9HYDmxQcI6Zq8vaEBsRbwWPWRYvZ6eBHQacCB3cYpFbPHHogB7LI8dSDXsu4hg1I8UZTP5Ci8PbthOf7DKMyu7KfFelqx1PBvTBzIAl0A6kYf7_x1vcU80fadvqAUi_LypzvuDQrU-6INVqHi?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe4djeeRIX9HYDmxQcI6Zq8vaEBsRbwWPWRYvZ6eBHQacCB3cYpFbPHHogB7LI8dSDXsu4hg1I8UZTP5Ci8PbthOf7DKMyu7KfFelqx1PBvTBzIAl0A6kYf7_x1vcU80fadvqAUi_LypzvuDQrU-6INVqHi?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. Выше последней строки будет раздел «**Next steps:**». В этом разделе будут написаны две команды. Вам необходимо выделить их курсором и с помощью сочетаний клавиш **Ctrl** + **C** / **Ctrl** + **V** (**Скопировать** / **Вставить**) эти команды в нижнюю строку и нажать «**Enter**». Теперь мы сможем напрямую обращаться через «Терминал» к программе «Homebrew».

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXd9_6EdJHydklbfNgtZqopK4q7Z0QAEM5kuwbeBSVuF5aGuwwsJmYwzpgtVhXjQW1DGRloEpsJt611RbOL5QmriYkhw1fGv9k7ximXOaQCCoGDRivqH_E1GPiBTvjSJ9aKw59nhj9rvAz-GHfubgbbsQ3nq?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd9_6EdJHydklbfNgtZqopK4q7Z0QAEM5kuwbeBSVuF5aGuwwsJmYwzpgtVhXjQW1DGRloEpsJt611RbOL5QmriYkhw1fGv9k7ximXOaQCCoGDRivqH_E1GPiBTvjSJ9aKw59nhj9rvAz-GHfubgbbsQ3nq?key=-Dq4uzRdwdR6YvZS5hryuQ)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXcRkWwpxqecuLyFJXH9ScovXL_iSUeR0GpTVKuE9sv7tiKd52xTtgInD5bWTwOIqoJE3P7aQxnjc17xDKRk9k5IXsP66bLKwRC6DyBC_Uo3Nw3y2F4RGIjcUQgZgYOBRqAue8xhNSvTLgIUdDJ329BugJU?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcRkWwpxqecuLyFJXH9ScovXL_iSUeR0GpTVKuE9sv7tiKd52xTtgInD5bWTwOIqoJE3P7aQxnjc17xDKRk9k5IXsP66bLKwRC6DyBC_Uo3Nw3y2F4RGIjcUQgZgYOBRqAue8xhNSvTLgIUdDJ329BugJU?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. После успешной установки пакетного менеджера «Homebrew», воспользуемся им для установки необходимых нам программ. Для этого скопируйте и вставьте команду ниже в «Терминал» и нажмите «**Enter**».

brew install cmake protobuf rust python@3.10 git wget

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXfg40V4uvzxuurAK4bjpY0WhkikwPk3oLaz1KiJkTIh2Tlrz3EJTRrLnslQJYU3SELbn_pVYZVL75ke_IZNcCdJVJXHO_PHbGX2pbeeh-PeZCC1M3aseLQD9PfXanNHxylfA9TU3V8Ja2MvMJMMhVMoYh3b?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfg40V4uvzxuurAK4bjpY0WhkikwPk3oLaz1KiJkTIh2Tlrz3EJTRrLnslQJYU3SELbn_pVYZVL75ke_IZNcCdJVJXHO_PHbGX2pbeeh-PeZCC1M3aseLQD9PfXanNHxylfA9TU3V8Ja2MvMJMMhVMoYh3b?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. Дождитесь окончания установки всех компонентов.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXev0XRDE26h02zdFjD6s8HQ_vTl4dDAVBWSQArd3wnuAigHY8ZYAyG2unuO0Q7auJGyx0HFlV99qXDk-FLcyy1TwP_RW2RHqA1c7JUncXcSL4rR-ZeYK2QipEMg80ad4IAStB240rn9KZ1KmNnQyu5N9TY?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXev0XRDE26h02zdFjD6s8HQ_vTl4dDAVBWSQArd3wnuAigHY8ZYAyG2unuO0Q7auJGyx0HFlV99qXDk-FLcyy1TwP_RW2RHqA1c7JUncXcSL4rR-ZeYK2QipEMg80ad4IAStB240rn9KZ1KmNnQyu5N9TY?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. После окончания установки компонентов необходимо скачать веб-интерфейс Stable-Diffusion. Для этого скопируйте и вставьте команду ниже в «Терминал» и нажмите «**Enter**».

git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXcsnhu7Myun_S10KY5feZqqA8-5JoOYu1Q86pSWlQCACgCgLz_650yjpYWO3NkkYL-IxSNmIN8mmeMbyG0crHwBp6pwPGcKCsDLitD9QCbS4HIycM4rAe4CWnCxVeMQ_MzWFcuJWFReZoxfzTcMQD680m5k?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcsnhu7Myun_S10KY5feZqqA8-5JoOYu1Q86pSWlQCACgCgLz_650yjpYWO3NkkYL-IxSNmIN8mmeMbyG0crHwBp6pwPGcKCsDLitD9QCbS4HIycM4rAe4CWnCxVeMQ_MzWFcuJWFReZoxfzTcMQD680m5k?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. После окончания установки Stable-Diffusion введите следующую команду, чтобы открыть папку.
2. Для этого скопируйте и вставьте команду ниже в «Терминал» и нажмите «**Enter**».

open .

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXenxXHytQqiKPsQaghX9tDcUhmBSgU1LsHLfYRuqShWw_DlIpt077LtRuYHwHvt6W3HRLFd7IRhahN_eRVj6v9y_q_hCVTPsB-8kvOHqqygN0ZBtOU7nv4hOP2Bq_YNGZgP7AHBLbxlcblsOe0YzSuWH4o?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXenxXHytQqiKPsQaghX9tDcUhmBSgU1LsHLfYRuqShWw_DlIpt077LtRuYHwHvt6W3HRLFd7IRhahN_eRVj6v9y_q_hCVTPsB-8kvOHqqygN0ZBtOU7nv4hOP2Bq_YNGZgP7AHBLbxlcblsOe0YzSuWH4o?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. В открывшемся окне найдите папку «**stable-diffusion-webui**» и откройте ее.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXc6Y7__jquaVm4UPUmQNmOk18tHrAOvS6p6Murk9L6mDl1Yrr372ktYKOCyJf4EzA5Mw7WQSC6YHEwaSmS4M8JcjHlAEa5RPTJ5WXHtkAmhvvXo91QmwA7Ztj01H2mM3Wv9mE1dlsnpAnlsGFfD4LoJD9I?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc6Y7__jquaVm4UPUmQNmOk18tHrAOvS6p6Murk9L6mDl1Yrr372ktYKOCyJf4EzA5Mw7WQSC6YHEwaSmS4M8JcjHlAEa5RPTJ5WXHtkAmhvvXo91QmwA7Ztj01H2mM3Wv9mE1dlsnpAnlsGFfD4LoJD9I?key=-Dq4uzRdwdR6YvZS5hryuQ)

В папке будут находиться те же файлы и папки, что и при установке на Windows. Поэтому дальнейшие пункты для моделей, расширений и прочего актуальны и для mac OS.

1. Введите в «Терминале» следующую команду и нажмите «**Enter**»:

cd stable-diffusion-webui

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdPgsPWXrW2b0uv62nolsbnOnCDsUbFxyhCjHlHSYsoqRDT8UfKNXaX0h7qeqyYs-z0u6Yp40L2kHgBM0RadEUCm6nSh7NpriKa8cdkwLa-3Ifzm4Awvw4-ZsPhrfeAbOEksTXsR612hyXgbTa3AgV5ag67?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdPgsPWXrW2b0uv62nolsbnOnCDsUbFxyhCjHlHSYsoqRDT8UfKNXaX0h7qeqyYs-z0u6Yp40L2kHgBM0RadEUCm6nSh7NpriKa8cdkwLa-3Ifzm4Awvw4-ZsPhrfeAbOEksTXsR612hyXgbTa3AgV5ag67?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. Введите команду ls, чтобы увидеть все папки и файлы внутри папки «**stable-diffusion-webui**».

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXcLV62Pob8dPZHtFJUmeI9cFvKwrCmetam5hnQQx1U3l4l9m3jreEBvySm4RWNcuOPwucAm3gh26wlCjmz0pBlAQXbB0kVcd9cP_dRGPOvSTgGdw_nhz5nRb10YCX-HzLuQ6GNEJaS-XuMJfNcNx9OxYU31?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcLV62Pob8dPZHtFJUmeI9cFvKwrCmetam5hnQQx1U3l4l9m3jreEBvySm4RWNcuOPwucAm3gh26wlCjmz0pBlAQXbB0kVcd9cP_dRGPOvSTgGdw_nhz5nRb10YCX-HzLuQ6GNEJaS-XuMJfNcNx9OxYU31?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. После этого введите команду для запуска веб-интерфейса Stable-Diffusion и нажмите «**Enter**»

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdiiu_a4eQhH08eKWgeIHtDlzQdXKh7fQcOKiLd0NZBxq4JtvTDETRVyM-BWNcv4iTtJmFA4xMonaocaYP-X8T1OrGhfejhE6LA6wIXjllMDzsv8HbgWjuzlRSjVGgs8XMXoL4X95LK4581WV0D5fj2Dc0y?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdiiu_a4eQhH08eKWgeIHtDlzQdXKh7fQcOKiLd0NZBxq4JtvTDETRVyM-BWNcv4iTtJmFA4xMonaocaYP-X8T1OrGhfejhE6LA6wIXjllMDzsv8HbgWjuzlRSjVGgs8XMXoL4X95LK4581WV0D5fj2Dc0y?key=-Dq4uzRdwdR6YvZS5hryuQ)

При первом запуске, команда начнет скачивание и установку необходимых для корректной работы интерфейса компонентов. (*Внимание! В зависимости от скорости вашего интернета, данный процесс может занять от нескольких минут до нескольких десятков минут*)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXfq3ZfVRfdsYxu6B6Yfh3mSq5-cEo5JHXnTB5wTyarAeGxDlvCGQ7wOYAae_z2AvEBR_up-BnxPxjHMmXjI6Eg5uFTM4RddOMRNeBls1hXEx5jG6eghSc0KqK5fbw6B0ZUxoDIKvPVKwj7HsdF2iyECPNk?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfq3ZfVRfdsYxu6B6Yfh3mSq5-cEo5JHXnTB5wTyarAeGxDlvCGQ7wOYAae_z2AvEBR_up-BnxPxjHMmXjI6Eg5uFTM4RddOMRNeBls1hXEx5jG6eghSc0KqK5fbw6B0ZUxoDIKvPVKwj7HsdF2iyECPNk?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. При успешном завершении всего, появится строка с адресом веб-интерфейса и произойдет запуск браузера. Но, если у вас статичное черное окно, где последней строчкой будет написано об ошибке (error), связанной с запуском Torch, то не пугайтесь - это нормальная ситуация, для ее решения перейдите к дополнительной настройке, описанной в следующем пункте 2.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXduKcDMK5S4pQSkAjwb2QqAvvO-RCGlaVM2GaJ9d42ZeXBOsvLm7_8rY1JDxtwah7TYvwmEzETqaLp9r3WQCni037L2NXPUBr4rygviLsKED0n2PLPoJYhqVh9O73t3UTo6c1YI3AqKUvAjqQycZFG8I3UU?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXduKcDMK5S4pQSkAjwb2QqAvvO-RCGlaVM2GaJ9d42ZeXBOsvLm7_8rY1JDxtwah7TYvwmEzETqaLp9r3WQCni037L2NXPUBr4rygviLsKED0n2PLPoJYhqVh9O73t3UTo6c1YI3AqKUvAjqQycZFG8I3UU?key=-Dq4uzRdwdR6YvZS5hryuQ)

*Внимание! Stable-Diffusion работает через консоль, поэтому не закрывайте «Терминал» пока не закончите работать с нейросетью.*

1. При дальнейшей работе со Stable-Diffusion, для запуска веб-интерфейса необходимо будет выполнять всего 2 команды в «Терминале».

cd stable-diffusion-webui

./webui.sh

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXc3o_gV3WroyuP580GQ79r0FjPjbE7-1fPdON6j8Q8T9evFapyGys_XMCsxE5yBrDrdJBUM6c9_KQGHFQG8D_ZqFEevuzK9DR_xoZz9WxHF6QmGG6s_FnAZxGgFproj-jI8EFBN3ACTVKHwcHOI9dqEDQs?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc3o_gV3WroyuP580GQ79r0FjPjbE7-1fPdON6j8Q8T9evFapyGys_XMCsxE5yBrDrdJBUM6c9_KQGHFQG8D_ZqFEevuzK9DR_xoZz9WxHF6QmGG6s_FnAZxGgFproj-jI8EFBN3ACTVKHwcHOI9dqEDQs?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. **Stable Diffusion от AUTOMATIC 1111 – установка на Mac OS (ниже Big Sur 11.0)**

К сожалению, операционные системы Mac os ниже версии Big Sur 11.0 являются устаревшими и не гарантируют работоспособность Stable Diffusion.

1. Запустите браузер, например, Safari и введите в адресной строке - [https://www.macports.org/install.php#installing](https://www.macports.org/install.php#installing)

Этот сайт позволяет скачать пакетный менеджер Macports, который в свою очередь поможет в автоматическом режиме скачать и установить весь необходимый софт. Найдите на странице раздел с инсталляционными файлами и выберите вашу систему.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXcl4ACT9PVgmgQ3ZUuxQD3qIFGA0iMZmMzwD6qwKRdAHeZvAt1q_acEZJ3nQaukEhH2QDrXj4njgpQNmc-gsxsrRJGOam49CNMCZCg7SIOAoLSObDayd7pqbShE_7lrMQh5fSQnNcgaW0md66q8Yb77wOM?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcl4ACT9PVgmgQ3ZUuxQD3qIFGA0iMZmMzwD6qwKRdAHeZvAt1q_acEZJ3nQaukEhH2QDrXj4njgpQNmc-gsxsrRJGOam49CNMCZCg7SIOAoLSObDayd7pqbShE_7lrMQh5fSQnNcgaW0md66q8Yb77wOM?key=-Dq4uzRdwdR6YvZS5hryuQ)

Это установочные файлы для mac os, после скачивания файла - запустите его и произведите установку.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdcQ37xdp7dW5TKSPWL6spzUMS0YCiUL-ykGstkE-O2Vd1yShT7NAGKTUejJz7tj2auktjGadaehx5RBOPpS6bV4FTQtH5YeTi59vpIggMxokIpk1A7nTzW8m306wepTfGUdjuCgaaWLIacuD252mwjALqm?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdcQ37xdp7dW5TKSPWL6spzUMS0YCiUL-ykGstkE-O2Vd1yShT7NAGKTUejJz7tj2auktjGadaehx5RBOPpS6bV4FTQtH5YeTi59vpIggMxokIpk1A7nTzW8m306wepTfGUdjuCgaaWLIacuD252mwjALqm?key=-Dq4uzRdwdR6YvZS5hryuQ)

В открывшемся окне прощелкайте все стадии, нажимая кнопку “**Продолжить**” (**Continue**).

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXfdBii40AVsQj7w4g0Zl7UabZf0oHjbkzi7SVXApvjH9q6HXAHmPBbDQsBuN0qFySPoUVNqp0ewm3zAZltCwLSQiFgoNpjbDBdzX5gBQcCZG5IMC-AmVHMjvumiTwD0rpuKsxWeAI9ELU2ZtsHPnByBx7wi?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfdBii40AVsQj7w4g0Zl7UabZf0oHjbkzi7SVXApvjH9q6HXAHmPBbDQsBuN0qFySPoUVNqp0ewm3zAZltCwLSQiFgoNpjbDBdzX5gBQcCZG5IMC-AmVHMjvumiTwD0rpuKsxWeAI9ELU2ZtsHPnByBx7wi?key=-Dq4uzRdwdR6YvZS5hryuQ)

На каком-то этапе надо будет согласиться с лицензионным соглашением, нажав кнопку “**Согласен**” (**Agree**).

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXfHlI5O9sTsmDIcCLB5gKTjRKRNs0WASQIZRpKrw-hgA1u51mGvjjCi1obDYvRJ4pcMIe48GbQyYS46WyFBkaDd2yxrs3hIeTCzRPB8HAAgWZGF1XYNP8HxFOK1N4-HVTka3pq1Sjwx-BJ21QTbXlYO-ry6?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfHlI5O9sTsmDIcCLB5gKTjRKRNs0WASQIZRpKrw-hgA1u51mGvjjCi1obDYvRJ4pcMIe48GbQyYS46WyFBkaDd2yxrs3hIeTCzRPB8HAAgWZGF1XYNP8HxFOK1N4-HVTka3pq1Sjwx-BJ21QTbXlYO-ry6?key=-Dq4uzRdwdR6YvZS5hryuQ)

После чего приступить к установке нажав “**Установить**” (**Install**).

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXeuy6PmVDXhG7BRvYkMfpqh4dp2x75q-x4eab9i3arH31yWhUiXl9LoRNs5Sh_lgcEd3S93Xy_WBfzF775hGKdvzv078KTih5Saz6pF2Fwe-reYgFIHUH2GDYhgfWWsdCpoKWDCq_b79Cq84Qh0412P0X9k?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeuy6PmVDXhG7BRvYkMfpqh4dp2x75q-x4eab9i3arH31yWhUiXl9LoRNs5Sh_lgcEd3S93Xy_WBfzF775hGKdvzv078KTih5Saz6pF2Fwe-reYgFIHUH2GDYhgfWWsdCpoKWDCq_b79Cq84Qh0412P0X9k?key=-Dq4uzRdwdR6YvZS5hryuQ)

Во время установки может понадобится ввести пароль и дать доступ к папке “Загрузки”.

После успешной установки, окно установщика можно будет закрыть.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdYqYn0hh5WieDZb24fR5wcc9Jemv_S02abDZqAWkZYgWg_OQd-Q2gs7At2gdWgcyD2rvYMTHiXAmkQP0gmG9xQR66Y-ipBUM03DkMASO9yQqC79k54GJnoZHW6Vf8Due6B910sw7zoOhIvNaC2J8A2rMAC?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdYqYn0hh5WieDZb24fR5wcc9Jemv_S02abDZqAWkZYgWg_OQd-Q2gs7At2gdWgcyD2rvYMTHiXAmkQP0gmG9xQR66Y-ipBUM03DkMASO9yQqC79k54GJnoZHW6Vf8Due6B910sw7zoOhIvNaC2J8A2rMAC?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. Теперь необходимо запустить встроенную в mac OS командную строку, она называется Терминал (Terminal). Это можно сделать через Spotlight. Для этого нажмите сочетание клавиш **Command (Cmd) + Shift**, либо нажмите на иконку «Лупа» сверху справа и введите в строке «**Terminal**».

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXex_Ro6DsTtrCes_JN4r0hHhZHLh3HSE908KXIkvbuTHYBmVwqmmQJj_VQKSIJpxQfZ8DFOjhuSDC8mBtk6GA0tB5_YlE5o8nSnzPw2ci9p7DvlhBEl8rQl5ald2oLxLO2VKVyDtscd1_xZZWamIeqAnks1?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXex_Ro6DsTtrCes_JN4r0hHhZHLh3HSE908KXIkvbuTHYBmVwqmmQJj_VQKSIJpxQfZ8DFOjhuSDC8mBtk6GA0tB5_YlE5o8nSnzPw2ci9p7DvlhBEl8rQl5ald2oLxLO2VKVyDtscd1_xZZWamIeqAnks1?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. В Терминале необходимо будет произвести установки различных компонентов для Stable Diffusion. Установки будут автоматическими, благодаря программе Macports, которую установили ранее.
2. Установка программы cmake, для этого введите в Терминале команду:

sudo port install cmake

После нажатия на клавишу «Enter» появится сообщение с просьбой ввести пароль от учетной записи администратора. Соответственно это тот пароль, который вы вводите для входа в систему. Введите пароль и повторно нажмите «**Enter**», если пароль не задан, то сразу «**Enter**».

(*Внимание! В целях безопасности «Терминал» не отображает символы при вводе пароля, тем ни менее считывает их. Поэтому не обращайте внимание, что при вводе символов, они не появляются на экране*)

Для некоторых программ требуется установка дополнительного софта, об этом может быть написано в окне. При этом будет следующая строчка “**Продолжить? Да/нет**” (**Continue? Y/n**). Необходимо будет ввести **Y** и нажать клавишу “Enter”.

Когда в Терминале появится строчка, где будет просто **имя_вашего_пользователя@имя_мака ~ %**, то это будет означать готовность системы для ввода новой команды.

1. Установка программы nasm, для этого введите в Терминале команду:

sudo port install nasm

1. Установка программы jdk17, для этого введите в Терминале команду:

sudo port install jdk17

1. Установка программы ninja, для этого введите в Терминале команду:

sudo port install ninja

1. Установка программы rust, для этого введите в Терминале команду:

sudo port install rust

1. Установка программы git, для этого введите в Терминале команду:

sudo port install git

1. Установка программы wget, для этого введите в Терминале команду:

sudo port install wget

1. Установка программы python 3.10, для этого введите в Терминале команду:

sudo port install python310

1. Установка программы protobuf, для этого введите в Терминале команду:

sudo port install py310-protobuf3

1. После окончания установки Stable-Diffusion необходимо настроить дополнительные компоненты Python, для этого последовательно введите следующие команды:

python3.10 -m pip install upgrade pip

pip3.10 install numpy==1.21.3

pip3.10 install opencv-python==4.6.0.66

Если на этапе третьей команды возникает ошибка, выглядит она так:

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXcGHS-JD_8TPmcAvMHgykQkKFiEl1Y9qR0NX1MjDUz54wUa8XWlGzx41eQU03uXeCBIwYFSxYyvMDfTlrRBBEF09OwdmMxIFrb5h4gAA_hSeDwTw8gLmK_UHUzZ-W1dIxS4WECSSrxLV63VJ_g0ZJp8S4zW?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcGHS-JD_8TPmcAvMHgykQkKFiEl1Y9qR0NX1MjDUz54wUa8XWlGzx41eQU03uXeCBIwYFSxYyvMDfTlrRBBEF09OwdmMxIFrb5h4gAA_hSeDwTw8gLmK_UHUzZ-W1dIxS4WECSSrxLV63VJ_g0ZJp8S4zW?key=-Dq4uzRdwdR6YvZS5hryuQ)

То, к сожалению, это означает невозможность запуска Stable-Diffusion на вашем маке. Если ошибка отсутствует, то можно продолжать установку.

1. После окончания установки компонентов необходимо скачать веб-интерфейс Stable-Diffusion. Для этого скопируйте и вставьте команду ниже в «Терминал» и нажмите «**Enter**».

git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXcsnhu7Myun_S10KY5feZqqA8-5JoOYu1Q86pSWlQCACgCgLz_650yjpYWO3NkkYL-IxSNmIN8mmeMbyG0crHwBp6pwPGcKCsDLitD9QCbS4HIycM4rAe4CWnCxVeMQ_MzWFcuJWFReZoxfzTcMQD680m5k?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcsnhu7Myun_S10KY5feZqqA8-5JoOYu1Q86pSWlQCACgCgLz_650yjpYWO3NkkYL-IxSNmIN8mmeMbyG0crHwBp6pwPGcKCsDLitD9QCbS4HIycM4rAe4CWnCxVeMQ_MzWFcuJWFReZoxfzTcMQD680m5k?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. Далее необходимо открыть папку Stable-Diffusion, для этого скопируйте и вставьте команду ниже в «Терминал» и нажмите «**Enter**».

open .

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXenxXHytQqiKPsQaghX9tDcUhmBSgU1LsHLfYRuqShWw_DlIpt077LtRuYHwHvt6W3HRLFd7IRhahN_eRVj6v9y_q_hCVTPsB-8kvOHqqygN0ZBtOU7nv4hOP2Bq_YNGZgP7AHBLbxlcblsOe0YzSuWH4o?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXenxXHytQqiKPsQaghX9tDcUhmBSgU1LsHLfYRuqShWw_DlIpt077LtRuYHwHvt6W3HRLFd7IRhahN_eRVj6v9y_q_hCVTPsB-8kvOHqqygN0ZBtOU7nv4hOP2Bq_YNGZgP7AHBLbxlcblsOe0YzSuWH4o?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. В открывшемся окне найдите папку «**stable-diffusion-webui**» и откройте ее.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXc6Y7__jquaVm4UPUmQNmOk18tHrAOvS6p6Murk9L6mDl1Yrr372ktYKOCyJf4EzA5Mw7WQSC6YHEwaSmS4M8JcjHlAEa5RPTJ5WXHtkAmhvvXo91QmwA7Ztj01H2mM3Wv9mE1dlsnpAnlsGFfD4LoJD9I?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc6Y7__jquaVm4UPUmQNmOk18tHrAOvS6p6Murk9L6mDl1Yrr372ktYKOCyJf4EzA5Mw7WQSC6YHEwaSmS4M8JcjHlAEa5RPTJ5WXHtkAmhvvXo91QmwA7Ztj01H2mM3Wv9mE1dlsnpAnlsGFfD4LoJD9I?key=-Dq4uzRdwdR6YvZS5hryuQ)

В папке будут находиться те же файлы и папки, что и при установке на Windows. Поэтому дальнейшие пункты для моделей, расширений и прочего актуальны и для mac OS.

1. Введите в «Терминале» следующую команду и нажмите «**Enter**»:

cd stable-diffusion-webui

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdPgsPWXrW2b0uv62nolsbnOnCDsUbFxyhCjHlHSYsoqRDT8UfKNXaX0h7qeqyYs-z0u6Yp40L2kHgBM0RadEUCm6nSh7NpriKa8cdkwLa-3Ifzm4Awvw4-ZsPhrfeAbOEksTXsR612hyXgbTa3AgV5ag67?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdPgsPWXrW2b0uv62nolsbnOnCDsUbFxyhCjHlHSYsoqRDT8UfKNXaX0h7qeqyYs-z0u6Yp40L2kHgBM0RadEUCm6nSh7NpriKa8cdkwLa-3Ifzm4Awvw4-ZsPhrfeAbOEksTXsR612hyXgbTa3AgV5ag67?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. Введите команду ls, чтобы увидеть все папки и файлы внутри папки «**stable-diffusion-webui**».

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXcLV62Pob8dPZHtFJUmeI9cFvKwrCmetam5hnQQx1U3l4l9m3jreEBvySm4RWNcuOPwucAm3gh26wlCjmz0pBlAQXbB0kVcd9cP_dRGPOvSTgGdw_nhz5nRb10YCX-HzLuQ6GNEJaS-XuMJfNcNx9OxYU31?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcLV62Pob8dPZHtFJUmeI9cFvKwrCmetam5hnQQx1U3l4l9m3jreEBvySm4RWNcuOPwucAm3gh26wlCjmz0pBlAQXbB0kVcd9cP_dRGPOvSTgGdw_nhz5nRb10YCX-HzLuQ6GNEJaS-XuMJfNcNx9OxYU31?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. После этого введите команду для запуска веб-интерфейса Stable-Diffusion и нажмите «**Enter**»

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdiiu_a4eQhH08eKWgeIHtDlzQdXKh7fQcOKiLd0NZBxq4JtvTDETRVyM-BWNcv4iTtJmFA4xMonaocaYP-X8T1OrGhfejhE6LA6wIXjllMDzsv8HbgWjuzlRSjVGgs8XMXoL4X95LK4581WV0D5fj2Dc0y?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdiiu_a4eQhH08eKWgeIHtDlzQdXKh7fQcOKiLd0NZBxq4JtvTDETRVyM-BWNcv4iTtJmFA4xMonaocaYP-X8T1OrGhfejhE6LA6wIXjllMDzsv8HbgWjuzlRSjVGgs8XMXoL4X95LK4581WV0D5fj2Dc0y?key=-Dq4uzRdwdR6YvZS5hryuQ)

При первом запуске, команда начнет скачивание и установку необходимых для корректной работы интерфейса компонентов. (*Внимание! В зависимости от скорости вашего интернета, данный процесс может занять от нескольких минут до нескольких десятков минут*)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXfq3ZfVRfdsYxu6B6Yfh3mSq5-cEo5JHXnTB5wTyarAeGxDlvCGQ7wOYAae_z2AvEBR_up-BnxPxjHMmXjI6Eg5uFTM4RddOMRNeBls1hXEx5jG6eghSc0KqK5fbw6B0ZUxoDIKvPVKwj7HsdF2iyECPNk?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfq3ZfVRfdsYxu6B6Yfh3mSq5-cEo5JHXnTB5wTyarAeGxDlvCGQ7wOYAae_z2AvEBR_up-BnxPxjHMmXjI6Eg5uFTM4RddOMRNeBls1hXEx5jG6eghSc0KqK5fbw6B0ZUxoDIKvPVKwj7HsdF2iyECPNk?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. При успешном завершении всего, появится строка с адресом веб-интерфейса и произойдет запуск браузера. Но, если у вас статичное черное окно, где последней строчкой будет написано об ошибке (error), связанной с запуском Torch, то не пугайтесь - это нормальная ситуация, для ее решения перейдите к дополнительной настройке, описанной в следующем пункте 2.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXduKcDMK5S4pQSkAjwb2QqAvvO-RCGlaVM2GaJ9d42ZeXBOsvLm7_8rY1JDxtwah7TYvwmEzETqaLp9r3WQCni037L2NXPUBr4rygviLsKED0n2PLPoJYhqVh9O73t3UTo6c1YI3AqKUvAjqQycZFG8I3UU?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXduKcDMK5S4pQSkAjwb2QqAvvO-RCGlaVM2GaJ9d42ZeXBOsvLm7_8rY1JDxtwah7TYvwmEzETqaLp9r3WQCni037L2NXPUBr4rygviLsKED0n2PLPoJYhqVh9O73t3UTo6c1YI3AqKUvAjqQycZFG8I3UU?key=-Dq4uzRdwdR6YvZS5hryuQ)

*Внимание! Stable-Diffusion работает через консоль, поэтому не закрывайте «Терминал» пока не закончите работать с нейросетью.*

1. При дальнейшей работе со Stable-Diffusion, для запуска веб-интерфейса необходимо будет выполнять всего 2 команды в «Терминале».

cd stable-diffusion-webui

./webui.sh

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXc3o_gV3WroyuP580GQ79r0FjPjbE7-1fPdON6j8Q8T9evFapyGys_XMCsxE5yBrDrdJBUM6c9_KQGHFQG8D_ZqFEevuzK9DR_xoZz9WxHF6QmGG6s_FnAZxGgFproj-jI8EFBN3ACTVKHwcHOI9dqEDQs?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc3o_gV3WroyuP580GQ79r0FjPjbE7-1fPdON6j8Q8T9evFapyGys_XMCsxE5yBrDrdJBUM6c9_KQGHFQG8D_ZqFEevuzK9DR_xoZz9WxHF6QmGG6s_FnAZxGgFproj-jI8EFBN3ACTVKHwcHOI9dqEDQs?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. **Дополнительная настройка Stable Diffusion**

Веб-интерфейс Stable Diffusion имеет ряд дополнительных настроек для оптимизации его работы на системах с различными аппаратными конфигурациями. Данные настройки также позволяют исправить ряд ошибок, которые могут возникать в ходе запуска веб-интерфейса. Вне зависимости от используемой операционной системы (Windows/Mac OS) возможный набор параметров настройки программы идентичен.

Настройка Stable-Diffusion происходит с помощью редактирования специального файла с именем – «**webui-user**», для Windows этот файл будет иметь расширение ***.bat**, а для Mac OS расширение ***.sh**

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdc2kf45bSIxSJwU1cRschMizZSm3dbpjXyFLT7AkHhc_0nG_cJ2U9MWLmhWj_Elsm475mBT9qLXXJtmCqBVT5Ci6jUJbtnCK7Bd5mB8_c7FO8nXAHwB_mG3FeCDXhyFyXhUesxknGxX4_119JaiJfxeMw?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdc2kf45bSIxSJwU1cRschMizZSm3dbpjXyFLT7AkHhc_0nG_cJ2U9MWLmhWj_Elsm475mBT9qLXXJtmCqBVT5Ci6jUJbtnCK7Bd5mB8_c7FO8nXAHwB_mG3FeCDXhyFyXhUesxknGxX4_119JaiJfxeMw?key=-Dq4uzRdwdR6YvZS5hryuQ)

*В системе Windows*

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdZDVuyRlZhU17BCdc7ddrXwOyug8nk0Io6ahDBbKMkCde2Qi5vbz_upJNiCQ_sMrrJppL4vc_e5lpuOBJ-1q_fXOHjCFvhLe7h9YS2lfCTeTg_2vWdz3h5ERz72GbBuaKDHmpGoh9K7Pp7ojGOfcq8dulB?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdZDVuyRlZhU17BCdc7ddrXwOyug8nk0Io6ahDBbKMkCde2Qi5vbz_upJNiCQ_sMrrJppL4vc_e5lpuOBJ-1q_fXOHjCFvhLe7h9YS2lfCTeTg_2vWdz3h5ERz72GbBuaKDHmpGoh9K7Pp7ojGOfcq8dulB?key=-Dq4uzRdwdR6YvZS5hryuQ)

*В системе Mac OS*

А) (Для Windows) Чтобы отредактировать файл «**webui-user.bat**», нажмите по нему правой кнопкой мыши и выберите в меню пункт «**Изменить**». (*Внимание! Не выбирайте пункт «Открыть» или не нажимайте по файлу два раза левой кнопкой мыши, т.к. это приведет к запуску скрипта внутри этого файла*).

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXek2hukKTuYATawNFPZIw9DCnarrKd_-rY-BcQnY_3qyPHTgUlMysXbEembZMlSw_LBn6fr3yM531w9qYcKaZZDJPb6X0_kt6XH3-TtqNT6A3n5KexVWOLh0nx4jPE0cO4tHhaczq7wIGYa27sLzvFk2mCV?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXek2hukKTuYATawNFPZIw9DCnarrKd_-rY-BcQnY_3qyPHTgUlMysXbEembZMlSw_LBn6fr3yM531w9qYcKaZZDJPb6X0_kt6XH3-TtqNT6A3n5KexVWOLh0nx4jPE0cO4tHhaczq7wIGYa27sLzvFk2mCV?key=-Dq4uzRdwdR6YvZS5hryuQ)

В открывшемся файле найдите строчку «**set COMMANDLINE_ARGS=**», именно в нее необходимо будет записать те параметры, которые подходят к вашей аппаратной конфигурации компьютера. По правилам параметры записываются через пробел, каждый параметр начинается с двух тире «--», порядок записи параметров неважен.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXe5bDnlGsJWkdHof5Zu0Qtz1UczdlodxfwqLkuIrTdwbgpL6SQWD6YKDY5GcRWFozffD9TqC5AfAJCQlut_LuxNnl2INCEx6rkbIYRI3IfQsfqEBHw0qIDEdprBwqx-fkc40FOci3XNnnT0T9ZJRRBq_fYP?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe5bDnlGsJWkdHof5Zu0Qtz1UczdlodxfwqLkuIrTdwbgpL6SQWD6YKDY5GcRWFozffD9TqC5AfAJCQlut_LuxNnl2INCEx6rkbIYRI3IfQsfqEBHw0qIDEdprBwqx-fkc40FOci3XNnnT0T9ZJRRBq_fYP?key=-Dq4uzRdwdR6YvZS5hryuQ)

Пример: set COMMANDLINE_ARGS=--skip-torch-cuda-test –-no-half

Б) (Для Mac OS) Чтобы отредактировать файл «**webui-user.sh**», нажмите по нему правой кнопкой мыши и выберите пункт «**Открыть с помощью**» -> «**Текстовый редактор**». (*Внимание! Не выбирайте пункт «Открыть» или не нажимайте по файлу два раза левой кнопкой мыши, т.к. это приведет к запуску скрипта внутри этого файла*).

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXco4j9bhfcNsUuEWHq734giaNC72uU-cnWhM_B65IW86ntcP182Brwj9SC48HLT1Gz42O1hQ9Vvr0g9R-Er8lo7O7etZbJZb4lpXHYY2Zhwpea9bsh64VtRGGAatIHzkiSXi3y8751o7hFq5XanTlHbHa0_?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXco4j9bhfcNsUuEWHq734giaNC72uU-cnWhM_B65IW86ntcP182Brwj9SC48HLT1Gz42O1hQ9Vvr0g9R-Er8lo7O7etZbJZb4lpXHYY2Zhwpea9bsh64VtRGGAatIHzkiSXi3y8751o7hFq5XanTlHbHa0_?key=-Dq4uzRdwdR6YvZS5hryuQ)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXeg8WnIbqSbs5cfz6mvphxr2Ww0isitXwFxvtzLXFKdNMdjutOWKFLEc7yCOQOx_CkCu4TB3D_CctOL3ECsTc7KQJOoBE9-YPN0QvbxAwHtax4FarlJ1AsJevhYoRMML3lcjP-4j6-QpWS9ibO1eYQCREA4?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeg8WnIbqSbs5cfz6mvphxr2Ww0isitXwFxvtzLXFKdNMdjutOWKFLEc7yCOQOx_CkCu4TB3D_CctOL3ECsTc7KQJOoBE9-YPN0QvbxAwHtax4FarlJ1AsJevhYoRMML3lcjP-4j6-QpWS9ibO1eYQCREA4?key=-Dq4uzRdwdR6YvZS5hryuQ)

В открывшемся файле найдите строчку «

**#export COMMANDLINE_ARGS=””**

», именно в нее необходимо будет записать те параметры, которые подходят к вашей аппаратной конфигурации компьютера. По правилам параметры записываются через пробел, внутри двойных кавычек, каждый параметр начинается с двух тире «--», порядок записи параметров неважен. Важно! Перед тем как начать вводить параметры, удалите в начале этой строки символ решетки

**#**

перед словом export.

Пример: export COMMANDLINE_ARGS=”--skip-torch-cuda-test –-no-half”

**Внимание! После ввода необходимых параметров не забудьте сохранить файл!**

Ниже предложены комбинации параметров для различных конфигураций пк:

1. Конфигурация без видеокарты NVIDIA/macbook:
- -skip-torch-cuda-test –-no-half –-use-cpu all
1. Конфигурация с картой NVIDIA ниже GTX10 серии (нкапример, GTX850/GTX750 и т.д.)
- -skip-torch-cuda-test --opt-split-attention –-lowvram
1. Конфигурация с картой NVIDIA GTX10 серии и выше (например, GTX1650/RTX2060 и т.д.)

–-xformers --opt-sdp-attention

1. **Базовая модель Stable Diffusion 1.5**

Если базовая модель Stable Diffusion v1.5 не скачалась автоматически, то ее можно скачать по ссылке: [https://huggingface.co/runwayml/stable-diffusion-v1-5/tree/main](https://huggingface.co/runwayml/stable-diffusion-v1-5/tree/main)

Для проверки нужно перейти в папку «**stable-diffusion-portable-main\models\Stable-diffusion**».

На странице появится список различных файлов, из всего списка вам необходима модель с названием **v1-5-pruned-emaonly.ckpt** (расширение *.ckpt как раз означает второе название моделей - чекпоинты). Для скачивания файла нажмите на иконку (стрелка вниз).

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXchy1FocOjMZq3H8YZ41-L26mob3Zc3IID72P2vnVDNsvBeo5lRiZzBGGdWfFMcmzVq9-P6Et4-tcn4VafN_SYdJbfXKNwXqpMP5-c4SnF6ka9w2wlZJhXayDU_gvud6rxTYXvJmYs_vHGIRKru0BmvD0g?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXchy1FocOjMZq3H8YZ41-L26mob3Zc3IID72P2vnVDNsvBeo5lRiZzBGGdWfFMcmzVq9-P6Et4-tcn4VafN_SYdJbfXKNwXqpMP5-c4SnF6ka9w2wlZJhXayDU_gvud6rxTYXvJmYs_vHGIRKru0BmvD0g?key=-Dq4uzRdwdR6YvZS5hryuQ)

Модель «**v1-5-pruned-emaonly.ckpt**» необходимо скопировать в папку «**Stable-diffusion**», которая находится в папке «**stable-diffusion-portable-main\models\Stable-diffusion**».

1. **Кастомные модели Stable Diffusion**

Все кастомные модели представляют из себя файлы с расширением *.ckpt (либо *.safetensors) и помещаются в папку «**Stable Diffusion**» по адресу: «**stable-diffusion-portable-main\models\Stable-diffusion**». Там же хранится базовая модель Stable Diffusion v1.5.

А) **Realistic Vision** - [https://civitai.com/models/4201?modelVersionId=130072](https://civitai.com/models/4201?modelVersionId=130072)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdWVcFaKc5MK_0mvGNhauSSikjHRtNYEXUXCyX0B2uEFZGQYbDNbnipsNy0YAEbtDQwy-AM6Pak6uF94ZUecjLWh_w_6sC3FjNxwfNqKHBQ57WKSpZYl3_gG2QTdl06IJ9i-eqT5LgAXgCjSRqDDpJrkdtk?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdWVcFaKc5MK_0mvGNhauSSikjHRtNYEXUXCyX0B2uEFZGQYbDNbnipsNy0YAEbtDQwy-AM6Pak6uF94ZUecjLWh_w_6sC3FjNxwfNqKHBQ57WKSpZYl3_gG2QTdl06IJ9i-eqT5LgAXgCjSRqDDpJrkdtk?key=-Dq4uzRdwdR6YvZS5hryuQ)

Б) **epiCRealism** - [https://civitai.com/models/25694/epicrealism](https://civitai.com/models/25694/epicrealism)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXcyfnRwRUZ4-MMMHp1tp6VvfehT2Jibb2XJZzwOZXnOOExUJLW9EtgkHIPtBWOHbzRNpNQnbbHOhsGk-1XyoJ0UcPNL46ZWzj7XGbVrpIEr2kxEXxMXlqClnshAC6Vz3QClA4hW4psUJ7VFzjkyMcn-Ys1H?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcyfnRwRUZ4-MMMHp1tp6VvfehT2Jibb2XJZzwOZXnOOExUJLW9EtgkHIPtBWOHbzRNpNQnbbHOhsGk-1XyoJ0UcPNL46ZWzj7XGbVrpIEr2kxEXxMXlqClnshAC6Vz3QClA4hW4psUJ7VFzjkyMcn-Ys1H?key=-Dq4uzRdwdR6YvZS5hryuQ)

Для данной модели расширение файла будет иным - *.safetensors

В) **Reliberate** - [https://huggingface.co/XpucT/Reliberate/tree/main](https://huggingface.co/XpucT/Reliberate/tree/main)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXerVDxClK15aAigKoyU0MpDVg1COKDC9iD78eti0FL2tgHMTOLmLuu2cM5ypWAfQllgWsAqOLxDvglfA5uOjYXnmvIjINREpCeezT4xEBlmVcizxnjyKBRKLegOgtyqzfb6DBz6568nrivD_F76n8NwyBA?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXerVDxClK15aAigKoyU0MpDVg1COKDC9iD78eti0FL2tgHMTOLmLuu2cM5ypWAfQllgWsAqOLxDvglfA5uOjYXnmvIjINREpCeezT4xEBlmVcizxnjyKBRKLegOgtyqzfb6DBz6568nrivD_F76n8NwyBA?key=-Dq4uzRdwdR6YvZS5hryuQ)

Для данной модели расширение файла будет иным - *.safetensors

Г) **Deliberate** - [https://huggingface.co/XpucT/Deliberate/tree/main](https://huggingface.co/XpucT/Deliberate/tree/main)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXfQCWoe3vaV1YgIJgqVa2eYTfx8RsxrMxNraQ-ye0qk7Jq6q8u4IB-MTkBrH1TaSZponGffj0VNw-Ek0h-wvRbOtHzr53yjpRJPtLQ5Y1vlvy2FmBsFD2dBy6IsCwrO7YnfhsNBlsNYCz2hr9Pu-DDyB2Q?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfQCWoe3vaV1YgIJgqVa2eYTfx8RsxrMxNraQ-ye0qk7Jq6q8u4IB-MTkBrH1TaSZponGffj0VNw-Ek0h-wvRbOtHzr53yjpRJPtLQ5Y1vlvy2FmBsFD2dBy6IsCwrO7YnfhsNBlsNYCz2hr9Pu-DDyB2Q?key=-Dq4uzRdwdR6YvZS5hryuQ)

Для данной модели расширение файла будет иным - *.safetensors

Д) **Photon** - [https://civitai.com/models/84728?modelVersionId=90072](https://civitai.com/models/84728?modelVersionId=90072)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXcLldQmd_fq7ul-JwBOldd3sB2YhbqkilkVQ-QHGrQfFb5kMlqehUrhj-fBaNMlV3j-TZ-IEJAnO1oyF-eK3DRxgPdSmr9GgOG7uezrkPGNv58vw6pkSGrLMl7WN3HHuyTt-qCQPCg_e3fWs3ZuxMHBkc5Q?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcLldQmd_fq7ul-JwBOldd3sB2YhbqkilkVQ-QHGrQfFb5kMlqehUrhj-fBaNMlV3j-TZ-IEJAnO1oyF-eK3DRxgPdSmr9GgOG7uezrkPGNv58vw6pkSGrLMl7WN3HHuyTt-qCQPCg_e3fWs3ZuxMHBkc5Q?key=-Dq4uzRdwdR6YvZS5hryuQ)

Для данной модели расширение файла будет иным - *.safetensors

1. **Модели LoRa**

Все модели LoRa представляют из себя файлы с расширением *.ckpt (либо *.safetensors) и помещаются в папку «**Lora**» по адресу: «**stable-diffusion-portable-main\models\Lora**».

А) **Detail Tweaker LoRA** - [https://civitai.com/models/58390/detail-tweaker-lora-lora](https://civitai.com/models/58390/detail-tweaker-lora-lora)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXevD654YB97W_STUsp2rh-piijos9DHvULHQa9_tDRR9orbUL191Bs9FkO5vLWJ4KceREs-B9GTd-zuNQ23boaX8DTFzmE1W0rXlACK5Z2v8X7k1vIIapXG-qI4nPD7_64f-PGYKaV1fS1EI2RIiFzaV5cj?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXevD654YB97W_STUsp2rh-piijos9DHvULHQa9_tDRR9orbUL191Bs9FkO5vLWJ4KceREs-B9GTd-zuNQ23boaX8DTFzmE1W0rXlACK5Z2v8X7k1vIIapXG-qI4nPD7_64f-PGYKaV1fS1EI2RIiFzaV5cj?key=-Dq4uzRdwdR6YvZS5hryuQ)

Б) **MIR** - [https://civitai.com/models/121955/mir](https://civitai.com/models/121955/mir)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdnconylDd-LEAnlhoiAwi5DffJcSkEbEvsxtSs_qtMR8B8-HbufgHD0bijNp1UtG7St5aheWIjHUdyeASDYJwac0HILmnASccq_gha5O37FmsCMWfrBzjILEw5eiCcQF8eGYkbEbSZRaxgV6sriaSM1wI?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdnconylDd-LEAnlhoiAwi5DffJcSkEbEvsxtSs_qtMR8B8-HbufgHD0bijNp1UtG7St5aheWIjHUdyeASDYJwac0HILmnASccq_gha5O37FmsCMWfrBzjILEw5eiCcQF8eGYkbEbSZRaxgV6sriaSM1wI?key=-Dq4uzRdwdR6YvZS5hryuQ)

В) **Minustype_UrbanAerial** - [https://civitai.com/models/24063/minustypeurbanaerial](https://civitai.com/models/24063/minustypeurbanaerial)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXfQi_X_1bQt_9ZX-uLngKMVLFF77TKgwnRO1kNSiDPOmrLoJu585hCufJBwL6EHhpg2X6zbvaqG1Si2e-PBpgXK0rBD4opNhCTHzk0RH-3aoHq6NyAarWp1a-48DXzf4srDdckecywmYRPAR5r_9aSsQGQT?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfQi_X_1bQt_9ZX-uLngKMVLFF77TKgwnRO1kNSiDPOmrLoJu585hCufJBwL6EHhpg2X6zbvaqG1Si2e-PBpgXK0rBD4opNhCTHzk0RH-3aoHq6NyAarWp1a-48DXzf4srDdckecywmYRPAR5r_9aSsQGQT?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. **Расширение ControlNet**

Дополнение ControlNet устанавливается внутри Stable Diffusion через его веб-интерфейс. Поэтому перед установкой запустите Stable Diffusion. Процесс установки также можно посмотреть в видео по ссылке: [https://www.youtube.com/watch?v=aNOPusJ4Z1E&ab_channel=Archive](https://www.youtube.com/watch?v=aNOPusJ4Z1E&ab_channel=Archive)

1. Запустите **Stable Diffusion**
2. Внутри веб-интерфейса нажмите вкладку «**Extensions**», затем вкладку «**Available**», в ней на кнопку «**Load from:**». После загрузки списка расширений введите в поисковой строке: «**controlnet**»

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXe81q0pDygk6k_G75WqQ5kNMdo0vqKcSCKZCRzJ4Quc_WprJea9aWvh_AbeIgbrFdekwshwc15bfGXzTYUnJCC-Bnc6tUSZ5Am3IViPHeonIHts2RkHvvw8SWmaMm9-Wee58Ez1GPbh8Ye8TUNgrKiuu24?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe81q0pDygk6k_G75WqQ5kNMdo0vqKcSCKZCRzJ4Quc_WprJea9aWvh_AbeIgbrFdekwshwc15bfGXzTYUnJCC-Bnc6tUSZ5Am3IViPHeonIHts2RkHvvw8SWmaMm9-Wee58Ez1GPbh8Ye8TUNgrKiuu24?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. В списке найдите «**sd-webui-controlnet**», описание к которой начинается с «**WebUI**» и нажмите кнопку «**Install**» в правой части окна.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdcZH6me0IGwM6vcVyioZLPO-83I8RAj1xmaTxNDn07nb1xVIkKSWwm7PTINkQdRSbUKnxomwwUriSk75o2O4OaSPaokjbOKPoYNt2nIa0EcLerYAIGCvQR1PQYpr4oBSVc66mwmnqrGDZGLnt_pxQN01wJ?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdcZH6me0IGwM6vcVyioZLPO-83I8RAj1xmaTxNDn07nb1xVIkKSWwm7PTINkQdRSbUKnxomwwUriSk75o2O4OaSPaokjbOKPoYNt2nIa0EcLerYAIGCvQR1PQYpr4oBSVc66mwmnqrGDZGLnt_pxQN01wJ?key=-Dq4uzRdwdR6YvZS5hryuQ)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdti8tqKJXlD8Y0YsMOVa2rhOhn1fQJpK0PZY_x4xupspkupmvko2C4cca6jCLirbbMGdY7JoLa_rqvdYC9LdZ6GPbBmPgWN1MQYIpnoy952tYaa8PUE_kKYpwacRgAzPtl6L20EzDGA6cb3ZOf607r7TlT?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdti8tqKJXlD8Y0YsMOVa2rhOhn1fQJpK0PZY_x4xupspkupmvko2C4cca6jCLirbbMGdY7JoLa_rqvdYC9LdZ6GPbBmPgWN1MQYIpnoy952tYaa8PUE_kKYpwacRgAzPtl6L20EzDGA6cb3ZOf607r7TlT?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. Перейдите во вкладку «**Installed**» и проверьте, что в списке появилась строка с названием расширения «**sd-webui-controlnet**». После чего нажмите кнопку «**Apply & Restart**» для установки расширения в систему.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdwImXdlbxCgBKS-7wcE1IvJ3Oel2QsbV1V1HhSf9BtQII8NH6zuTk8eycVQ2w41HFH4DCzShHPPknVyOX2JuH4q3Pc205IzrHEgdAH3jrBNpeI0zTAf2Ua5bVCOfsecghGEsspaXcH5z36K_rF9257DrE?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdwImXdlbxCgBKS-7wcE1IvJ3Oel2QsbV1V1HhSf9BtQII8NH6zuTk8eycVQ2w41HFH4DCzShHPPknVyOX2JuH4q3Pc205IzrHEgdAH3jrBNpeI0zTAf2Ua5bVCOfsecghGEsspaXcH5z36K_rF9257DrE?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. После перезагрузки интерфейса внизу должен появится раздел «**ControlNet**»

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXfSkfUl6JRKoQ4_4hjJU2l8z_zCne5fJJa8dR2rQXEeyI7RQ8yL6SU3d1Z7YDGsD8pjNKEy8PGQus7XUOru0d81rmHDlu04WG1h-PJZpCxXXrrknq5ogQTPOia88XYnTBsHf8QduT3mrc0mGXIzLy4wBln7?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfSkfUl6JRKoQ4_4hjJU2l8z_zCne5fJJa8dR2rQXEeyI7RQ8yL6SU3d1Z7YDGsD8pjNKEy8PGQus7XUOru0d81rmHDlu04WG1h-PJZpCxXXrrknq5ogQTPOia88XYnTBsHf8QduT3mrc0mGXIzLy4wBln7?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. На этом установка ControlNet завершена, остается только скачать для данного расширения модели по ссылке: [https://huggingface.co/lllyasviel/ControlNet-v1-1/tree/main](https://huggingface.co/lllyasviel/ControlNet-v1-1/tree/main)

Из списка файлов скачайте следующие:

- control_v11f1p_sd15_depth.pth
- control_v11p_sd15_canny.pth
- control_v11p_sd15_lineart.pth
- control_v11p_sd15_mlsd.pth
- control_v11p_sd15_softedge.pth
- control_v11f1e_sd15_tile.pth

Для скачивания файлов нажимайте на иконку (стрелка вниз). Файлы данного расширения (*.pth) необходимо поместить в папку «**models**», которая находится по адресу: «**stable-diffusion-portable-main\extensions\sd-webui-controlnet\models**»

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXfdaWxOMm6ItqegL8jrB9MGhpYhKqErQu7CD_5XK-KorvAvPwROjR4_n_fMJ48bXdl1RCYq265gA33Ii67flTlwnh8B37EGHL_HLhyKRtltjkZ3yGwWB6RNkaFwQj01CzYeLi-ZXWKqDD6tBtAC4vgzRHA?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfdaWxOMm6ItqegL8jrB9MGhpYhKqErQu7CD_5XK-KorvAvPwROjR4_n_fMJ48bXdl1RCYq265gA33Ii67flTlwnh8B37EGHL_HLhyKRtltjkZ3yGwWB6RNkaFwQj01CzYeLi-ZXWKqDD6tBtAC4vgzRHA?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. Скачайте также модели по данной ссылке: [https://huggingface.co/lllyasviel/sd_control_collection/tree/main](https://huggingface.co/lllyasviel/sd_control_collection/tree/main)

Из списка файлов скачайте следующие:

- ip-adapter_sd15.pth
- ip-adapter_sd15_plus.pth

Для скачивания файлов нажимайте на иконку (стрелка вниз). Файлы данного расширения (*.pth) необходимо поместить в папку «**models**», которая находится по адресу: «**stable-diffusion-portable-main\extensions\sd-webui-controlnet\models**»

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdbcB9gjUqmYamn6bxb1rOUVd24xE2iE90HgKe7MAAz0VqdXnFgCrX0GsqyEo97w7T4E5Xti3cdI7gVfj_1-rVSqdtobHd24I329vzgyhjkDOFsp18fpCrNeCorH_E7w0vSk_Sm6Qu7r_GYqLoyAKFDGj3n?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdbcB9gjUqmYamn6bxb1rOUVd24xE2iE90HgKe7MAAz0VqdXnFgCrX0GsqyEo97w7T4E5Xti3cdI7gVfj_1-rVSqdtobHd24I329vzgyhjkDOFsp18fpCrNeCorH_E7w0vSk_Sm6Qu7r_GYqLoyAKFDGj3n?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. **Расширение Photopea**

Дополнение Photopea устанавливается внутри Stable Diffusion через его веб-интерфейс. Поэтому перед установкой запустите Stable Diffusion.

1. **Запустите Stable Diffusion**
2. **Внутри веб-интерфейса нажмите вкладку «Extensions», затем вкладку «Install from URL» и в поле «URL for extension’s git repository» введите следующий адрес: [https://github.com/yankooliveira/sd-webui-photopea-embed](https://github.com/yankooliveira/sd-webui-photopea-embed) После чего нажмите кнопку «Install»**

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXfp-80GzPMSNtFm0F-8nTwqtzUli9ACtMti2fwg-pLuSRe8UVVKmZtrjndCeye_IzIRJCMbCM56ejncNayEFtN18i-iLiELiMhEK1CuhVr-M8hFmAqr6C1bR79dm-ANYs6Vv84YQDNO2npGld8m72JW-k8N?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfp-80GzPMSNtFm0F-8nTwqtzUli9ACtMti2fwg-pLuSRe8UVVKmZtrjndCeye_IzIRJCMbCM56ejncNayEFtN18i-iLiELiMhEK1CuhVr-M8hFmAqr6C1bR79dm-ANYs6Vv84YQDNO2npGld8m72JW-k8N?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. После завершения установки под кнопкой появится соответствующая надпись.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXcPi3rwa5mSNs2xCK5mvUFsfpnj6OGcsw-wHPyzk5pE9CHonb7DP5ehWqWow6gTTPZcTgAudekBzDhy9rsyLhqbpKUStwYS2LaoWpb2dfYvIgenPMM6emOQPeWoHwUVj0A3dUu_iHdb9C16D27ibSo8R1FD?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcPi3rwa5mSNs2xCK5mvUFsfpnj6OGcsw-wHPyzk5pE9CHonb7DP5ehWqWow6gTTPZcTgAudekBzDhy9rsyLhqbpKUStwYS2LaoWpb2dfYvIgenPMM6emOQPeWoHwUVj0A3dUu_iHdb9C16D27ibSo8R1FD?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. Перейдите во вкладку «**Installed**» после чего нажмите кнопку «**Apply & Restart**» для установки расширения в систему.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXeVTHY6PVBPfLSUreyAqZJNZAK2EJpvWMmF4XpLSdAnIHZp3Kx3YyQNuk76RzbDeSNPlnOL29kyvvUeLXefODVBykcZXqZ7ENVjFaZ-tWAVPMsp5mesHWDfj29esToek_HT5BLErGLvghI0H61coAqpq2s?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeVTHY6PVBPfLSUreyAqZJNZAK2EJpvWMmF4XpLSdAnIHZp3Kx3YyQNuk76RzbDeSNPlnOL29kyvvUeLXefODVBykcZXqZ7ENVjFaZ-tWAVPMsp5mesHWDfj29esToek_HT5BLErGLvghI0H61coAqpq2s?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. После перезагрузки интерфейса появится новый раздел «**Photopea**»

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXcA34ZmvkG65Fl6TAv2ACoO0uQH1ywWR5nHmIM5yzmUtxBrlAs3lgn49STynfPCrg3ZM6coE5Sufxi0YNNqhNjZSKx56Dl-Zp8STQeCRsX6Ak76vLmtRBhOzfrII2lkCpYk7dnyctcq_ZDBF3Us9XzLEA83?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcA34ZmvkG65Fl6TAv2ACoO0uQH1ywWR5nHmIM5yzmUtxBrlAs3lgn49STynfPCrg3ZM6coE5Sufxi0YNNqhNjZSKx56Dl-Zp8STQeCRsX6Ak76vLmtRBhOzfrII2lkCpYk7dnyctcq_ZDBF3Us9XzLEA83?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. **Модели Embedding**

Все модели Embedding представляют из себя файлы с расширением *.pt и помещаются в папку «**Embeddings**» по адресу: «**stable-diffusion-portable-main\embeddings**».

А) **veryBadImageNegative** - [https://civitai.com/models/11772/verybadimagenegative](https://civitai.com/models/11772/verybadimagenegative)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXeTDXNXxKosahE0ZBeAntlVAzrnhdVyeQNEpb5kQgtyrMwHx5wU503gH4JZgfmh2x8lqD5OLIWulTcoGm1seF_5TpHr92FLxKditFcYI4F-MjUDjqhb0tMCzj6gSpTm7pkmnU3HJdu5QKQrE-hHA6qNKa2y?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeTDXNXxKosahE0ZBeAntlVAzrnhdVyeQNEpb5kQgtyrMwHx5wU503gH4JZgfmh2x8lqD5OLIWulTcoGm1seF_5TpHr92FLxKditFcYI4F-MjUDjqhb0tMCzj6gSpTm7pkmnU3HJdu5QKQrE-hHA6qNKa2y?key=-Dq4uzRdwdR6YvZS5hryuQ)

Б) **BadDream + UnrealisticDream** - [https://civitai.com/models/72437/baddream-unrealisticdreamnegative-embeddings](https://civitai.com/models/72437/baddream-unrealisticdreamnegative-embeddings)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXfyRrGQqXm2EDbHOpMigZgAtAkf7bEPQy3Zh5nYgUKlNr_DSRvGx4uJxq6FbobaXFCiL-Hki1XhduPDlHCeUsthImJYfjvryHoRNLCdB3KTGnhWE0vXjlibACOb27OAPWbXXJlAXN0Qa9eRRjvy85clWtxQ?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfyRrGQqXm2EDbHOpMigZgAtAkf7bEPQy3Zh5nYgUKlNr_DSRvGx4uJxq6FbobaXFCiL-Hki1XhduPDlHCeUsthImJYfjvryHoRNLCdB3KTGnhWE0vXjlibACOb27OAPWbXXJlAXN0Qa9eRRjvy85clWtxQ?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. **Расширение Ultimate SD Upscale**

Дополнение Ultimate SD Upscale устанавливается внутри Stable Diffusion через его веб-интерфейс. Поэтому перед установкой запустите Stable Diffusion.

1. **Запустите Stable Diffusion**
2. **Внутри веб-интерфейса нажмите вкладку «Extensions», затем вкладку «Install from URL» и в поле «URL for extension’s git repository» введите следующий адрес: [https://github.com/Coyote-A/ultimate-upscale-for-automatic1111](https://github.com/Coyote-A/ultimate-upscale-for-automatic1111) После чего нажмите кнопку «Install»**

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXd_KN0es04Ye-YYzmhpfOHTTApllEbM6N9Mip3hmmWYt7fAdjhPRoxw-UPP2dJ3qsAKjbDo5CjJcMsO3dZmcSOL-E_7VuQqYz3QYygDyxpFusAyonX4ynTFc2aFZowqMdlZcHmm_2uGhotvqB3O4GDmIav-?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd_KN0es04Ye-YYzmhpfOHTTApllEbM6N9Mip3hmmWYt7fAdjhPRoxw-UPP2dJ3qsAKjbDo5CjJcMsO3dZmcSOL-E_7VuQqYz3QYygDyxpFusAyonX4ynTFc2aFZowqMdlZcHmm_2uGhotvqB3O4GDmIav-?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. После завершения установки под кнопкой появится соответствующая надпись.
2. Перейдите во вкладку «**Installed**» после чего нажмите кнопку «**Apply & Restart**» для установки расширения в систему.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXeVTHY6PVBPfLSUreyAqZJNZAK2EJpvWMmF4XpLSdAnIHZp3Kx3YyQNuk76RzbDeSNPlnOL29kyvvUeLXefODVBykcZXqZ7ENVjFaZ-tWAVPMsp5mesHWDfj29esToek_HT5BLErGLvghI0H61coAqpq2s?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeVTHY6PVBPfLSUreyAqZJNZAK2EJpvWMmF4XpLSdAnIHZp3Kx3YyQNuk76RzbDeSNPlnOL29kyvvUeLXefODVBykcZXqZ7ENVjFaZ-tWAVPMsp5mesHWDfj29esToek_HT5BLErGLvghI0H61coAqpq2s?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. На этом установка расширения завершена
2. **Tiled Diffusion (multidiffusion)**

Дополнение Ultimate Tiled Diffusion устанавливается внутри Stable Diffusion через его веб-интерфейс. Поэтому перед установкой запустите Stable Diffusion.

1. **Запустите Stable Diffusion**
2. **Внутри веб-интерфейса нажмите вкладку «Extensions», затем вкладку «Install from URL» и в поле «URL for extension’s git repository» введите следующий адрес: [https://github.com/pkuliyi2015/multidiffusion-upscaler-for-automatic1111](https://github.com/pkuliyi2015/multidiffusion-upscaler-for-automatic1111) После чего нажмите кнопку «Install»**

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXd_KN0es04Ye-YYzmhpfOHTTApllEbM6N9Mip3hmmWYt7fAdjhPRoxw-UPP2dJ3qsAKjbDo5CjJcMsO3dZmcSOL-E_7VuQqYz3QYygDyxpFusAyonX4ynTFc2aFZowqMdlZcHmm_2uGhotvqB3O4GDmIav-?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd_KN0es04Ye-YYzmhpfOHTTApllEbM6N9Mip3hmmWYt7fAdjhPRoxw-UPP2dJ3qsAKjbDo5CjJcMsO3dZmcSOL-E_7VuQqYz3QYygDyxpFusAyonX4ynTFc2aFZowqMdlZcHmm_2uGhotvqB3O4GDmIav-?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. После завершения установки под кнопкой появится соответствующая надпись.
2. Перейдите во вкладку «**Installed**» после чего нажмите кнопку «**Apply & Restart**» для установки расширения в систему.

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXeVTHY6PVBPfLSUreyAqZJNZAK2EJpvWMmF4XpLSdAnIHZp3Kx3YyQNuk76RzbDeSNPlnOL29kyvvUeLXefODVBykcZXqZ7ENVjFaZ-tWAVPMsp5mesHWDfj29esToek_HT5BLErGLvghI0H61coAqpq2s?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeVTHY6PVBPfLSUreyAqZJNZAK2EJpvWMmF4XpLSdAnIHZp3Kx3YyQNuk76RzbDeSNPlnOL29kyvvUeLXefODVBykcZXqZ7ENVjFaZ-tWAVPMsp5mesHWDfj29esToek_HT5BLErGLvghI0H61coAqpq2s?key=-Dq4uzRdwdR6YvZS5hryuQ)

1. На этом установка расширения завершена
2. **Дополнительные апскейлеры**

Дополнительные модели для апскейлеров представляют из себя файлы с расширением *.pt и помещаются в папку «**ESRGAN**» по адресу: «**stable-diffusion-portable-main\models\ESRGAN**».

Если папка отсутствует, то ее необходимо создать.

А) **4x_NMKD-Siax_200k** - [https://huggingface.co/gemasai/4x_NMKD-Siax_200k/tree/main](https://huggingface.co/gemasai/4x_NMKD-Siax_200k/tree/main)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXd67uLSkdQh2C8oU4Vpi92CcbSRcmFtzRXExQYj1Hv1a5LXpTsmUvRattJinbaeoi2aHfKBl4BVVMMyZUehM2LlUnyppQr7W5J8EYbJlUWL9FzhFcNd-mzir0RvIavLeFaAh82xx68EYadzwN899Ec7Cygi?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd67uLSkdQh2C8oU4Vpi92CcbSRcmFtzRXExQYj1Hv1a5LXpTsmUvRattJinbaeoi2aHfKBl4BVVMMyZUehM2LlUnyppQr7W5J8EYbJlUWL9FzhFcNd-mzir0RvIavLeFaAh82xx68EYadzwN899Ec7Cygi?key=-Dq4uzRdwdR6YvZS5hryuQ)

Б) **4x_foolhardy_Remacri** - [https://huggingface.co/FacehugmanIII/4x_foolhardy_Remacri/tree/main](https://huggingface.co/FacehugmanIII/4x_foolhardy_Remacri/tree/main)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXdWrsDPpM2AEQTQz1ClZrkyg97AFESvHP0OGLJMf9_mOdXRu9aAw5UCyB-npm0kMcOcYuoQ3zJQOF18XFY5YbpuaMHOen9oIELP1eybGlQ0R6imlrXTcIriiyda5JDIp9uySlJbvoxuqEwGHsB9-dV0FHGE?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdWrsDPpM2AEQTQz1ClZrkyg97AFESvHP0OGLJMf9_mOdXRu9aAw5UCyB-npm0kMcOcYuoQ3zJQOF18XFY5YbpuaMHOen9oIELP1eybGlQ0R6imlrXTcIriiyda5JDIp9uySlJbvoxuqEwGHsB9-dV0FHGE?key=-Dq4uzRdwdR6YvZS5hryuQ)

В) **4x-Ultrasharp** - [https://huggingface.co/lokCX/4x-Ultrasharp/tree/main](https://huggingface.co/lokCX/4x-Ultrasharp/tree/main)

[https://lh7-rt.googleusercontent.com/docsz/AD_4nXc1ensFz_alHt8VB0GFxf_lkWoQpUVRc0oAdxSinwPUj9uCD3mLk3Bpuc13UtZuL6Nj-BR6EDhW6H2Fto0GrZbRictXCxiYD-w_XuOMwTY2_KLeGroziIApFuYo4gDPY2B_e14uI0aJJAIJ3qKkOQsVeYm_?key=-Dq4uzRdwdR6YvZS5hryuQ](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc1ensFz_alHt8VB0GFxf_lkWoQpUVRc0oAdxSinwPUj9uCD3mLk3Bpuc13UtZuL6Nj-BR6EDhW6H2Fto0GrZbRictXCxiYD-w_XuOMwTY2_KLeGroziIApFuYo4gDPY2B_e14uI0aJJAIJ3qKkOQsVeYm_?key=-Dq4uzRdwdR6YvZS5hryuQ)