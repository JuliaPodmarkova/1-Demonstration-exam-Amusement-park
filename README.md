1	ИТОГОВЫЙ ДЕМОНТРАЦИОННЫЙ ЭКЗАМЕН

Тема «Задание итогового демонстрационного экзамена»

Цель
Научиться создавать и настраивать новую информационную систему.

Порядок работы
1.	Изучить введение, ресурсы и описание задачи.
2.	Выполнить задания для самостоятельной работы.
3.	Изучить критерии оценки.

Введение и описание задания

Введение
В задании на демонстрационный экзамен в качестве основного учетного механизма предполагается использование механизмов оперативного учета технологической платформы 1С: Предприятия 8. Кроме этого, могут быть проверены знания по другим возможностям платформы – внимательно изучите всё задание и выданные ресурсы перед тем, как приступить к работе.
Поскольку модули задания предназначены для проверки понимания механизмов платформы, а не для реального внедрения, при их разработке были приняты некоторые упрощения и допущения:
−	в постановке задач существуют некоторые условности и упрощения. Например, в некоторых задачах не учитываются налоги, используются упрощенные алгоритмы расчета и т.п.;
−	так как время решения задачи ограничено, то следует реализовывать именно те задачи, которые описаны в задании явно. Например, следует реализовать учет остатков товаров на складах, а про ценообразование ничего не сказано, следовательно, его вести не надо;
−	часть механизмов оставлено на усмотрение решающего задачу. Так, если в задании указано только как списывается товар, то механизм его поступления выполняющий задание может выбрать самостоятельно. Если в задании в явном виде не указан механизм формирования отчета, то отчет надо уметь строить любым из перечисленных способов: с использованием компоновки данных, построителя отчетов, сводной таблицы, а в некоторых случаях использовать фиксированный макет.
С другой стороны, при решении любой из задач необходимо учитывать ряд дополнительных требований:
−	внешний вид форм и интерфейсов, если это явно указано в задаче – должны выглядеть так, как это указано на скриншотах;
−	состав объектов конфигурации и их структуру для выполнения поставленных задач необходимо самостоятельно определить и реализовать. Если информационная база 1С не выдана в ресурсах – создайте её;
−	в состав ресурсов входит обработка «Консоль запросов», предназначенная для облегчения работы и отладки создаваемого прикладного решения;
−	в том случае, когда в задании приведен пример с заполненными в режиме 1С: Предприятия данными, желательно производить отладку решения именно на данных из примера.
При решении задач рекомендуется использовать встроенную в платформу документацию и синтаксис-помощник. 
На проверку следует передавать законченное решение – с прокомментированным программным кодом, без ошибок в коде и во времени выполнения, выдающее понятную обратную связь пользователю при выполнении ключевых операций. 
Описание задания
Вам необходимо разработать приложение и базу данных для Парка аттракционов. Заказчик предоставил вам комплект документации и дополнительные файлы (ресурсы), чтобы вы могли разработать систему в соответствии с его потребностями. 
Документация к системе
Пожалуйста, внимательно изучите задание и все файлы к заданию (ресурсы). Это поможет вам понять, что именно необходимо разработать. При разработке вы должны придерживаться указанного в задании вида интерфейсных объектов.
Именование
Если имя какого-либо элемента системы не указано, вы должны его придумать. При этом (в схеме именования) необходимо следовать логике. То есть следить за тем, чтобы выбранное имя как можно точнее отражало суть того или иного элемента системы, его назначения и, при необходимости, совпадало с именем, приведенном в соответствующем окне. Это позволит существенно сократить время на обучение сотрудников работе с системой.

Задания для самостоятельной работы:
Задание 1. Создание конфигурации
Запустите 1С и создайте новую информационную базу, после чего в режиме Конфигуратора добавьте необходимые для задач этой сессии объекты метаданных.
На данном этапе нет необходимости создавать все предлагаемые для решения задач будущих задач объекты конфигурации – просто учтите, что именно созданная вами сейчас система будет использоваться и развиваться на протяжении всех заданий (если не оговорено отдельно). 

Задание 2. Добавление в объекты конфигурации списков, связанных с работой Парка
В этом модуле следует реализовать возможность хранения и ввода информации, связанной с внутренним устройством компании.
При создании списков данного вида необходимо учитывать следующие особенности:
1.	В системе необходимо хранить информацию о том, в каком подразделении работает сотрудник и какую должность в этом подразделении он занимает.
2.	Каждый сотрудник может работать только в одном подразделении и занимать только одну должность
3.	Компания состоит из отдельных подразделений. Структура подразделений Парка выглядит следующим образом:
−	Администрация
−	Бухгалтерия
−	Техническая поддержка
−	Обслуживание гостей.
4.	Форма списка сотрудников определена заказчиком на рис. 1.1.

 

Рис. 1.1. Форма списка сотрудников

5.	Карточка сотрудника определена заказчиком на рис. 1.2.

 

Рис. 1.2. Карточка сотрудника


