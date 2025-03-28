
# Список реализованных роботов
## Ниже приведён список уже реализованных роботов в органах власти (и не только)


### Комитет по Финансам
| Номер | Название                            |
| ----- | :---------------------------------- |
| 1     | Сверка с план-графиком и подписание |
| 2     | Контроль исполнения и подписание    |
| 3     | Контроль изменения сведений в ГК    |
| 4     | Проверка актов СБИС и подписание    |
| 5     | Контроль сведений в ГК              |

### Жилищный Комитет

| Номер | Название                                                     |
| ----- | :----------------------------------------------------------- |
| 1     | Внесение изменений в региональную программу капитального ремонта |
| 2     | Сводный отчет по уборке зима/лето                            |
| 3     | Поиск по ИНН по реестрам для закупок                         |
| 4     | Проверка реестра добросовестных поставщиков                  |
| 5     | Тарифная разница - проверка в ГИС ЖКХ                        |
| 6     | Тарифная разница - проверка актов                            |
| 7     | Внесение данных в ИС Расселение комун. Квартир (ГорЖилОбмен) |
| 8     | Формирование списка первоочередников (ГорЖилОбмен)           |
| 9     | Сбор сводного отчета и рассылка по отчётам ГУЖА         |
| 10     | Робот для Жилкома по обработке обращений граждан в ССТУ|

1. Внесение изменений в региональную программу капитального ремонта

   > Робот считывает текст постановления формата word, далее согласно тексту вносит изменения в таблицу эксель в части изменения наименований (пр. в пункте 2 строки 3 таблицы заменить “Дунайская д.1 литер А” на “ул. Дунайская д.1 литера А), добавляет или исключает пункты или отдельные строки пункта

2. Сводный отчет по уборке зима/лето

   > Робот получает отчет в формате эксель от 18 районов с почтового ящика, обрабатывает отчет и записывает данные в сводную таблицу. Отправляет ответ отправителю отчета в формате “Здравствуйте, Ваш отчет принят”, либо “Отчет не принят. Проверьте пункт “Средства малой механизации”, или “Отчет не соответствует формату” и т.д 

3. Поиск по ИНН по реестрам для закупок

   > Поиск информации по определенному ИНН на перечне сайтов, формирование скриншотов и сводного файла по проверке (содержит инн, название организации, скриншот)

4. Проверка реестра добросовестных поставщиков

   > Проверка кандидатов для включения в этот реестр (по сути тоже самое, только другой док проверяет) Проверяет участников реестра со статусом “действующий” на перечне сайтов, при расхождениях - делает скриншот и сохраняет ссылку для проверки сотрудником в целях исключения участника из реестра 

5. Тарифная разница - проверка в ГИС ЖКХ

   > Робот проверяет список адресов МКД в файле эксель на правильно указанную управляющую компанию на сайте ГИС ЖКХ. Помимо этого для правильного поиска (в файле часто указывается неполный адрес) обращается к сайту ФИАС

6. Тарифная разница - проверка актов

   > По каждому адресу или контракту робот находит подписанный акт сверки тарифов в формате HTML, анализирует, выделяет цветом поля номер контракта, дата заключения, адрес, суммы

7. Внесение данных в ИС Расселение комун. Квартир (ГорЖилОбмен) 

8. Формирование списка первоочередников (ГорЖилОбмен)

9. Сбор сводного отчета ГУЖА

   > Робот собирает с почты полученные ежедневные акты об выполненной уборке в разных кадастровых кварталах, берет с них данные и сводит в единый сводный отчет. 

10. Рассылка по отчетам ГУЖА

    > Робот преобразует полученные в xlsx формате ежедневные акты в pdf и еженедельно выполняет рассылку сводного отчета с недельным срезом в администрации района
### Комитет по Экономической Политике и Стратегическому Планированию

| Номер | Название              |
| ----- | :-------------------- |
| 1     | Формирование НМЦК     |
| 2     | Сбор данных о закупке |

1. Формирование НМЦК

    > Робот проходит по каждому товару/услуге из списка закупок. Ищет нужную позицию в документах комитета госзаказа, если не находит - собирает коммерческие предложения из интернета (с помощью сайта РТС Тендер). Далее вставляет информацию ф заданную таблицу и рассчитывает нмцк на всю закупку. В процессе поиска КП делает скриншоты 

2. Сбор данных о закупке

    > Пользователь заполняет таблицу-шаблон в которой указываются фильтры для поиска (наименование, код ОКПД2, даты). 	Робот считывает данные и ищет на сайте госзакупки и при нахождении требуемой позиции собирает данные по объекту закупки и данные о контракте и заносит в отдельный exel файл.

### Комитет по Транспорту

