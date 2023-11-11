# Портфолио: аналитик данных

## Обо мне

Привет! Меня зовут Елена, я начинающий аналитик данных. В этом репозитории вы найдете некоторые из моих проектов, выполненных во время обучения и практики.

<br>

## Навыки и технологии
- Инструменты анализа данных: ``SQL``, ``Excel``
- Языки программирования и библиотеки: ``Python``
- Системы управления базами данных: ``MySQL``, ``PostgreSQL``
- Средства визуализации данных: ``PowerBi``



## Проекты
<p> Проект 1: Калькулятор юнит-экономики онлайн-школы.</p>
<p> Что нужно было сделать:<p>
<ol>
 <li>Задача 1: добавить в имеющийся калькулятор поправочный коэффициент на привлечение и с его помощью пересчитать количество новых студентов за определенный период.</li>
 <li>Задача 2: пересчитать план найма преподавателей с учетом новых данных, изменив значения пропускной способности и Retention преподавателей.</li>
</ol>

<p>Как решала:<p>
<ol>
 <li>Задача 1: добавила в список параметров имеющегося калькулятора показатель "поправочный коэффициент на привлечение", добавила возможность изменять этот показатель для определенного рассчетного периода через столбец "изменение"; настроила динамический расчет количества новых студентов за определенный период с поправкой на этот коэффициент; просчитала сценарий, при котором планы маркетинга будут увеличены на 12%.</li>
 <li>Задача 2: добавила в имеющийся калькулятор найма преподавателей возможность изменять входные параметры с помощью дополнительного столбца с процентыми изменениями; сделала поправку в расчете общей пропускной способности, изменив формулу так, чтобы она отражала, что новые преподаватели в первый месяц своей работы могли проводить только половину уроков от средней пропускной способности преподавателя, задаваемой параметром; обновила прогнозное количество уроков, добавив новые значения из задачи 1; просчитала сценарий, при котором пропускная способность преподавателей увеличилась на 15%, а Retention преподавателей упал на 2%; составила новый план найма при помощи "Поиска решений" с ограничением, в котором указано, что за месяц нельзя нанять больше 70 преподавателей.</li>
</ol>

> <a href="https://joxi.ru/Dr80zRpHnMKBOr.jpg">Ссылка на задачу 1</a>
> 
> <a href="https://joxi.ru/4AkBXgDc1kj6g2.jpg">Ссылка на задачу 2</a>

<p>Итоги:<p>
<ol>
 <li>Итог по задаче 1: получили новое рассчетное количество студентов.</li>
 <li>Итог по задаче 2: получили обновленный план по найму с количеством новых преподавателей по месяцам за определенный период.</li>
</ol>
<br>

<p> Проект 2: Калькулятор юнит-экономики онлайн-кинотеатра.</p>
<p> Что нужно было сделать:<p>
<ol>
 <li>Задача 1: посчитать юнит-экономику продукта и предложить сценарий по настройке параметров для выхода на 25-процентную маржинальность.</li>
 <li>Задача 2: собрать хорошую наглядную визуализацию, где будет показано, кто, где и в каком объеме смотрит фильмы на платформе.</li>
</ol>

<p>Как решала:<p>
<ol>
 <li>Задача 1: на основании исходных данных рассчитала Retention, LT, price юнита, объем скидок, LTR, CAC, CAC на юнит, fixed costs на юнит, маржинальность, указала базовую цену; построила калькулятор, в который внесла данные AS-IS, так же TO-BE, предложив выход на 25-процентную маржинальность.</li>
 <li>Задача 2: при помощи имеющихся данных сделала визуализацию количества новых пользователей за период, распределения новых пользователей по часовым поясам, ативности пользователей по дням недели, по времени, так же сделала визуализацию по популярности фильмов + прописала сценарий по настройке параметров для выхода на 25-процентную маржинальность.</li>
</ol>

> <a href="https://joxi.ru/Vm6qjZEi0vKXVr.jpg">Ссылка на задачу 1</a>
> 
> <a href="https://docs.google.com/presentation/d/16APhowJa1AQm2_SW_LHZ8l6cmtWgQrn9NmXV-tnPIS8/edit#slide=id.g299fdca0979_1_92">Ссылка на задачу 2</a>

<p>Итоги:<p>
<ol>
 <li>Итог по задаче 1: построили калькулятор юнит-экономики и предложили сценарий по настройке параметров для выхода на 25-процентную маржинальность.</li>
 <li>Итог по задаче 2: получили хорошую наглядную визуализацию, увидели кто, где и в каком объеме смотрит фильмы на платформе, получили стратегию для достижения 25-процентной маржинальности.</li>
</ol>
<br>

