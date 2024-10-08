# Задача 13

### Условие
Найдите наибольшее натуральное число, факториал которого не делится на $3^{2019}$.

### Решение
- Свойства степени, факториала и формула Лежандра
- Начнем с того, что $3^{2019}$ значит $2019$ множителей $3$ отсюда тогда нам нужно найти такой факториал который будет сапоставим по множителям $3$ с числом вышем, для этого пусть возьмем число $2019 * 2 = 4038$, теперь нужно узнать сколько троек к него входит, вообще факториал данного числа выглядит так $1 * 2 * 3 * 4 * 5 * 6 * 7 * 8 * 9 * ... * 4038$, а теперь давайте поставим в дробь два числа и получим $\frac{1 * 2 * 3 * 4 * 5 * 6 * 7 * 8 * 9 * ... * 4038}{3 * 3 * 3 * 3 * 3 * 3 * 3 * 3 * 3 * ... * 3}$, заметим что число $9$ сокращает не одну тройку а $2$, так как $9 = 3^2$ то можем сделать вывод что нужно делать подсчет не только по обычным тройкам, но и по степенным до $7$ показателя степени так как $3^8 > 4038$, то что мы сейчас вывели и есть формула Лежандра, в формульном ввиде(нашего случая) $\sum_{k = 1}^{7}\left[\frac{n}{p^k}\right]$, $\sum_{k = 1}^{7}\left[\frac{4038}{3^k}\right] = 2018$ то-есть очень близко теперь нужно понять максимальное ли это число, или есть больше, тогда возьмем $4040$, получим $> 2019$ отсюда понятно, но нужно проверить, что $4039$ подходит, после подставление в формулу стало ясно, что получилось $< 2019$.

---

### Ответ
- 4039