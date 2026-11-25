# Шрифты тем оболочки

Проверка лицензий и кириллицы выполнена **до скачивания файлов шрифтов**
(FR-614, FR-613). Дата проверки — **2026-09-09**. Все девять семейств идут под
**SIL Open Font License, Version 1.1** (SPDX `OFL-1.1`); полный текст лицензии
каждого семейства лежит рядом отдельным файлом.

## Таблица семейств

| Семейство           | Тема и роль                     | Лицензия                           | Файл лицензии                     | Первоисточник (URL)                                                                                                                                                                                                                 | Кириллица (чем подтверждена)                                                                                                                                                                            | `cyrillic-ext` |
| ------------------- | ------------------------------- | ---------------------------------- | --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------- |
| IBM Plex Sans       | `dispatch` — интерфейс          | SIL Open Font License, Version 1.1 | `LICENSE-ibm-plex-sans.txt`       | https://raw.githubusercontent.com/google/fonts/main/ofl/ibmplexsans/OFL.txt (совпадает байт в байт с https://raw.githubusercontent.com/IBM/plex/master/LICENSE.txt)                                                                 | CSS-ответ `https://fonts.googleapis.com/css2?family=IBM+Plex+Sans&display=swap`: блоки `/* cyrillic */` (`unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116`) и `/* cyrillic-ext */` | да             |
| IBM Plex Mono       | `dispatch` — числа              | SIL Open Font License, Version 1.1 | `LICENSE-ibm-plex-mono.txt`       | https://raw.githubusercontent.com/google/fonts/main/ofl/ibmplexmono/OFL.txt (совпадает байт в байт с https://raw.githubusercontent.com/IBM/plex/master/LICENSE.txt)                                                                 | CSS-ответ `https://fonts.googleapis.com/css2?family=IBM+Plex+Mono&display=swap`: блоки `/* cyrillic */` и `/* cyrillic-ext */`                                                                          | да             |
| Golos Text          | `editorial` — интерфейс         | SIL Open Font License, Version 1.1 | `LICENSE-golos-text.txt`          | https://raw.githubusercontent.com/google/fonts/main/ofl/golostext/OFL.txt (правообладатель — https://github.com/googlefonts/golos-text, репозиторий существует, GitHub API отдаёт `"spdx_id": "OFL-1.1"`)                           | CSS-ответ `https://fonts.googleapis.com/css2?family=Golos+Text&display=swap`: блоки `/* cyrillic */` и `/* cyrillic-ext */`                                                                             | да             |
| Literata            | `editorial` — заголовки и числа | SIL Open Font License, Version 1.1 | `LICENSE-literata.txt`            | https://raw.githubusercontent.com/google/fonts/main/ofl/literata/OFL.txt (правообладатель — https://github.com/googlefonts/literata, GitHub API отдаёт `"spdx_id": "OFL-1.1"`)                                                      | CSS-ответ `https://fonts.googleapis.com/css2?family=Literata&display=swap`: блоки `/* cyrillic */` и `/* cyrillic-ext */`                                                                               | да             |
| Manrope             | `instrument` — интерфейс        | SIL Open Font License, Version 1.1 | `LICENSE-manrope.txt`             | https://raw.githubusercontent.com/google/fonts/main/ofl/manrope/OFL.txt                                                                                                                                                             | CSS-ответ `https://fonts.googleapis.com/css2?family=Manrope&display=swap`: блоки `/* cyrillic */` и `/* cyrillic-ext */`                                                                                | да             |
| JetBrains Mono      | `instrument` и `layer` — числа  | SIL Open Font License, Version 1.1 | `LICENSE-jetbrains-mono.txt`      | https://raw.githubusercontent.com/google/fonts/main/ofl/jetbrainsmono/OFL.txt (совпадает байт в байт с https://raw.githubusercontent.com/JetBrains/JetBrainsMono/master/OFL.txt)                                                    | CSS-ответ `https://fonts.googleapis.com/css2?family=JetBrains+Mono&display=swap`: блоки `/* cyrillic */` и `/* cyrillic-ext */`                                                                         | да             |
| Fira Sans           | `signal` — интерфейс            | SIL Open Font License, Version 1.1 | `LICENSE-fira-sans.txt`           | https://raw.githubusercontent.com/google/fonts/main/ofl/firasans/OFL.txt (upstream — https://raw.githubusercontent.com/mozilla/Fira/master/LICENSE, та же OFL 1.1, отличается только строка копирайта: «Digitized data copyright…») | CSS-ответ `https://fonts.googleapis.com/css2?family=Fira+Sans&display=swap`: блоки `/* cyrillic */` и `/* cyrillic-ext */`                                                                              | да             |
| Fira Sans Condensed | `signal` — шапки таблиц         | SIL Open Font License, Version 1.1 | `LICENSE-fira-sans-condensed.txt` | https://raw.githubusercontent.com/google/fonts/main/ofl/firasanscondensed/OFL.txt (upstream — https://raw.githubusercontent.com/mozilla/Fira/master/LICENSE)                                                                        | Проверено **отдельно от Fira Sans**: CSS-ответ `https://fonts.googleapis.com/css2?family=Fira+Sans+Condensed&display=swap` содержит блоки `/* cyrillic */` и `/* cyrillic-ext */`                       | да             |
| Onest               | `layer` — интерфейс             | SIL Open Font License, Version 1.1 | `LICENSE-onest.txt`               | https://raw.githubusercontent.com/google/fonts/main/ofl/onest/OFL.txt                                                                                                                                                               | CSS-ответ `https://fonts.googleapis.com/css2?family=Onest&display=swap`: блоки `/* cyrillic */` и `/* cyrillic-ext */`                                                                                  | да             |