<p> Проект 3: Когортный анализ онлайн-кинотеатра с помощью SQL.</p>
<p> Что нужно было сделать:<p>
<ol>
 <li>Задача 1: построить распределение количества первых покупок клиента по полям is_trial, name_partner; построить гистограмму с накоплением и добавить к графику срез, на котором можно выбрать на каких по счету покупках в рамках клиента построена гистограмма (только на первых; только на вторых; на всех, кроме первых, и т. д.); дополнить код таким образом, чтобы получились винтажные доходимости, т. е. для каждого партнера необходимо рассчитать, какой процент клиентов дошел до второй покупки, до третьей покупки и т. д.</li>
 <li>Задача 2: построить распределение выплаченных клиентам денег по месяцам; дополнить запрос так, чтобы получилось три разных скользящих средних (по сумме денег по месяцам): MA(3) — скользящее среднее, принимающее текущее значение и два предыдущих, MA(7) — скользящее среднее, принимающее текущее значение и шесть предыдущих, MA_2side(5) — двустороннее скользящее среднее, принимающее текущее значение, два предыдущих и два следующих.</li>
</ol>

<p>Как решала:<p>
<ol>
 <li>Задача 1: ознакомилась с информацией в таблице; проставила каждой покупке свой ранг, который показывает какой по счету является данная покупка в рамках всей таблицы; проставила каждой покупке свой ранг, который показывает, какой по счету является данная покупка в рамках всех покупок клиента; построила распределение количества первых покупок клиента по полям is_trial и name_partner; с помощью функции row_number проставила ранги покупок в рамках каждого клиента по времени; сгруппировала полученные результаты и перенесла полученные результаты в Excel, визуализировала их и поле "ранг" сделала срезом; чтобы посчитать количество клиентов, дошедших до определенного количества покупок использовала sum(case when...).</li>
 <li>Задача 2: с помощью функции date_trunc извлекла месяц из столбца с датами; вычислила сумму платежа; использовав подзапрос при помощи avg вычислила средние значения: MA(3) — скользящее среднее, принимающее текущее значение и два предыдущих, MA(7) — скользящее среднее, принимающее текущее значение и шесть предыдущих, MA_2side(5) — двустороннее скользящее среднее, принимающее текущее значение, два предыдущих и два следующих.</li>
</ol>

> <a href="https://docs.google.com/document/d/10k4sQ_ta87gzf7HwZmI441TL8DNGDvCn-Pc3vrpSuwA/edit?usp=sharing">Ссылка на задачу 1</a>
> 
> <a href="https://docs.google.com/document/d/1T5XNrnTCs1ehd--Cl9i1EfquT7jgWRiGkrvsY7aMkJE/edit?usp=sharing">Ссылка на задачу 2</a>

<p>Итоги:<p>
<ol>
 <li>Итог по задаче 1 и 2: с помощью SQL написаны запросы, которые ответили на поставленные вопросы и помогли визуализировать полученные данные.</li>
</ol>
<br>

<p> Проект 4: Построение витрины для модели машинного обучения в банке.</p>
<p> Что нужно было сделать:<p>
<ol>
 <li>Задача 1: для специалистов по машинному обучению необходимо составить витрину со следующими полями: внутренний идентификатор клиента — поле id_client, название города — поле name_city из таблицы skybank.region_dict, числовой признак, который принимает значение 1 для мужчин и 0 для женщин — новое поле nflag_gender на основании поля gender, возраст — поле age, числовая переменная, которая показывает, в первый ли раз клиент обратился к нам за кредитом, — поле first_time, числовой признак, который принимает значение 1 при наличии мобильного телефона и 0 при его отсутствии — новое поле nflag_cellphone на основании поля cellphone, числовая переменная, которая показывает, активен ли клиент, — поле is_active, номер клиентского сегмента — поле cl_segm, размер выданного кредита — поле amt_loan, дата выдачи кредита — поле date_loan (необходимо привести к формату даты), тип выданного кредита — поле credit_type, суммарный объем кредитов, выданных в этом городе, доля данного кредита среди всех кредитов, выданных в этом городе, суммарный объем кредитов, выданных в рамках указанного типа кредита, доля данного кредита среди всех кредитов, выданных в рамках указанного типа кредита, суммарный объем кредитов, выданных в рамках указанного типа кредита и города, доля данного кредита среди всех кредитов, выданных в рамках указанного типа кредита и города, количество кредитов, выданных в этом городе, количество кредитов, выданных в рамках указанного типа кредита, количество кредитов, выданных в рамках указанного типа кредита и города.</li>
</ol>

<p>Как решала:<p>
<ol>
 <li>Задача 1: ознакомилась с исходными данными; с использованием join подтянула названия городов из таблицы skybank.region_dict; с помощью case when указала числовой признак для мужчин и женщин, точно также указала числовой признак для наличия или отсутствия мобильного телефона; привела поле date_loan к формату дату при помощи date; с использованием подзапроса рассчитала суммарный объем кредитов, выданных в городе, суммарный объем кредитов, выданных в рамках указанного типа кредита и суммарный объем кредитов, выданных в рамках указанного типа кредита и города; затем рассчитала оставшиеся параметры.</li>
</ol>

