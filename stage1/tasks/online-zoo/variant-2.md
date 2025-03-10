# Вариант #2

Выполнить задание согласно макету автора *DinaK*: **[Online Zoo Project](https://www.figma.com/file/lnK11foY8Aoa6oOlDXovVN/Online-ZOO-Project)**  
Текст ссылки: https://www.figma.com/file/lnK11foY8Aoa6oOlDXovVN/Online-ZOO-Project


## Создание макета: неделя #1+2

Выполняется создание всех страниц для ширины экрана **1920px**.


### Технические требования

Максимальный балл: **80**


#### Общие

Все фоновые элементы макета должны растягиваться на всю доступную ширину экрана, если ширина больше 1920px. При этом направляющие должны сохраняться в исходном размере, 1400px. Особенностью этого проекта являются:
- элементы, выходящие за границы направлюящих (карточки животных, отзывы),
- детально проработанные модальные окна.

Для создания вертикальных отступов лучше использовать вертикальные margin на блоках высшего порядка, насколько это возможно. При этом иметь ввиду, что вертикальные margin могут схлопнуться.

Для создания многоколоночных структур, или элементов имеющих относительное горизонтальное расположение, должно быть использовано одно из свойств:
- display: flex
- display: grid
- display: inline-block


#### Landing (20 баллов)

1. **Header** (`<header>` содержит только логотип, панель навигации и иконки соц. сетей)
- Логотип находится слева. Нажатие на логотип работает по принципу нажатия на `About`, перебрасывает нас на текущую страницу, на *First Page (Landing)*.
- Интерактивная панель навигации.
- Нажатие на `Map` перебрасывает нас на *Map Page*.
- Нажатие на `Zoos` перебрасывает нас на *Zoos Page Panda*.
- Нажатие на `Contact Us` перебрасывает нас на *Contact Us*.
- Нажатие на `Design` перебрасывает нас на оригинальную страницу [Figma](https://www.figma.com/file/lnK11foY8Aoa6oOlDXovVN/Online-ZOO-Project).
- Должен быть подсвечен первый элемент `About`. И он должен перестать быть интерактивным.
- Интерактивная панель соцсетей. Нажатия на иконки соцсетей могут вести просто на заглавные страницы соотвествующих ресурсов.
- На странице обязательно должен присутствовать один элемент `<h1>`. В нем должен быть текст `Online Zoo`.
- Хедер "липким" делать не нужно. Т.е. при скролле он остается на своей позиции.

2. Блок **Watch your favorite animal online**
- Кнопка `View live cam` должна быть интерактивной.  Нажатие перебрасывает нас на *Zoos Page Panda*.
- Бекграунд является картинкой.

3. Блок **Welcome to the zoo / How it works**
- Правильное расположение картинок относительно текста.

4. Блок **Your donation makes a difference**
- Input `$ Donation amount` должен быть типа number, со [cкрытыми стрелками](https://www.w3schools.com/howto/howto_css_hide_arrow_number.asp). Сам символ `$` при вводе сохраняется. На поле должно быть ограничение в 4 символа.
- Кнопка со стрелкой должна быть интерактивной. При нажатии может ничего не происходить.

5. Блок **Meet some our friends**
- Кнопки влево и вправо должны быть интерактивными. При нажатии может ничего не происходить.
- Карточки животных должны быть интерктивными. Нажатие на любую область карточки должно вести на страницу с соотвествующим животным. Если такого животного нет среди 4х представленных, то может ничего не происходить.
- ❗ При наведении курсора на карточку животного должна быть анимация [плавного увеличения на 20px в каждом из направлений относительно центра](https://thoughtbot.com/blog/transitions-and-transforms).
- Кнопка `Choose your favorite` должна быть интерактивной. При нажатии ведет нас на страницу `Map`.
- ❗ Справа карточки выходят за ширину направляющих. На ширине более 1920px остаток карточки должен переходить градиентом в цвет фона. Т.е. элементов не должно быть больше, чем доступно на 1920px. При этом, если сделано без затемнения или градиента, а карточки просто увеличиваются в количестве до края экрана справа, то это ошибкой считаться не будет.

6. Блок **Pay and feed**
- Кнопка `Donate now` должна быть интерактивной. При нажатии может ничего не происходить.

7. Блок **What our users think**
- Кнопки влево и вправо должны быть интерактивными. При нажатии может ничего не происходить.
- Кнопка `Leave feedback` должна быть интерактивной. При нажатии может ничего не происходить.
- Справа отзывы выходят за ширину направляющих. На ширине более 1920px новых отзывов появляться не должно. Т.е. элементов не должно быть больше, чем доступно на 1920px.

8. Блок **Care fro the animals you love**
- Картинки без надписей не должны быть интерактивными.
Карточки животных должны быть интерктивными. Нажатие на любую область карточки должно вести на страницу с соотвествующим животным. Если такого животного нет среди 4х представленных, то может ничего не происходить.
- При наведении курсора на карточку животного должна быть анимация [плавного увеличения на 20px в каждом из направлений относительно центра](https://thoughtbot.com/blog/transitions-and-transforms).
- Кнопка `Choose your favorite` должна быть интерактивной. Нажатие перебрасывает нас на *Map Page*.

9. **Footer** (`<footer>` содержит меню, логотипы, кнопки доната и соц. сетей):
- Интерактивная панель навигации. По умолчанию, элементы не имеют подсветки.
- Нажатие на `About` перебрасывает нас в верх страницы. Нажатие перебрасывает нас на верх текущей страницы, на *First Page (Landing)*.
- Нажатие на `Map` перебрасывает нас на Map Page.
- Нажатие на `Zoos` перебрасывает нас на Zoos Page Panda.
- Нажатие на `Contact Us` перебрасывает нас на Contact Us.
- Кнопка `Donate for volunteers` должна быть интерактивной.
- Нажатие на основной логотип работает по принципу нажатия на `About`, перебрасывает нас на верх текущей страницы, на *First Page (Landing)*.
- Остальные Логотипы не интерактивные. Они не должны реагировать на нажатие. Но должен появлятся тултип (атрибут title) с соотвествующей надписью (Yem Digital, Rolling Scopes School).
- Интерактивная панель соцсетей. Нажатия на иконки соцсетей могут вести просто на заглавные страницы соотвествующих ресурсов.


#### Map (10 баллов)

1. **Header** (`<header>` содержит только логотип, панель навигации и иконки соц. сетей)
- Логотип находится слева. Нажатие на логотип работает по принципу нажатия на `About`, перебрасывает нас на First Page. Landing.
- Интерактивная панель навигации.
- Нажатие на `About` перебрасывает нас на First Page. Landing.
- Нажатие на `Zoos` перебрасывает нас на Zoos Page Panda.
- Нажатие на `Contact Us` перебрасывает нас на Contact Us.
- Нажатие на `Design` перебрасывает нас на оригинальную страницу [Figma](https://www.figma.com/file/lnK11foY8Aoa6oOlDXovVN/Online-ZOO-Project?node-id=0%3A1).
- Должен быть подсвечен элемент `Map`. И он должен перестать быть интерактивным.
- Интерактивная панель соцсетей. Нажатия на соцсети могут вести просто на заглавные страницы соотвествующих ресурсов.
- На странице обязательно должен присутствовать один элемент `<h1>`. В нем должен быть текст `Online Zoo`.
- Хедер "липким" делать не нужно. Т.е. при скролле он остается на своей позиции.

2. Блок **Map**
- Иконки животных должны занимать свою позицию относительно карты.
- При наведении на иконку животного должен появится тултип с названием животного, локация. Обязательно для 4х животных, упомянутых в дизайне. Для остальных нужно иконки сделать неинтерактивными. По желанию, можно добавить подходящее описание в тултип.

3. **Footer** (`<footer>` содержит меню, логотипы, кнопки доната и соц. сетей):
- Интерактивная панель навигации. По умолчанию, элементы не имеют подсветки.
- Нажатие на `About` перебрасывает нас на First Page. Landing.
- Нажатие на `Map` перебрасывает нас на Map Page.
- Нажатие на `Contact Us` перебрасывает нас на Contact Us.
- Кнопка `Donate for volunteers` должна быть интерактивной.
- Логотипы не интерактивные. Они не должны реагировать на нажатие. Но должен появлятся тултип (атрибут title) с соотвествующей надписью (Online Zoo, Yem Digital, Rolling Scopes School).
- Интерактивная панель соцсетей. Нажатия на соцсети могут вести просто на заглавные страницы соотвествующих ресурсов.

#### Zoos page (10 x 4 = 40 баллов)
Требования для типовой страницы. Переход осуществляется по ссылкам типа `.../zoos/panda` или `.../zoos/lemur`

1. **Header** (`<header>` содержит только логотип, панель навигации и иконки соц. сетей)
- Логотип находится слева. Нажатие на логотип работает по принципу нажатия на `About`, перебрасывает нас на First Page. Landing.
- Интерактивная панель навигации.
- Нажатие на `About` перебрасывает нас на First Page. Landing.
- Нажатие на `Map` перебрасывает нас на Map Page.
- Нажатие на `Contact Us` перебрасывает нас на Contact Us.
- Нажатие на `Design` перебрасывает нас на оригинальную страницу [Figma](https://www.figma.com/file/lnK11foY8Aoa6oOlDXovVN/Online-ZOO-Project?node-id=0%3A1).
- Должен быть подсвечен элемент `Zoos`. И он должен перестать быть интерактивным.
- Интерактивная панель соцсетей. Нажатия на соцсети могут вести просто на заглавные страницы соотвествующих ресурсов.
- На странице обязательно должен присутствовать один элемент `<h1>`. В нем должен быть текст `Online Zoo`.
- Хедер "липким" делать не нужно. Т.е. при скролле он остается на своей позиции.

2. **Side bar** (`<aside>`)
- Панель слева: Должно быть подсвечено выбранное животное.
- Панель слева: При скролле, как только экран опускается ниже хедера, меню с животными должно "прилипнуть" к верху экрана. На этот счет ознакомьтесь с [position: sticky](https://medium.com/web-standards/sticky-bc7ff7088693).
- Выбранное животное становится не интерактивным, а также занимает первую позицию в списке.

3. Блок **Live cams**
- Кнопка `Donate now` должна быть интерактивной.
- Блок видео - это элемент `iframe` с видео трансляции, его можно добавить на страницу по [инструкции](https://support.google.com/youtube/answer/171780?hl=ru).
- Кнопки влево и вправо должны быть интерактивными.
- Картинки в карусели - это должны быть либо превью с youtube, либо такие же `iframe` с видео.
- Сверху, поверх видео, есть элемент, с надписью, какая это камера. Что касается самих видео - надо наложить полностью поверх прозрачный элемент, который не даст нажать видео, и ничего не произойдет. Эта заглушка нужна будет при работе с js.

4. Блок **Quick donate**
- Input `$ Donation amount` должен быть типа number, со cкрытыми стрелками.
- Кнопка со стрелкой должна быть интерактивной.

5. Блок **Did you know?**
- Тени вокруг блока должны быть сделаны свойством box-shadow. Даже если визуально они будуь выглядеть чуть-чуть иначе.
- Кнопка `View Map` должна быть интерактивной. При нажатии перебрасывает нас на Map Page.
  
6. **Footer** (`<footer>` содержит меню, логотипы, кнопки доната и соц. сетей):
- Интерактивная панель навигации. По умолчанию, элементы не имеют подсветки.
- Нажатие на `About` перебрасывает нас на First Page. Landing.
- Нажатие на `Map` перебрасывает нас на Map Page.
- Нажатие на `Contact Us` перебрасывает нас на Contact Us.
- Кнопка `Donate for volunteers` должна быть интерактивной.
- Логотипы не интерактивные. Они не должны реагировать на нажатие. Но должен появлятся тултип (атрибут title) с соотвествующей надписью (Online Zoo, Yem Digital, Rolling Scopes School).
- Интерактивная панель соцсетей. Нажатия на соцсети могут вести просто на заглавные страницы соотвествующих ресурсов.

#### Contact us (10 баллов)

1. **Header** (`<header>` содержит только логотип, панель навигации и иконки соц. сетей)
- Логотип находится слева. Нажатие на логотип работает по принципу нажатия на `About`, перебрасывает нас на текущую страницу, на First Page. Landing.
- Интерактивная панель навигации.
- Нажатие на `About` перебрасывает нас на First Page. Landing.
- Нажатие на `Map` перебрасывает нас на Map Page.
- Нажатие на `Zoos` перебрасывает нас на Zoos Page Panda.
- Нажатие на `Design` перебрасывает нас на оригинальную страницу [Figma](https://www.figma.com/file/lnK11foY8Aoa6oOlDXovVN/Online-ZOO-Project?node-id=0%3A1).
- Должен быть подсвечен первый элемент `Contact us`. И он должен перестать быть интерактивным.
- Интерактивная панель соцсетей. Нажатия на соцсети могут вести просто на заглавные страницы соотвествующих ресурсов.
- На странице обязательно должен присутствовать один элемент `<h1>`. В нем должен быть текст `Online Zoo`.
- Хедер "липким" делать не нужно. Т.е. при скролле он остается на своей позиции.
  
2. Блок **Get in touch**
- Нужно реализовать форму
- Поля (input, textarea), помеченные звездочкой, должны быть обязательными для заполнения, т.е. required. Если при нажатии на кнопку `send message` хоть одно поле не проходит валидацию, запрос не должен быть отправлен.
- Поле Your Email Address должна проходить валидацию типа email.
- Кнопка `Send Message` должна быть интерактивной.
  
3. **Footer** (`<footer>` содержит меню, логотипы, кнопки доната и соц. сетей):
- Интерактивная панель навигации. По умолчанию, элементы не имеют подсветки.
- Нажатие на `About` перебрасывает нас на First Page. Landing.
- Нажатие на `Map` перебрасывает нас на Map Page.
- Нажатие на `Contact Us` перебрасывает нас на Contact Us.
- Кнопка `Donate for volunteers` должна быть интерактивной.
- Логотипы не интерактивные. Они не должны реагировать на нажатие. Но должен появлятся тултип (атрибут title) с соотвествующей надписью (Online Zoo, Yem Digital, Rolling Scopes School).
- Интерактивная панель соцсетей. Нажатия на соцсети могут вести просто на заглавные страницы соотвествующих ресурсов.


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
