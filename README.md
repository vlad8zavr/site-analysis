# site-analysis

**Анализ сайта lifehacker**

## Network

1. **Неоптимальные моменты**

![bad moments](/screens/long-stalled-requests.png)
Format: ![bad  moments](url)

`(screens/long-stalled-requests.png)`

2. **Лишние размеры**

Файл | kBytes | Избыточность
---- | ------ | ------------
context_static.js | (1 091 kB) | 70%
tag.js | (368 kB) | избыточность 64%
show_ads_impl.js | (233 kB) | избыточность 87%
vendors.min.js.?ver=1.3.12 | (147 kB) | избыточность 78%
all.min.css?ver=1.3.12 | (129 kB) | избыточность 87%
vendors.min.css?ver=1.3.12 | (107 kB) | избыточность 95%

3. **дублирование css**

Повторения | Файл | Версии
---------- | ---- | ------
x2 | style.css | (ver=1.3.12/7)
x2 | style.min.css | (ver=5.1.2/17)
x2 | all.min.css | (ver=1.3.12/1.0.0)
x2 | main.min.css / main.css | 

4. **дублирование js**

Повторения | Файл | Версии
---------- | ---- | ------
x2 | all.min.js | (ver=1.3.12\1.0.0)
x2 | integrator.js?domain=lifehacker.ru | 
x2 | show_ads_impl.js | 
x2 | app.js | (ver=17\7)
x3 | jquery.js?ver=1.12.4 \ jquery-migrate.min.js?ver=1.4.1 \ jquery.lazy.min.js?ver=1.3.12 | 

5. **дублирование html**

Повторения | Файл
---------- | ----
x3 | render.html

6. **Проблемы загрузки**

Файл pixel не давал загрузиться странице.

![bad moment](/screens/network-problem-pixel.png)
Format: ![bad  moment](url)

`(screens/network-problem-pixel.png)`


![bad moment](/screens/network-problem-pixel-source.png)
Format: ![bad  moment](url)

`(screens/network-problem-pixel-source.png)`



Долгая загрузка у следующих запросов:

![bad moment](/screens/network-slow-load.png)
Format: ![bad  moment](url)

`(screens/network-slow-load.png)`


## Performance

Событие | Время
------- | -----
First Paint | 1106,7 ms
First Meaningful Paint | 2189.1 ms
DOM Content Loaded | 3835.0 ms
Load | 6285.1 ms
====  | ====
Loading | 93 ms
Scripting | 3046 ms
Rendering | 1274 ms
Painting | 234 ms

## Coverage

1. неиспользуемый css

Источник | Bytes
-------- | -----
https://lifehacker.ru/wp-content/plugins/lh-twister/assets/style.css?ver=7 | 431
https://lifehacker.ru/wp-content/themes/lifehacker/static/fonts/style.css?ver=1.3.12 | 1 629
https://lifehacker.ru/wp-content/themes/lifehacker/static/styles/all.min.css?ver1.3.12 | 112 552
https://lifehacker.ru/wp-content/themes/lifehacker/static/styles/vendors.min.css?ver=1.3.12 | 101 884
https://lifehacker.ru | ~ 6 000

**Сумма = 222,496 kBytes**

2. **неиспользуемый js**

**Сумма = 2 235 kBytes**

![bad moment](/screens/coverage-screen.png)
Format: ![bad  moment](url)

`(screens/coverage-screen.png)`