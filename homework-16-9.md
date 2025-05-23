# Домашнее задание к занятию «Решение задач бухгалтерского учета. Часть 4»

## Цель задания

1. Закрепить полученные знания.
2. Научиться самостоятельно решать задачи бухгалтерского учета из экзамена "1С:Специалист по Платформе".

Эта практика позволит вам определить свои сильные и слабые стороны в решении задач оперативного учета и пригодятся для самостоятельной подготовки к экзамену.

## Чеклист готовности к домашнему заданию

- Скачать каркасную конфигурацию [файл new_carcass_8_3_17_1496.dt](https://github.com/ObzhigalovSV/Netology_Accounting/blob/main/new_carcass_8_3_17_1496.dt)
- Создать пустую информационную базу
- Загрузить в нее каркасную конфигурацию
- Просмотреть материал занятия

## Инструкция к заданию

1. Решите описанную задачу в конфигураторе
2. Протестируйте решение в пользовательском режиме
3. Отправьте на проверку в личном кабинете Нетологии один файл выгрузки базы данных (.dt), содержащий решение задачи. Файл прикрепите в раздел «решение» в практическом задании. Имя файла должно быть в формате "ФамилияИО_БУ4.dt".

## Описание задачи

Необходимо создать документ «Операция», с помощью которого пользователь должен иметь возможность ввести проводки с произвольной корреспонденцией счетов. При решении задачи следует учитывать возможность наличия проводок, сформированных с помощью данного документа.

Компания занимается оптовой торговлей. Учет товаров ведется в разрезе организаций и мест хранения. Подразумевается, что для каждой организации баланс будет формировать отдельно (каждая организация это отдельное юридическое лицо). Поступление товаров отражается документом «Приходная накладная», продажа - «Расходная накладная». Организация, валюта, контрагент и склад указываются в шапке документов.

Документ «Приходная накладная» реализует следующую проводку:

*Дт «Товары» - Кт «Поставщики» на количество и сумму закупаемого товара.*

Документ «Расходная накладная» реализует следующие проводки:

*Дт «Прибыли и убытки» - Кт «Товары» на количество и сумму себестоимости;*

*Дт «Покупатели» - Кт «Прибыли и убытки» на сумму в продажных ценах.*

Себестоимость определяется как средняя для каждой номенклатурной позиции, в каждой организации, но сразу по всем складам.

Взаиморасчеты с покупателями ведутся в различных валютах.

Поступление оплаты от покупателей фиксируется документом «Приход денег». В шапке документа указывается организация и валюта документа, в табличной части – контрагент и сумма. Сумма оплаты не может превосходить сумму задолженности. В том случае, если сумма оплаты больше суммы задолженности по контрагенту, то документ не проводится.

Контроль задолженностей должен быть осуществлен по валютным суммам. Незакрытые задолженности в рублях, но закрытые в валюте, погашаются пользователем вручную с помощью документа «Операция».

Документ «Приход денег» формирует следующую проводку:

*Дт «Касса» - Кт «Покупатели» на сумму оплат*

Необходимо создать отчеты по продажам товаров и по состоянию взаиморасчетов с покупателями.

![image](https://github.com/ObzhigalovSV/Netology_Accounting/blob/main/%D0%9E%D1%82%D1%87%D0%B5%D1%82%D0%9F%D1%80%D0%BE%D0%B4%D0%B0%D0%B6.png)

Прибыль рассчитывается как: «Сумма продаж» - «Себестоимость»

Отчет должен быть построен для конкретной организации, за любой расчетный период. Организация и границы периода должны задаваться пользователем напрямую в форме отчета.

![image](https://github.com/ObzhigalovSV/Netology_Accounting/blob/main/%D0%97%D0%B0%D0%B4%D0%BE%D0%BB%D0%B6%D0%B5%D0%BD%D0%BD%D0%BE%D1%81%D1%82%D1%8C%D0%9F%D0%BE%D0%BA%D1%83%D0%BF%D0%B0%D1%82%D0%B5%D0%BB%D0%B5%D0%B9.png)

В печатной форме заголовок и шапка отчета должны соответствовать заданию.

ОБЯЗАТЕЛЬНО! В пользовательском режиме заведите тестовый пример. Данные для примера генерируете самостоятельно.

------

### Критерии оценки 

1. Зачёт — реализован весь требуемый функционал, нет критичных ошибок и нарушения логики. 
2. Введены тестовые данные в пользовательском режиме.
3. На доработку — задание выполнено частично или не выполнено, в логике выполнения заданий есть противоречия, критичные ошибки.
Любые вопросы по решению задач задавайте в чате учебной группы.

*Примерное время выполнения: 45–180 минут*