| Номер | Название                                  |
| ----- | :---------------------------------------- |
| 1     | Сведения о выполнении транспортной работы |

### Комитет по Благоустройству

| Номер | Название                       |
| ----- | :----------------------------- |
| 1     | Регистрация заявок в ЕСЭДД     |
| 2     | Направление платежек в ГИС ГМП |

1. Регистрация заявок в ЕСЭДД

    > Робот собирает с почты письма на основании которых необходимо создать заявку на ЕСЭДе. Робот высылает excel форму, пользователям, для заполнения. После получения заполненной формы робот заходит на ЕСЭД и регистрирует заявку прикрепляя приложенную к письму документацию (pdf).

2. Направление платежек в ГИС ГМП

    > Робот забирает информацию (штрафные начисления) из облачной версии 1с КомФина и переносит информацию в ЕКДЛ, откуда данные уже переносятся в ГИС ГМП

### Комитет по Здравоохранению

| Номер | Название                                                     |
| ----- | :----------------------------------------------------------- |
| 1     | Внесение в реестр граждан по коду 707                        |
| 2     | Выгрузка формы 090/у                                         |
| 3     | Выгрузка формы 027/у                                         |
| 4     | Робот для сбора информации по формам 090/у и 027/у по районам |
| 5     | Внесение данных в 6s                                         |
| 6     | Формирование отчётности для экономического отдела            |
| 7     | Проверка лекарственных препаратов на сайте Госздравнадзора            |

1. Внесение в реестр граждан по коду 707  

> Робот входит в систему, там появляется список пациентов, которых нужно включить в реестр если нет галочек. Проверяется каждая запись на галки - если их нет - заходит в реестровую запись,  отжимается кнопка включить в реестр по коду (707 или 710).

### Архивный Комитет

| Номер | Название                        |
| ----- | :------------------------------ |
| 1     | Конвертация файлов из wav в mp3 |
| 2     | Замена файлов на портале        |

1. Конвертация файлов из wav в mp3 

> Форматирование аудио файлов в формат mp3 для сокращения места для диске.

2. Замена файлов на портале  

> Робот заходит в закрытую систему, скачивает файл в формате wav, форматирует его в mp3, заменяет файл в системе в целях экономии места.

### Комитет Территориального Развития

| Номер | Название                                   |
| ----- | :----------------------------------------- |
| 1     | Поиск по ключевым словам                   |
| 2     | Робот по направления в инцидент-менеджмент |

### Комитет по Государственному Заказу

| Номер | Название                                                    |
| ----- | :---------------------------------------------------------- |
| 1     | Проверка на сайте государственных закупок цен по контрактам |
| 2     | Сбор данных для нужд комитета с ЕИС                         |
| 3     | Поиск по ИНН по реестрам для закупок                        |

### Комитет государственной службы и кадровой политики

| Номер | Название                          |
| ----- | :-------------------------------- |
| 1     | Занесение анкет МКР в базу данных |

### Центр Управления Парковками

| Номер | Название                                    |
| ----- | :------------------------------------------ |
| 1     | Внесение парковочных разрешений             |
| 2     | Расшифровка государственных номерных знаков |
| 3     | Сбор информации с ГИС ГМП                   |

### Комитет по Информатизации и Связи

| Номер | Название                                           |
| ----- | :------------------------------------------------- |
| 1     | Робот по распределению писем в СЭД на исполнителей |
| 2     | Распределение обращение и формироване поручений    |

### Комитет по Образованию

| Номер | Название                                              |
| ----- | :---------------------------------------------------- |
| 1     | Робот по тарификации сотрудников                      |
| 2     | Формирование договоров на оплату платных услуг        |
| 3     | Индексация и проверка сайтов школ на ключевые слова   |
| 4     | Робот по тарификации сотрудников лицей                |
| 5     | Робот по написанию допсоглашения для сотрудника лицея |

### Комитет по Контролю за Имуществом

| Номер | Название                           |
| ----- | :--------------------------------- |
| 1     | Запрос ЕГРН по кадастровому номеру |

### Городской Информационно-Расчётный Центр

| Номер | Название                              |
| ----- | :------------------------------------ |
| 1     | Проверка отчётов по социальному такси |
| 2     | Формирование писем для расчёта НМЦК   |

### Территориальный Фонд Обязательного Медицинского Страхования

| Номер | Название                                                     |
| ----- | :----------------------------------------------------------- |
| 1     | Формирование платежных поручений и сопроводительных писем для ТФОМС |

### Комитет по Социальной Политике

| Номер | Название                                           |
| ----- | :------------------------------------------------- |
| 1     | Формирование направления для помещения детей-сирот |

### Государственная Жилищная Инспекция