Тема `base` шрифтов не везёт: она остаётся на системном стеке
(`--vr-font-family-base`, `tokens.css`).

## Совместимость с поставкой

OFL 1.1 разрешает включение шрифтов в состав программного продукта, в том
числе коммерческого, и распространение установщиком, при двух условиях,
которые здесь выполнены: файлы шрифтов не продаются сами по себе, и каждая
копия сопровождается копирайтом и текстом лицензии. Ограничение OFL на
Reserved Font Name (у IBM Plex — «Plex») касается только модифицированных
версий; мы поставляем файлы без изменений.

**Как лицензии попадают к пользователю.** Сами `woff2` едут внутри `app.asar`
(Vite эмитирует их в `out/renderer/assets/`), а этот каталог — `src/…` — в
`app.asar` не попадает вовсе: `electron-builder.yml` отрезает его правилом
`'!src/*'`. Поэтому девяти файлов `LICENSE-*.txt` и этой сводки в поставке
сначала не было — шрифты распространялись без сопровождающего текста лицензии.
Починено в T029a отдельной записью `extraResources`: лицензии кладутся в
`resources/fonts/` рядом с `app.asar`, а не внутрь него — лицензия должна
читаться без распаковки архива. Проверять факт нужно составом `resources/`
после сборки, а не намерением: первоначальное утверждение «лежат в репозитории
и попадают в сборку» было принято на веру и оказалось неверным.

IBM Plex Sans и IBM Plex Mono идут под одной лицензией одного правообладателя,
Fira Sans и Fira Sans Condensed — тоже. Файлы лицензий всё равно продублированы
по одному на семейство, чтобы соответствие «семейство → лицензия» читалось по
каталогу без домысливания.

## Подмножества не режем

Файлы `woff2` кладутся такими, какими их отдаёт первоисточник. Урезание набора
глифов (subsetting) делает файл Modified Version в терминах OFL, а OFL требует
от модифицированной версии сменить имя и запрещает использовать Reserved Font
Name. Ради экономии пары сотен килобайт в офлайн-приложении это не делается.

## Как перепроверить

```sh
curl -sS -H "User-Agent: Mozilla/5.0" \
  "https://fonts.googleapis.com/css2?family=Fira+Sans+Condensed&display=swap" \
  | grep -E "^/\*|unicode-range"
```

Кириллический диапазон — `U+0400-045F` в блоке `/* cyrillic */`; расширенный —
`U+0460-052F` в `/* cyrillic-ext */`.

## Поставляемые файлы

