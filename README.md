# MediasoftAnalitycsTask
Медиасофт Аналитика

Дано:

Мобильное клиент-серверное приложение "Soul Light" (приложение для продажи украшений)
Необходимо описать:
1. Бизнес-процесс создания заказа (использовать любую удобную нотацию моделирования бизнес-процессов).

Выполненное задание представлено в файле "diagram.svg", код которого находится в файле "diagram.bpmn"

2. Опишите процесс синхронизации данных между клиентом и сервером (создание, редактирование и отмена заказа, изменение персональных данных, оплата заказа и т.д.). Представить все в диаграммах UML, API методах и других представлениях, также составить ER-диаграмму сущностей.

В файле "UML Activity.png" представлена диаграмма UML Activity.

В файле "ERD.png" представлена ER-диаграмма сущностей. Более подробно с ней можно ознакомиться по ссылке 

https://drive.google.com/file/d/1rI1UmVGnFQHwu6Mf0JBzboAHIZpnjCT0/view?usp=sharing

Диаграмма UML sequence представлена в файле "UML Создание заказа.PNG", код диаграммы, созданный с помощью платформы PlantUML, находится в файле "UML Создание, оплата заказа". В ней представлено взаимодействие клиента и сервера при оформлении заказа, оплате и частичном редактировании персональных данных (Внесение или изменение данных для доставки) 

API-методы представлены с помощью таблицы в файле "API-методы.pdf"


3. Подготовить прототип одного из экранов данного мобильного приложения и описать пользовательский интерфейс для данного экрана (например, создание заказа).

Прототипы для главного экрана приложения и экрана корзины (создания заказа) представлены в файле "Прототип экранов приложения.pdf"

Главный экран приложения

На главном экране в левом верхнем углу находится название магазина (приложения), справа от него находится кнопка "Уведомления", при нажатии на которую пользователь может увидеть личные уведомления. Ниже находится строка поиска по магазину. Основную часть пространства занимает каталог магазина, на котором сверху представлены актуальные акции магазина а ниже расположены рекомендуемые/популярные товары. Под каждым фото товара представлено его наименование и цена. В самом низу находится главная плашка навигации. Если смотреть слева на право, то первой стоит иконка, при нажатии на которую пользователь переходит на главный экран приложения. Вторая иконка отправляет пользователя на страничку с каталогом товаров, в котором представлены типы украшений, пользователь может выбрать подходящее и перейти на страничку, где предложенные товары будут соответствовать выбранному типу. По середине, третьей, находится кнопка "Корзина", при нажатии на которую пользователь переходит в свою корзину товаров. Четвертая кнопка отправляет пользователя на страницу с его избранными товарами. Последняя кнопка переносит пользователя в его личный кабинет.

Корзина

Сверху экрана отображается название приложение, ниже находится наименование страницы "Корзина". В самом низу находится главная плашка навигаций. Основную часть занимают товары, находящиеся в корзине. Фото товаров располагается с левой стороны экрана. Справа от каждого фото сверху вниз располагаются цена, наименование товара, описание, количество данного товара в корзине, которое можно редактировать с помощью интерактивных кнопок увеличения/уменьшения количества товара, и сумма за выбранное количество данного товара. В правом верхнем углу пространства, которое занимает описание товара, находится интерактивная кнопка выбора, при нажатии на которую пользователь добавляет выбранный товар в формирующийся заказ, данный товар выделяется, а сама кнопка меняет цвет. Выше главной плашки навигации находятся данные о заказе и кнопка "Оформить заказ". Данные о заказе включают в себя количество выбранных позиций, скидка и итоговая сумма заказа. При нажатии на кнопку "Оформить заказ" пользователю предлагают ввести данные для доставки и далее оплатить заказ онлайн.

4. Подготовить подробное описание функции редактирования заказа , которую можно было бы использовать в качестве постановки задачи для разработки (помимо текстового описания, использовать UML диаграммы, указать используемые API методы, передаваемые и получаемые параметры, описать процесс хранения информации о покупках пользователя). 

5. Перед вами реляционная модель данных. Необходимо написать SQL-запросы.

- Вывести покупателей с количеством осуществленных покупок
- Общую стоимость товаров для каждого покупателя и отсортировать результат в порядке убывания
- Получить покупателей, купивших только один товар
