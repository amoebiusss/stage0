# Вариант #3

Выполнить задание согласно макету автора *Vladislav Chernov*: **[Online Zoo](https://www.figma.com/file/74wXlorl9mZQP0uhqDg83j/Online-Zoo)**  
Текст ссылки: https://www.figma.com/file/74wXlorl9mZQP0uhqDg83j/Online-Zoo


## Создание макета: неделя #1+2

Выполняется создание всех страниц для ширины экрана **1920px**.


### Технические требования

Максимальный балл: **80**


#### Общие

Все фоновые элементы макета должны растягиваться на всю доступную ширину экрана, если ширина больше 1920px. При этом направляющие должны сохраняться в исходном размере, 1800px. Особенностью этого проекта являются:
- интересная реализация боковой панели,
- разнообразие страниц,
- детализация эффектов.

Для создания вертикальных отступов лучше использовать вертикальные margin на блоках высшего порядка, насколько это возможно. При этом иметь ввиду, что вертикальные margin могут схлопнуться.

Для создание многоколоночных структур, или элементов имеющих относительное горизонтальное расположение, должно быть использовано одно из свойств:
- display: flex
- display: grid
- display: inline-block

Если на макете присутствуют тени (вокруг карточек, отзывов, фишек, под блоками или над ними), делать их точь-в-точь не обязательно, т.к. качество тени оцениваться не будет. Достаточно применить свойство box-shadow, чтобы было визуально похоже.

❗ Кнопки по умолчанию должны быть в состоянии "static". Если в макете указан цвет другого состояния, то все равно следует использовать состояние "static" из панели *Components*. Состояния "hover" и "active" приведены как пример интерактивности кнопок.

#### Landing (20 баллов)

1. **Header** (`<header>` содержит только логотип, панель навигации и иконку юзера)
- Логотип находится слева. Нажатие на логотип работает по принципу нажатия на `About`, перебрасывает нас на текущую страницу, на First Page. Landing. Более детальное описание лотипа будет в блоке *side bar*.
- Интерактивная панель навигации. (About / Map / Zoos / Contact Us / Design)
- Нажатие на `Map` перебрасывает нас на Zoos Map.
- Нажатие на `Zoos` перебрасывает нас на Zoos Translation с пандой.
- Нажатие на `Contact Us` перебрасывает нас на страницу с ошибкой 404.
- Нажатие на `Design` перебрасывает нас на оригинальную страницу [Figma](https://www.figma.com/file/74wXlorl9mZQP0uhqDg83j/Online-Zoo).
- Должен быть подсвечен первый элемент `About`. И он должен перестать быть интерактивным.
- На странице обязательно должен присутствовать один элемент `<h1>`. В нем должен быть текст `Online Zoo`.
- Хедер, за исключением логотипа, "липким" делать не нужно. Т.е. при скролле он остается на своей позиции.

2. **Side bar** (`<aside>` содержит кнопку "вверх", кнопки соц. сетей)
- ❗ Фоновый цвет и границы - не прозрачные.
- Панель слева: При скролле она должна "прилипнуть" к своей позиции, и всегда оставаться там вплоть до футера [position: fixed](https://developer.mozilla.org/ru/docs/Web/CSS/position#fixed_positioning).
- ❗ Можно сделать любую из интерпретаций:  
-- Логотипа может не быть, он будет только в хедере. Можно оставить сайдбар в виде, как он есть, на 115px от верха окна браузера. А можно сделать так, что сайдбар будет "отрываться", т.е. переходить в состояние `sticky` на расстоянии 25px от верхней границы окна браузера.  
-- Логотип может присутствовать в сайдбаре и в хедере, тогда он будет дублирован, оставаясь в обоих панелях.  
-- Логотип может быть только в сайдбаре, тогда при скролле он будет покидать позицию хедера.  
- При нажатии кнопки "вверх" может ничего не происходить.
- Интерактивная панель соцсетей. Нажатия на соцсети могут вести просто на заглавные страницы соотвествующих ресурсов.

3. Блок **Watch your favorite animal online**
- Кнопка `Choose zoo` должна быть интерактивной. Нажатие перебрасывает нас на Zoos Map.
- Кнопка `Watch online` должна быть интерактивной. Нажатие перебрасывает нас на Zoos Translation с пандой.

4. Блок **How zoo online works**
- Кнопка `Try now` должна быть интерактивной. Нажатие перебрасывает нас на Zoos Translation с пандой.
  
5. Блок **Famous pets**
- Кнопки влево и вправо должны быть интерактивными. При нажатии может ничего не происходить.
- Карточки животных должны быть интерактивными. [Пример анимации](https://drive.google.com/drive/folders/1yrzuAEEHFqkZn-4zkrlrYAHbNXdHOpRo), который также можно посмотреть во вкладке Components.

6. Блок **Pay and feed**
- Заголовки, текст, картинки, стрелки - это все разные элементы.

7. Блок **Testimonials**
- Кнопка `Leave Feedback` должна быть интерактивной. При нажатии может ничего не происходить.
- Кнопка `See more reviews` должна быть интерактивной. При нажатии может ничего не происходить.
- Кнопки влево и вправо должны быть интерактивными. При нажатии может ничего не происходить.

8. Блок **Zoogeography**
- На карте должно быть 4 интерактивных иконки. При наведении должна быть анимация, когда элемент увеличивается и граница меняет цвет. При нажатии может ничего не происходить.
- По умолчанию выбран Eagle, панель слева показывает описание. Описание может не меняться.
- Кнопка `Watch now` перебрасывает нас на Zoos Translation с соотвествующим животным. В случае с орлом - на страницу орла.

9. **Footer** (`<footer>` содержит меню, логотипы, кнопки доната и соц. сетей):
- Интерактивная панель навигации. По умолчанию, элементы не имеют подсветки. Каждая ссылка - это [якорь](https://webref.ru/course/html-tutorial/anchor), по нажатию на который нас перебрасывает на нужное место на странице:  
-- Watch online  
-- How it works  
-- Famous pets  
-- Pay & feed  
-- Testimonials  
-- Zoogeography  
- Кнопка `Donate for volunteers` должна быть интерактивной. При нажатии может ничего не происходить.
- Нажатие на основной логотип работает по принципу нажатия на About, перебрасывает нас на текущую страницу, на Landing.
- Остальные Логотипы не интерактивные. Они не должны реагировать на нажатие. Но должен появлятся тултип (атрибут title) с соотвествующей надписью (Yem Digital, Rolling Scopes School). При этом логотипы и промежуточное изображение могут быть центрированы по вертикали.
- Интерактивная панель соцсетей. Нажатия на соцсети могут вести просто на заглавные страницы соотвествующих ресурсов.
- ❗ В футере должен быть реализован 3х колоночный макет в рамках направляющих. При этом колонки могут быть равноразмерными. А можно подогнать их под размеры, указанные на макете. Несовпадение горизнотальных отступов не будет считаться ошибкой.


#### Zoos Map (10 баллов)

1. **Header** (`<header>` содержит только логотип, панель навигации и иконку юзера)
- Логотип находится слева. Нажатие на логотип работает по принципу нажатия на `About`, перебрасывает нас на *First Page. Landing*.
- Интерактивная панель навигации. (About / Map / Zoos / Contact Us / Design)
- Нажатие на `About` перебрасывает нас на Landing.
- Нажатие на `Zoos` перебрасывает нас на Zoos Translation с пандой.
- Нажатие на `Contact Us` перебрасывает нас на страницу с ошибкой 404.
- Нажатие на `Design` перебрасывает нас на оригинальную страницу [Figma](https://www.figma.com/file/74wXlorl9mZQP0uhqDg83j/Online-Zoo).
- Должен быть подсвечен элемент `Map`. И он должен перестать быть интерактивным.
- На странице обязательно должен присутствовать один элемент `<h1>`. В нем должен быть текст `Online Zoo`.
- Хедер, за исключением логотипа, "липким" делать не нужно. Т.е. при скролле он остается на своей позиции.

2. **Side bar** (`<aside>` содержит иконку логотипа, кнопки животных и стрелки)
- Фоновый цвет и границы - не прозрачные.
- Панель слева: Всегда будет в одной позиции, можно не делать "липкой".
- Интерактивная панель с животными. Нажатия на животных могут вести просто на заглавные страницы соотвествующих ресурсов.
- Стрелки вверх и вниз должны быть интерактивными. При нажатии может ничего не происходить.

3. Блок **Map**
- Иконки животных должны занимать свою позицию относительно карты.
- При наведении должна быть анимация, когда элемент увеличивается и граница меняет цвет. При нажатии может ничего не происходить.
- Карту можно зафиксировать в положении, как на дизайне. Главное, масштаб картинки должен соотвествовать такому же, как на дизайне.
- Не должно быть быть ни вертикального, ни горизонтального скролла.


#### Zoos Translation (10 x 5 = 40 баллов)
Требования для типовой страницы. Переход осуществляется по ссылкам типа `.../zoos/panda` или `.../zoos/gorilla`

1. **Header** (`<header>` содержит только логотип, панель навигации и иконки соц. сетей)
- Логотип находится слева. Нажатие на логотип работает по принципу нажатия на `About`, перебрасывает нас на *First Page. Landing*. Более детальное описание лотипа будет в блоке *side bar*.
- Интерактивная панель навигации. (About / Map / Zoos / Contact Us / Design)
- Нажатие на `About` перебрасывает нас на Landing.
- Нажатие на `Map` перебрасывает нас на Zoos Map.
- Нажатие на `Contact Us` перебрасывает нас на страницу с ошибкой 404.
- Нажатие на `Design` перебрасывает нас на оригинальную страницу [Figma](https://www.figma.com/file/74wXlorl9mZQP0uhqDg83j/Online-Zoo).
- Должен быть подсвечен элемент `Zoos`. И он должен перестать быть интерактивным.
- На странице обязательно должен присутствовать один элемент `<h1>`. В нем должен быть текст `Online Zoo`.
- Хедер, за исключением логотипа, "липким" делать не нужно. Т.е. при скролле он остается на своей позиции.

2. **Side bar** (`<aside>` содержит иконку логотипа, кнопки животных, вопросительный знак и стрелки)
- Фоновый цвет и границы - не прозрачные.
- Панель слева: При скролле она должна "прилипнуть" к своей позиции, и всегда оставаться там вплоть до футера [position: fixed](https://developer.mozilla.org/ru/docs/Web/CSS/position#fixed_positioning).
- ❗ Можно сделать любую из интерпретаций:  
-- Логотипа может не быть, он будет только в хедере. Можно оставить сайдбар в виде, как он есть, на 115px от верха окна браузера. А можно сделать так, что сайдбар будет "отрываться", т.е. переходить в состояние `sticky` на расстоянии 25px от верхней границы окна браузера.  
-- Логотипа может не быть, он будет только в хедере, но тогда должна быть кнопка "вверх" (как на странице *Landing*, просто стрелочка), которая может находится на месте логотипа. Нажатие будет поднимать страницу к самому верху.  
-- Логотип может присутствовать в сайдбаре и в хедере, тогда он будет дублирован, оставаясь в обоих панелях.  
-- Логотип может быть только в сайдбаре, тогда при скролле он будет покидать позицию хедера.  
- Интерактивная панель с кнопками животных. Нажатие перебрасывает нас на Zoos Translation с соотвествующим животным.
- При нажатии на "?" может ничего не происходить.
- Стрелки вверх и вниз должны быть интерактивными. При нажатии может ничего не происходить.

3. Блок **Main cam**
- В кнопке `Feed the animal` вместо animal должно быть название животного.
- Кнопка `Feed the animal` должна быть интерактивной. При нажатии может ничего не происходить.
- Блок видео - это элемент `iframe` с видео трансляции, его можно добавить на страницу по [инструкции](https://support.google.com/youtube/answer/171780?hl=ru).

4. Блок **Other cams**
- Картинки в карусели - это должны быть либо превью с youtube, либо такие же `iframe` с видео.
- При наведении на элемент видео, поверх должен появляться текст и затемняться картинка снизу. Такого эффекта можно достичь наложив полностью прозрачный элемент сверху, который не даст нажать видео, и ничего не произойдет. Эта заглушка нужна будет при работе с js.
- Кнопки со стрелками должны быть интерактивными. При нажатии может ничего не происходить.

5. Блок **Interesting facts**
- Если панели будут закрыты, и не смогут открыться - это будет считаться ошибкой. При этом выпадающие панели с информацией могут быть полностью раскрыты на момент выполнения недели#1-3, это не ошибка.
- Когда панель раскрыта, то на заголовке появляется "-" (будет везде в случае, если панели просто будут раскрыты). В случае закрытой панели, будет "+".
- Ссылки в тексте будут перебрасывать нас на соотвествующий ресурс.

6. Блок **Pay and feed**
- Заголовки, текст, картинки, стрелки - это все разные элементы.

7. **Footer** (`<footer>` содержит меню, логотипы, кнопки доната и соц. сетей):
- Интерактивная панель навигации. По умолчанию, элементы не имеют подсветки. Каждая ссылка - это [якорь](https://webref.ru/course/html-tutorial/anchor), по нажатию на который нас перебрасывает на нужное место на странице *Landing*:  
-- Watch online  
-- How it works  
-- Famous pets  
-- Pay & feed  
-- Testimonials  
-- Zoogeography  
- Кнопка `Donate for volunteers` должна быть интерактивной. При нажатии может ничего не происходить.
- Нажатие на основной логотип работает по принципу нажатия на About, перебрасывает нас на текущую страницу, на Landing.
- Остальные Логотипы не интерактивные. Они не должны реагировать на нажатие. Но должен появлятся тултип (атрибут title) с соотвествующей надписью (Yem Digital, Rolling Scopes School).
- Интерактивная панель соцсетей. Нажатия на соцсети могут вести просто на заглавные страницы соотвествующих ресурсов.
- В футере должен быть реализован 3х колоночный макет в рамках направляющих. При этом колонки могут быть равноразмерными. А можно подогнать их под размеры, указанные на макете. Несовпадение горизнотальных отступов не будет считаться ошибкой.

#### 404 Error (10 баллов)

1. **Header** (`<header>` содержит только логотип, панель навигации и иконки соц. сетей)
- Логотип находится слева. Нажатие на логотип работает по принципу нажатия на `About`, перебрасывает нас на текущую страницу, на First Page. Landing.
- Интерактивная панель навигации. (About / Map / Zoos / Contact Us / Design)
- Нажатие на `About` перебрасывает нас на Landing.
- Нажатие на `Map` перебрасывает нас на Zoos Map.
- Нажатие на `Zoos` перебрасывает нас на Zoos Translation с пандой.
- Нажатие на `Design` перебрасывает нас на оригинальную страницу [Figma](https://www.figma.com/file/74wXlorl9mZQP0uhqDg83j/Online-Zoo).
- Должен быть подсвечен элемент `Contact Us`. И он должен перестать быть интерактивным.
- На странице обязательно должен присутствовать один элемент `<h1>`. В нем должен быть текст `Online Zoo`.
- Хедер, за исключением логотипа, "липким" делать не нужно. Т.е. при скролле он остается на своей позиции.

2. Блок **Oops**
- Кнопка `Back to main page` должна быть интерактивной. Нажатие перебрасывает нас на Landing.
- Подсвеченная ссылка `click here to go to support` должна иметь интерактивность ссылки, но не должна никуда вести, т.к. мы уже на нужной странице.

3. **Footer** (`<footer>` содержит меню, логотипы, кнопки доната и соц. сетей):
- Интерактивная панель навигации. По умолчанию, элементы не имеют подсветки. Каждая ссылка - это [якорь](https://webref.ru/course/html-tutorial/anchor), по нажатию на который нас перебрасывает на нужное место на странице **Landing**:  
-- Watch online  
-- How it works  
-- Famous pets  
-- Pay & feed  
-- Testimonials  
-- Zoogeography  
- Кнопка `Donate for volunteers` должна быть интерактивной. При нажатии может ничего не происходить.
- Нажатие на основной логотип работает по принципу нажатия на About, перебрасывает нас на текущую страницу, на Landing.
- Остальные Логотипы не интерактивные. Они не должны реагировать на нажатие. Но должен появлятся тултип (атрибут title) с соотвествующей надписью (Yem Digital, Rolling Scopes School).
- Интерактивная панель соцсетей. Нажатия на соцсети могут вести просто на заглавные страницы соотвествующих ресурсов.
- В футере должен быть реализован 3х колоночный макет в рамках направляющих. При этом колонки могут быть равноразмерными. А можно подогнать их под размеры, указанные на макете. Несовпадение горизнотальных отступов не будет считаться ошибкой.

### Рекомендации:
- Сделать поп-ап *Profile* согласно шаблону. Выводить на экран на данном этапе не обязательно.


## Порядок оценки cross-check: неделя 1&2

Открываем на ширине экрана 1920px. Если экран меньше, можно сделать масштабирование, а можно поставить на странице ширину 1920px и смотреть со включенной горизонтальной плосой прокрутки. Если экран шире, можно поставить область уже или сузить окно.

❗ Балл не может опуститься ниже **0** за страницу. Если не указано в требованиях отдельно, то для всех блоков или элементов в состоянии покоя (без `hover`) справедливо:
- Отступы от границ элементов (или наборов элементов) до краев блока, по горизонтали или вертикали, отличаются на 10px или более: **-1** за каждый блок.
- Отступы внутри набора или сетки между элементами, по горизонтали или вертикали, отличаются на 5px или более: **-1** за каждый блок.
- Цвет фона блока или элемента сильно отличается от дизайна (например, отличие по каналу более чем на 32. #bbb и #ddd - не ошибка, больше - ошибка): **-1** за каждый блок.
- Отсуствует картинка как фоновая, так и картинка элемента: **-1** за каждый блок.
- Шрифт или семейство шрифтов не подключено: **-1** за каждый блок.


## Адаптивность: неделя #3

Сверстанные страницы адаптируюятся под следующую ширину экрана устройства:
- 1920px (уже будет готово)
- 1200px
- 640px
- 320px

### Технические требования

Максимальный балл: **40**

🚧 Задание в процессе разработки 🚧


## Функционалная часть и пользовательские события: неделя #4-5

Добавление JavaScript.

### Технические требования

Максимальный балл: **80**

🚧 Задание в процессе разработки 🚧