Скачано **2026-09-09** через Google Fonts CSS API v2 (`https://fonts.googleapis.com/css2?…`)
с браузерным `User-Agent` — API отдаёт готовые `woff2` первоисточника. Взяты
только блоки `/* cyrillic */` и `/* latin */`; `latin-ext`, `cyrillic-ext`,
`greek`, `greek-ext`, `vietnamese` не скачивались. Это **выбор из готовых
файлов**, а не subsetting: каждый файл лежит ровно таким, каким его отдал
первоисточник, набор глифов внутри файла не менялся, поэтому запрет из раздела
«Подмножества не режем» не нарушен.

Начертания выбраны по фактическому коду: в `design/tokens.css` объявлены
`--vr-font-weight-regular: 400`, `--vr-font-weight-medium: 500`,
`--vr-font-weight-semibold: 600`, а `grep font-weight` по `renderer/src`
дополнительно даёт литералы `600`, `700` и `bold`. Итого нужны 400, 500, 600, 700. Курсивы не скачивались — `font-style: italic` в коде не встречается.

Переменный файл взят там, где Google Fonts его отдаёт (запрос `wght@400..700`
возвращает `font-weight: 400 700` одним файлом): IBM Plex Sans, Golos Text,
Literata, Manrope, JetBrains Mono, Onest. У IBM Plex Mono, Fira Sans и
Fira Sans Condensed variable-версии на Google Fonts нет — запрос с диапазоном
возвращает HTTP 400, поэтому для них взяты четыре статических начертания
(400/500/600/700) на подмножество.

| Файл                                     | Семейство           | Начертание / диапазон весов  | Подмножество | Размер  |
| ---------------------------------------- | ------------------- | ---------------------------- | ------------ | ------- |
| `fira-sans-400-cyrillic.woff2`           | Fira Sans           | статический 400              | `cyrillic`   | 10.5 КБ |
| `fira-sans-400-latin.woff2`              | Fira Sans           | статический 400              | `latin`      | 23.3 КБ |
| `fira-sans-500-cyrillic.woff2`           | Fira Sans           | статический 500              | `cyrillic`   | 10.6 КБ |
| `fira-sans-500-latin.woff2`              | Fira Sans           | статический 500              | `latin`      | 23.5 КБ |
| `fira-sans-600-cyrillic.woff2`           | Fira Sans           | статический 600              | `cyrillic`   | 11.3 КБ |
| `fira-sans-600-latin.woff2`              | Fira Sans           | статический 600              | `latin`      | 24.3 КБ |
| `fira-sans-700-cyrillic.woff2`           | Fira Sans           | статический 700              | `cyrillic`   | 11.3 КБ |
| `fira-sans-700-latin.woff2`              | Fira Sans           | статический 700              | `latin`      | 24.4 КБ |
| `fira-sans-condensed-400-cyrillic.woff2` | Fira Sans Condensed | статический 400              | `cyrillic`   | 10.6 КБ |
| `fira-sans-condensed-400-latin.woff2`    | Fira Sans Condensed | статический 400              | `latin`      | 23.5 КБ |
| `fira-sans-condensed-500-cyrillic.woff2` | Fira Sans Condensed | статический 500              | `cyrillic`   | 10.5 КБ |
| `fira-sans-condensed-500-latin.woff2`    | Fira Sans Condensed | статический 500              | `latin`      | 23.5 КБ |
| `fira-sans-condensed-600-cyrillic.woff2` | Fira Sans Condensed | статический 600              | `cyrillic`   | 11.3 КБ |
| `fira-sans-condensed-600-latin.woff2`    | Fira Sans Condensed | статический 600              | `latin`      | 24.4 КБ |
| `fira-sans-condensed-700-cyrillic.woff2` | Fira Sans Condensed | статический 700              | `cyrillic`   | 11.3 КБ |
| `fira-sans-condensed-700-latin.woff2`    | Fira Sans Condensed | статический 700              | `latin`      | 24.6 КБ |
| `golos-text-var-cyrillic.woff2`          | Golos Text          | переменный, диапазон 400–700 | `cyrillic`   | 21.5 КБ |
| `golos-text-var-latin.woff2`             | Golos Text          | переменный, диапазон 400–700 | `latin`      | 37.0 КБ |
| `ibm-plex-mono-400-cyrillic.woff2`       | IBM Plex Mono       | статический 400              | `cyrillic`   | 8.2 КБ  |
| `ibm-plex-mono-400-latin.woff2`          | IBM Plex Mono       | статический 400              | `latin`      | 14.4 КБ |
| `ibm-plex-mono-500-cyrillic.woff2`       | IBM Plex Mono       | статический 500              | `cyrillic`   | 8.3 КБ  |
| `ibm-plex-mono-500-latin.woff2`          | IBM Plex Mono       | статический 500              | `latin`      | 14.5 КБ |
| `ibm-plex-mono-600-cyrillic.woff2`       | IBM Plex Mono       | статический 600              | `cyrillic`   | 9.1 КБ  |
| `ibm-plex-mono-600-latin.woff2`          | IBM Plex Mono       | статический 600              | `latin`      | 15.3 КБ |
| `ibm-plex-mono-700-cyrillic.woff2`       | IBM Plex Mono       | статический 700              | `cyrillic`   | 8.5 КБ  |
| `ibm-plex-mono-700-latin.woff2`          | IBM Plex Mono       | статический 700              | `latin`      | 14.6 КБ |
| `ibm-plex-sans-var-cyrillic.woff2`       | IBM Plex Sans       | переменный, диапазон 400–700 | `cyrillic`   | 28.8 КБ |
| `ibm-plex-sans-var-latin.woff2`          | IBM Plex Sans       | переменный, диапазон 400–700 | `latin`      | 44.6 КБ |
| `jetbrains-mono-var-cyrillic.woff2`      | JetBrains Mono      | переменный, диапазон 400–700 | `cyrillic`   | 8.7 КБ  |
| `jetbrains-mono-var-latin.woff2`         | JetBrains Mono      | переменный, диапазон 400–700 | `latin`      | 30.7 КБ |
| `literata-var-cyrillic.woff2`            | Literata            | переменный, диапазон 400–700 | `cyrillic`   | 20.5 КБ |
| `literata-var-latin.woff2`               | Literata            | переменный, диапазон 400–700 | `latin`      | 38.1 КБ |
| `manrope-var-cyrillic.woff2`             | Manrope             | переменный, диапазон 400–700 | `cyrillic`   | 14.2 КБ |
| `manrope-var-latin.woff2`                | Manrope             | переменный, диапазон 400–700 | `latin`      | 24.3 КБ |
| `onest-var-cyrillic.woff2`               | Onest               | переменный, диапазон 400–700 | `cyrillic`   | 15.5 КБ |
| `onest-var-latin.woff2`                  | Onest               | переменный, диапазон 400–700 | `latin`      | 33.0 КБ |

