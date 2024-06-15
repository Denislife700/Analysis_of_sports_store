# Analysis_of_sports_store
Данное исследование - это итоговый проект по курсу DA Junior.
Исследование состоит из пяти частей: 
1. Предобработка данных
2. Бинарная классификация
3. Проведение A/B-тестирования
4. Кластеризация
5. Построение модели склонности клиента к покупке

Мне предоставили данные о покупках клиентов за два месяца. Чтобы не возникло утечки, вся информация была зашифрована. Данные хранятся в базе данных.
База данных содержит три таблицы:
personal_data — ID клиентов, их пол, возраст, образование, страна и город проживания;
personal_data_coeffs — данные с персональными коэффициентами клиентов, которые рассчитываются по некоторой закрытой схеме;
purchases — данные о покупках: ID покупателя, название товара, цвет, стоимость, гендерная принадлежность потенциальных покупателей товара, наличие скидкии дата покупки.

При передаче данных выяснилось, что часть информации о клиентах из таблицы personal_data была утеряна. Поэтому, помимо базы данных, был предоставлен сжатый CSV-файл с утерянными данными (personal_data.csv.gz). К сожалению, информацию о поле клиентов восстановить не удалось. 
Мной была построена модель классификации на полных данных, чтобы, соответственно, восстановить утерянные.

Известно, что магазин проводил две маркетинговые кампании: 
- Первая кампания проводилась в период с 5-го по 16-й день, ID участвовавших в ней пользователей содержатся в файле ids_first_company_positive.txt. Эта кампания включала в себя предоставление персональной скидки 5 000 клиентов через email-рассылку. Для проведения A/B-тестирования, помимо людей, которым предлагалась персональная скидка, были отобраны люди со схожими социально-демографическими признаками и покупками, которым скидку не предложили. ID этих клиентов лежат в аналогичном файле ids_first_company_negative.txt.
- Вторая кампания проводилась на жителях города 1 134 и представляла собой баннерную рекламу на билбордах: скидка всем каждое 15-е число месяца (15-й и 45-й день в нашем случае).
В работе проведён анализ A/B тестирования и результаты маркетинговой кампании.

Далее данные были поделены на кластеры и проведен анализ а разрезе кластеров. Важным условием было узнать насколько на покупку влияет наличие скидки по кластерам.

Известно что планируется запуск новой маркетинговой кампании на жителях страны 32 города 1 188. Мной построена модель склонности клиента к покупке определённого товара.

Заключающий этап работы включал в себя подготовку отчета для руководителя с пояснением и отчет для публичной призентации проведенного исследования.



