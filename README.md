# site-analysis

**Анализ сайта lifehacker**

## Network

1. **Неоптимальные моменты**

![bad moments](/screens/long-stalled-requests.png)
Format: ![Alt Text](url)

`(screens/long-stalled-requests.png)`

1. **Лишние размеры**

Файл | kBytes | Избыточность
---- | ------ | ------------
context_static.js | (1 091 kB) | 70%
tag.js | (368 kB) | избыточность 64%
show_ads_impl.js | (233 kB) | избыточность 87%
vendors.min.js.?ver=1.3.12 | (147 kB) | избыточность 78%
all.min.css?ver=1.3.12 | (129 kB) | избыточность 87%
vendors.min.css?ver=1.3.12 | (107 kB) | избыточность 95%

2. **дублирование css**

Повторения | Файл | Версии
---------- | ---- | ------
x2 | style.css | (ver=1.3.12/7)
x2 | style.min.css | (ver=5.1.2/17)
x2 | all.min.css | (ver=1.3.12/1.0.0)
x2 | main.min.css / main.css | 

3. **дублирование js**

Повторения | Файл | Версии
---------- | ---- | ------
x2 | all.min.js | (ver=1.3.12\1.0.0)
x2 | integrator.js?domain=lifehacker.ru | 
x2 | show_ads_impl.js | 
x2 | app.js | (ver=17\7)
x3 | jquery.js?ver=1.12.4 \ jquery-migrate.min.js?ver=1.4.1 \ jquery.lazy.min.js?ver=1.3.12 | 

4. **дублирование html**

Повторения | Файл
---------- | ----
x3 | render.html


## Performance

## Coverage