**Итог:** 36 файлов, суммарно **688,5 КБ** (704 996 байт). Порог прироста
установщика — 1,5 МБ (SC-606); запас — около 848 КБ, то есть занято ~45 % бюджета.

Разбивка по семействам:

| Семейство           | Тип         | Веса               | Файлов | Суммарно |
| ------------------- | ----------- | ------------------ | ------ | -------- |
| IBM Plex Sans       | переменный  | 400–700            | 2      | 73,5 КБ  |
| IBM Plex Mono       | статический | 400, 500, 600, 700 | 8      | 92,7 КБ  |
| Golos Text          | переменный  | 400–700            | 2      | 58,5 КБ  |
| Literata            | переменный  | 400–700            | 2      | 58,6 КБ  |
| Manrope             | переменный  | 400–700            | 2      | 38,4 КБ  |
| JetBrains Mono      | переменный  | 400–700            | 2      | 39,4 КБ  |
| Fira Sans           | статический | 400, 500, 600, 700 | 8      | 139,2 КБ |
| Fira Sans Condensed | статический | 400, 500, 600, 700 | 8      | 139,7 КБ |
| Onest               | переменный  | 400–700            | 2      | 48,5 КБ  |

Проверка целостности: у всех 36 файлов первые четыре байта — `wOF2`
(`head -c4 <файл>`), минимальный размер — 8,2 КБ (`ibm-plex-mono-400-cyrillic.woff2`),
HTML-заглушек ошибки среди них нет.
