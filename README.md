# Exchange Rate Widget for Zoho CRM

## Опис
Віджет для модуля Deals, який:
- отримує курс USD з API НБУ,
- порівнює його з полем `Exchange_rate_test` в угоді,
- показує різницю у відсотках,
- якщо різниця ≥ 5% або ≤ -5%, дозволяє оновити поле до актуального курсу НБУ.

## Використання
1. Додати кастомне поле в угоди з API name `Exchange_rate_test`.
2. Додати цей віджет у Zoho CRM (location: `crm.tab.relatedlist`, module: `Deals`).
3. Віджет покаже курс НБУ, курс угоди та різницю.
4. Якщо різниця значна, з’явиться кнопка для оновлення поля.

## API
- [Офіційне API НБУ](https://bank.gov.ua/NBUStatService/v1/statdirectory/exchange?valcode=USD&json)