> <a href="https://joxi.ru/zANE7zXFxjw072.jpg">Ссылка на задачу 1</a>

<p>Итоги:<p>
<ol>
 <li>Итог по задаче 1: для специалистов по машинному обучению в SQL написан скрипт, который выводит все запрашиваемые поля.</li>
</ol>
<br>

<p> Проект 5: Моделирование изменения баланса студентов.</p>
<p> Что нужно было сделать:<p>
<ol>
 <li>Задача 1: смоделировать изменения баланса студентов, понять сколько всего уроков было на балансе всех учеников за каждый календарный день, как это количество менялось под влиянием транзакций (оплат, начислений, корректирующих списаний) и уроков (списаний с баланса по мере прохождения уроков), вычислить баланс каждого студента за каждый день.</li>
 <li>Задача 2: создать визуализацию полученного результата, подготовить вопросы для дата-инженеров и владельцев таблицы payments.</li>
</ol>

<p>Как решала:<p>
<ol>
 <li>Задача 1: узнала, когда была первая транзакция для каждого студента, создала CTE first_payments с двумя полями user_id и first_payment_date (дата первой успешной транзакции); собрала таблицу с датами за каждый календарный день 2016 года, выбрала все даты из таблицы classes, создала CTE all_dates с полем dt, где будут храниться уникальные даты (без времени) уроков; узнала, за какие даты имеет смысл собирать баланс для каждого студента, объединив таблицы и создав CTE all_dates_by_user, где будут храниться все даты жизни студента после того, как произошла его первая транзакция; нашла все изменения балансов, связанные с успешными транзакциями, выбрала все транзакции из таблицы payments, сгруппировала их по user_id и дате транзакции (без времени) и нашла сумму по полю classes, в результате получила CTE payments_by_dates с полями: user_id, payment_date, transaction_balance_change (сколько уроков было начислено или списано в этот день); нашла баланс студентов, который сформирован только транзакциями, для этого объединила all_dates_by_user и payments_by_dates так, чтобы совпадали даты и user_id, использовала оконные выражения (функцию sum), чтобы найти кумулятивную сумму по полю transaction_balance_change для всех строк до текущей включительно с разбивкой по user_id и сортировкой по dt, в результате получила CTE payments_by_dates_cumsum; нашла изменения балансов из-за прохождения уроков, создала CTE classes_by_dates, посчитав в таблице classes количество уроков за каждый день для каждого ученика, при этом не интересны вводные уроки и уроки со статусом, отличным от success и failed_by_student, получила результат, при этом classes умножила на -1, чтобы отразить, что - — это списания с баланса; по аналогии с уже проделанным шагом для оплат создала CTE для хранения кумулятивной суммы количества пройденных уроков, для этого объединила таблицы all_dates_by_user и classes_by_dates так, чтобы совпадали даты и user_id, использовала оконные выражения (функцию sum), чтобы найти кумулятивную сумму по полю classes для всех строк до текущей включительно с разбивкой по user_id и сортировкой по dt, получила CTE classes_by_dates_dates_cumsum; создала CTE balances с вычисленными балансами каждого студента, для этого объединила таблицы payments_by_dates_cumsum и classes_by_dates_dates_cumsum так, чтобы совпадали даты и user_id; выбрала топ-1000 строк из CTE balances с сортировкой по user_id и dt, посмотрела на изменения балансов студентов; для того, чтобы посмотреть как менялось общее количество уроков на балансах студентов просуммируем поля transaction_balance_change, transaction_balance_change_cs, classes, classes_cs, balance из CTE balances с группировкой и сортировкой по dt.</li>
 <li>Задача 2: создала визуализацию итогового результата с помощью линейной диаграммы, подготовила вопросы дата-инженерам и владельцам таблицы payments.</li>
</ol>

> <a href="https://docs.google.com/document/d/1pAWLiIRU9ER5ij0NJNjtziAouevqD1u1rE-JZEGHLpc/edit?usp=sharing">Ссылка на задачу 1</a>
> 
> <a href="https://docs.google.com/document/d/1puUZikuv8IGhuDgTn0l1f0_BMS1ylICw-hAUFyG-j3Q/edit?usp=sharing">Ссылка на задачу 2</a>

<p>Итоги:<p>
<ol>
 <li>Итог по задаче 1 и 2 : за 2016 год было куплено 21798 уроков, списано 17264, на 31.12.16 на балансе осталось 4534 урока, пики покупок уроков в основном прослеживаются по четвергам-пятницам, т.е. к концу недели покупают больше уроков, нежели в начале недели, списание уроков с балансов по большей части происходит в будние дни, скорее связано с тем, что купившие хотят успеть все среди недели, а в выходные отдыхать (то есть более низкая точка графика - это бОльшее значение в количестве уроков), на балансе осталось 4534 урока, возможно, эти уроки планируют допройти на новогодних праздниках.</li>
</ol>
<br>

## Контактная информация
- Email: zimina.elenalex@gmail.com








