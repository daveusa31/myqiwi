# myqiwi




Возможности
======
* Переводы на любой Qiwi Кошелек
* Статистика по платежам
* Получение информации о пользователе
* Сортировка платежей по типу(в/из), валюте.
* Определение провайдера мобильного телефона


Использование
======
```python
    import myqiwi
    wallet = myqiwi.Wallet(token, number="79001234567")
```

Быстрый туториал
======

Получить текущий баланс
----------------
```python
    print(wallet.balance())
```

Отправка платежа
----------------
```python
	payee = "7999778909" # Получатель платежа
	sum = 50 # Сумма перевода. Обязательно в рублях!
	comment = "Перевод сделан с помощью библиотеки myqiwi" # Необязательный
								#аргумент

    wallet.send(payee, sum, comment)
```


# To do
- [ ] Написать таблицу с методами, описанием и передаваемыми аргументами
- [ ] Переписать readme
- [ ] Переписать функцию generate_pay_form
- [ ] Добавить возможность вывода ошибок в транслите, с помощью библиотеки [transliterate](https://github.com/barseghyanartur/transliterate)


