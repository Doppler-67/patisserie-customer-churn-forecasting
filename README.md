# patisserie-customer-churn-forecasting
**Отдел маркетинга крупной сети кондитерских планирует промо акцию для 
удержания клиентов.
Акция заключается в предоставлении скидки в 25 % тем клиентам, которые с 
высокой вероятностью перейдут к конкурентам.**

## Цель проекта
Разработка ML модели для прогнозирования оттока клиентов.
## Про данные

Для прогнозирования используются данные о покупках юзеров за период 
2021 года. Всего доступно больше 2 млн. строк. 
Флаг оттока проставляется, если после покупки юзера прошло больше 45 
дней. 
Поведение юзера описывается историей его покупок, суммой чека и 
размером скидки к чеку. В компании действует программа лояльности, 
участвуя в которой юзеры получают скидку на любую покупку и могут 
получать дополнительные скидки по разным промо-акциям.

### Описание данных:

**data.csv**
---

**clnt_ID:** уникальный айди юзера, str;

**timestamp:** дата и время совершения покупки, datetime;

**gest_Sum:** сумма покупки, float;

**gest_Discount:** сумма скидки, float.

**target.csv**
---

**clnt_ID:**  уникальный айди юзера, str;

**target:** флаг оттока, int (1, если юзер ушел в отток и 0, если остался).