Задание 3. Добавление в объекты конфигурации списков, связанных с Ценообразованием
В этом модуле следует реализовать возможность хранения и ввода информации, связанной с учетом цен.
При создании списков данного вида необходимо учитывать следующие особенности:
1.	Вид создаваемых форм должен полностью совпадать с представленными в задании (рис. 1.3, 1.4).
2.	Основная форма ввода данных о ценах на билеты определена заказчиком на рис. 1.3.
3.	Значение в поле «Тип билета» может принимать одно из трех возможных значений:
−	Взрослый
−	Детский (от 3-х до 12 лет)
−	Льготный (от 60 лет)

 

Рис. 1.3. Форма ввода данных о ценах на билеты

4.	Перечень типов билетов с ценами представлен на рис. 1.4.

 

Рис. 1.4. Перечень типов билетов

Задание 4. Добавление в объекты конфигурации списков, связанных с посещением аттракционов
В этом задании следует реализовать возможность хранения и ввода информации, связанной с посещением аттракционов.
При создании списков данного вида необходимо учитывать следующие особенности:
1.	Каждый аттракцион уникален и расположен в конкретной зоне Парка
2.	Количество аттракционов и зон парка не ограничено.
3.	Форма аттракциона определена заказчиком на рис. 1.5.

 

Рис. 1.5. Форма аттракциона

4.	При работе с формой аттракциона необходимо предусмотреть возможность размещения его фотографии. Фотографии аттракционов должны храниться в информационной базе, но при этом первоначально загружаться из внешнего файла. 

Задание 5. Загрузка данных в созданные списки
Заказчик предоставил вам исходные данные для автоматической загрузки, чтобы создаваемая информационная база сразу могла выполнять поставленные задачи. Кроме этого, некоторые данные нужно ввести вручную. Следует внимательно изучить переданные файлы и корректно импортировать данные из них в соответствующие объекты конфигурации. Если какие-то объекты ранее созданы не были – создайте их.
1.	Данные об аттракционах представлены в файле «Аттракционы.xlsx» предназначены для программной загрузки.
2.	Данные о сотрудниках компании представлены в файле «Сотрудники.xlsx» предназначены для программной загрузки.
3.	Коллекция файлов с фотографиями аттракционов представлены в папке «Фото аттракционов».
Имейте, пожалуйста, ввиду: какие-то данные не отформатированы для импортирования непосредственно в базу данных, какие-то отформатированы. К сожалению, предыдущий программист не уделял вопросам форматирования данных должного внимания. Вам необходимо отформатировать данные и загрузить их в таблицы, которые Вы только что создали. Загрузка этих данных нужна для первоначального заполнения базы, поэтому Вы сами решайте, как эти данные отформатировать / преобразовать. Главное, чтобы данные полностью были загружены в систему, без потерь. 
Если для загрузки Вы будете преобразовывать исходные данные, то не забудьте задокументировать этот процесс и приложить файлы с подготовленными данными. Не факт, что перед запуском рабочей системы Вы лично будете производить первоначальную загрузку данных.
Внимание! Механизм импорта определите и реализуйте самостоятельно.

Задание 6. Создание списка Заказов на посещение аттракционов
Для посещения Парка аттракционов клиент на сайте компании заполняет специальную форму заказа (рис. 1.6). 
Далее на основании введенных в форму данных в информационной базе должен быть сформирован документ «Заказ». В предлагаемой задаче каждый заказ формируется вручную в режиме 1С: Предприятия (в пользовательском режиме).
1.	Заказчик предоставил вам форму Заказа для ознакомления с составом полей и реквизитов. 
2.	Настройте внешний вид формы, используя в том числе и дополнительные надписи (рис. 1.6) 

 

Рис. 1.6. Форма заказа

3.	При работе с заказами необходимо реализовать Проверку на обязательное заполнение следующих полей:
−	Дата посещения Парка аттракционов
−	Тип билета и количество (в табличной части)
−	Номер телефона клиента и его электронная почта
4.	Также необходимо реализовать следующие возможности:
−	Значения поля «Цена 1 билета» должны заполняться автоматически, после заполнения поля «Тип билета»;
−	Стоимость билета рассчитывается автоматически после ввода количества в каждой строке таблицы по формуле: «Цена 1 билета» * «Количество».
−	Информация об общем количестве билетов в заказе и сумме к оплате должны быть рассчитаны автоматически.

Задание 7. Создание списка объектов конфигурации, фиксирующих оплаты
1.	Прием денег от клиентов осуществляются кассиром по номеру заказа и на основании документа «Заказ» (рис. 1.6). 
При этом кассир указывает аттракцион, на который был сформирован заказ.
2.	Оплата должна быть произведена полностью. Частичная оплата – запрещена. 
3.	Форма документа приема денег представлена на рис. 1.7. 

 

Рис. 1.7. Форма документа оплата

4.	Дополнительно, при работе в форме оплаты необходимо реализовать следующие возможности:
−	Проверку на обязательное заполнение всех полей
−	Сумма оплаты вводится автоматически на основании заказа. 

Задание 8. Создание отчетов
1.	Для анализа работы кассиров в системе формируется отчет по проданным билетам за выбранный период. 
2.	Отчет должен содержать таблицу и диаграмму.

Задание 9. Создание подсистем
Создайте три подсистемы и поместите в них соответствующие объекты:
−	Подсистема «Аналитика»: все справочники и перечисления, отчеты и обработки.
−	Подсистема «Бухгалтерия»: документ Оплата.
−	Подсистема «Сервис» документ Заказ.
