# CHESS_MOVES_PREDICTION

Наш проект является анализом различных шахматных партий и, следовательно, предсказанием количества ходов в определенной шаматной игре, тестированием 
гипотез и моделей на основании полученных результатов.

Для более подробной работы с выбранными данными мы использовали различные библиотеки, методы визуализации и тд., что позволило в явном виде подтвердить или опровергнуть выдвинутые гипотезы, протестировать модели и сделать соответствующие выводы.

Данные, на основании которых базируется проект взяты с сайта pgnmentor, в связи с тем, что с остальных сайты с аналогичными данными, таких как chess.com достать информацию невозможно.

Далее представлены все этапы, проделанные нами в ходе выполнения проекта:

1) Сбор данных
   
В процессе поиска релевантных данных для парсинга мы столкнулись с проблемой, а именно с тем что в данный момент сайт chess.com и другие аналогичные сервисы заблокированны для парсинга из России. В связи с этим мы выполнили парсинг сайта с шахматными нотациями. В виду некоторых особенностей данного сайта и его ответов на реквесты нам пришлось прибегнуть к скачиванию данных через zip файлы и дальнейшему прогону их через библиотеку chess.

Для начала мы отправили запрос на сайт, ответом на который должен быть HTML код. Из него мы впоследствии и будем извлекать все интересующие нас данные. Далее, из всех выбранных нами данных отбираем лишь подходящие нам опенинги (дебюты) и записываем их в отдельные файлы. Затем скачиваем файлы и создаем на их основе табличку с данными.

2) Предварительная обработка

При анализе данных будут использоваться такие методы как K-mean или логистическая регрессия, так как в данных присутствует большое количество категориальных переменных и довольно сложно будет всё-всё-всё переделать в числовой формат.

Будет анализироваться:

a. Распределение побед в партиях (относительно белых и черных), так же их распределение в онлайн и оффлайн, и относительно отдельных игроков.

b. Насколько сильно влияет большая разница в рейтинге (более 100, или 150, так как партии по большей части сыграны гроссмейстерами, и разница в рейтинге у них не сильно решает).

c. Доминация некоторых отдельных дебютов в определенные года, поэтому нужно будет разбить года на отрезки по 5/10 лет, и посмотреть топ дебютов, и насколько они влияли на победу одних или других.
3) EDA 
на данном этапе мы визуализируем все наши данные и на основании их делаем выводы. 


![image](https://github.com/Nadinnnnnnn/CHESS_MOVES_PREDICTION/assets/169595713/dfdcc646-d131-4f72-b2dd-e1b99c1a86b7)

