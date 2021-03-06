# Техническое задание на вёрстку

* Название сайта: Глейси
* Домен: пока нет

---

1.  **Общие технические требования**

 * 1.1 Стандарты вёрстки: HTML5, CSS3, прогрессивное улучшение.
 * 1.2 Сетка: четыре колонки равной ширины (22.2%).
 * 1.3 Два варианта вёрстки:
	- под фиксированную ширину `900px` или `1200px`: с центровкой основного контента, с некоторыми блоками, которые тянутся на всю ширину;
	- с дополнительной резиновостью (необязательный вариант): диапазон ширин от `900px` до `1200px`.
 * 1.4 Используемые фреймворки: нет.
 * 1.5 Кроссбраузерность: IE10+, Chrome, Firefox, Opera, Safari.
 * 1.6 Типографика: частично определена в макете (прочее — на усмотрение разработчика).
 * 1.7 Используемый шрифт: Roboto (есть в папке с макетом и на Google Fonts).
 * 1.8 С макетом предоставлен `styleguide.psd`, содержащий прорисовку состояний элементов интерфейса. При любых расхождениях с макетами он должен иметь наивысший приоритет.

2.  **Пояснения для учащихся**

 * 2.1 В макетах есть скрытые слои с всплывающими окнами. Такие слои в блоке слоёв фотошопа выделены красным цветом.
 * 2.2 Макеты верстаются постепенно, не нужно сразу выполнять все требования.
 * 2.3 Ниже в разделе «Обязательные требования» описано поведение блоков, которое должно быть реализовано для получения допуска. Требования из раздела «Дополнительные требования» можно реализовать по желанию для выполнения дополнительных критериев. Некоторые размеры описаны в процентной ширине. Если вы выбрали вариант вёрстки с дополнительной резиновостью, то следуйте указанным процентам. Если вы выбрали вёрстку с фиксированной шириной, то проценты помогут вам высчитать правильные размеры блоков в пикселях.

3.  **Обязательные требования**

   **Все макеты:**

  * 3.1 Контентная область центрируется и не может быть уже макетной ширины.
  * 3.2 Внутренние отступы слева и справа для обеих страниц — по 2.3% от ширины всей контентной области.
  * 3.3 Отступы между колонками сетки одинаковые — по 2.2% от ширины всей контентной области.
  * 3.4 При достижении `1200px` сетка перестаёт масштабироваться дальше.
  * 3.5 Главное меню — при наведении на пункт меню «Каталог» появляется подменю (смотрите папку слоёв «Ховеры» в `gllacy-index.psd`).
  * 3.6 Главное меню — пункт подменю «Сливочное» должен вести на внутреннюю страницу (`gllacy-catalog.psd`).
  * 3.7 Шапка — при наведении на кнопку поиска появляется форма для ввода текста (смотрите папку слоёв «Ховеры» в `gllacy-index.psd`).
  * 3.8 Шапка — при наведении на кнопку «Вход» появляется форма для авторизации (смотрите папку слоёв «Ховеры» в `gllacy-index.psd`).
  * 3.9 Шапка — Если пользователь добавил что-то в корзину, соответствующий пункт в шапке страницы меняет цвет фона на белый. При наведении на этот пункт появляется форма с товарами (смотрите папку слоёв «Ховеры» в `gllacy-index.psd`).

   **gllacy-index.psd:**

  * 3.10 Логотип не является ссылкой.
  * 3.11 Карусель под шапкой страницы: слайдер. Вёрстка всех слайдов обязательна. Оживление слайдера необязательно, принцип оживления описан в 4 разделе.
  * 3.12 Блок карты — достаточная реализация — обычное изображение.
  * 3.13 Вёрстка модального окна обязательна (смотрите папку слоёв «Обратная связь»).
  * 3.14 Карточка товара: поведение этого элемента при наведении на главной странице аналогичны поведению на странице каталога (смотрите в `styleguide.psd`).

   **gllacy-catalog.psd:**

  * 3.15 Логотип — это ссылка на главную страницу.
  * 3.16 В хлебных крошках пункт «Главная» — это ссылка на главную страницу.
  * 3.17 Фильтр: верстать с помощью формы, кнопка «Применить» отвечает за отправку формы.
  * 3.18 Блок «Цена» — при наведении на любой из маркеров появляется указатель `cursor: pointer`, делать маркеры подвижными не обязательно, цена меняться не должна.
  * 3.19 Количество товаров может быть любым, оно не должно ломать страницу.

4.  **Дополнительные требования**

   **gllacy-index.psd:**

  * 4.1 Карусель под шапкой страницы: оживление слайдера. Cмена слайдов мгновенная, без промежуточных переходов. При смене слайдов происходит смена фонового цвета на всей странице (смотрите папку слоёв «Фон» в `gllacy-index.psd`).
  * 4.2 Блок карты — реализация по желанию — интерактивная карта, которая также масштабируется на 100% ширины, на карте размещён маркер. Допустимо использовать как стандартный, так и кастомный маркер.
  * 4.3 По клику на кнопку «форма обратной связи» возникает модальное окно с формой отправки сообщения (смотрите папку слоёв «Ховеры» в `gllacy-index.psd`), окно позиционируется относительно вьюпорта, а не страницы. При вводе текста в поле формы, «плейсхолдер» должен отобразиться над полем (смотрите папку слоёв «Фидбек» в `styleguide.psd`). Достаточно реализации с обычными плейсхолдерами.

   **gllacy-catalog.psd:**

  * 4.4 Фильтр: при выключенном JavaScript кнопка «Применить» должна осуществлять переход на отдельную страницу (отдельную страницу верстать не нужно).