| Номер | Название                                   |
| ----- | :----------------------------------------- |
| 1     | Перенос данных из ГИС ЖКХ в ЕСЭДД          |
| 2     | Внесение изменений в реестр МКД            |
| 3     | Проверка документов для отдела Бухгалтерии |

### Комитет по Строительству

| Номер | Название             |
| ----- | :------------------- |
| 1     | Сбор данных из ЕИСЖС |

### Комитет по Тарифам

| Номер | Название                                   |
| ----- | :----------------------------------------- |
| 1     | Робот для проверки лицензий аптечных точек |
| 2     | Робот для формирования писем в ЕСЭД        |
| 3     | Робот для проверки статуса точек ТО        |

### Центр Ценового Нормирования 

| Номер | Название                                        |
| ----- | :---------------------------------------------- |
| 1     | Внесение информации в ФГИС ЦС (материалы)       |
| 2     | Внесение информации в ФГИС ЦС (машины)          |
| 3     | Внесение информации в ФГИС ЦС (оптовые закупки) |

### Санкт-Петербургский Информационно-Аналитический Центр

| Номер | Название                         |
| ----- | :------------------------------- |
| 1     | Рассылка уведомлений об отпусках |
| 2     | Работа с обращениями по линии ИБ |

### Комитет по Вопросам Законности и Правопорядка

| Номер | Название                                               |
| ----- | :----------------------------------------------------- |
| 1     | Проверка табеля учета рабочего времени для бухгалтерии |

### Государственная техническая инспекция

| Номер | Название                                               |
| ----- | :----------------------------------------------------- |
| 1     | Проверка ТС на наличие страховки и формирование документов |

### Центр Энергосбережения 

| Номер | Название                               |
| ----- | :------------------------------------- |
| 1     | Интеграция двух приложений для ЦЭС ЭЗС |

### Администрации Города

| Номер | Название                              | Администрация|
| ----- | :------------------------------------ |:-------------|
| 1     | Отчет по физической культуре и спорту |Красносельская|
| 2     | Проверка справок о доходах госслужащие|Василеостровская|
| 3     | Проверка отчетов от ДС по изменению списка детей            |Красногвардейская|
| 4     | Формирование распоряжения по компенсации родительской платы |Красногвардейская|
| 5     | Запрос формы 9 |Невская|
| 6     | Выгрузка данных с ПК Имущество |Приморская|
|7| Выгрузка информации с портала Наш Санкт-Петербург         |Адмиралтейская|
| 8     | Формирование запросов для получения информации из ГИС ГМП|Адмиралтейская|
|9| Отчёт по энергоэффективностти|Центральная|
|10| Сбор и формирование отчётности для КЦСОН |Кронштадская|

1. Отчет по физической культуре и спорту
2. Проверка справок о доходах госслужащие
   > Ежегодно чиновники предоставляют декларации с информацией о доходах и расходах за предыдущий год. Робот считывает данные из декларации за 2023 год и 2022 год, по результатам сравнительного анализа каждого раздела формирует чек лист с информацией о совпадении данных либо наоборот их расхождения.

3. Проверка отчетов от ДС по изменению списка детей
4. Формирование распоряжения по компенсации родительской платы
   > 72 Детских сада Красногвардейского района ежемесячно направляют в Администрацию района информацию о включении или исключении из списка родителей детей, имеющих право на компенсацию части родительской платы. Робот пофамильно сверяет направленные списки с предыдущими месяцами. На основании итоговых списков формирует единое распоряжение с приложением к нему перечня родителей, имеющих право на льготу, по каждому детсаду.

5. Запрос формы 9
   > Робот обрабатывает заявки, поступающие от граждан, на получение справки по форме 9. 

6. Выгрузка данных с ПК Имущество
   > Робот формирует отчёт по количеству зданий, которые находятся в собственности организаций. Отчёт представлен в разбивке по типу организации (образовательная, здравоохранение, соцзащита и пр.)

7. Выгрузка информации с портала Наш Санкт-Петербург
   > Робот заходит на портал Наш Санкт-Петербург, вставляет в таблицу эксель информацию по показателям “Коэффициент исполнительской дисциплины по обработке граждан, поступающих на портал Наш Санкт-Петербург”, по которым администрация района является Контролером и/или Координатором на 1 число каждого месяца. Статистика по всем районам.

8. Формирование запросов для получения информации из ГИС ГМП

9. Отчёт по энергоэффективностти
   > Робот составляет сводную таблицу из разных таблиц (обычно по каждой сфере своя таблица). После анализирует на соответствие нормативным документам, при расхождении окрашивает ячейки. В случае расхождения данных по целевой статье - записывает на отдельный лист статью, вид расходов, суммы