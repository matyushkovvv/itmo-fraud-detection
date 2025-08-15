# Посмотрим сколько мошеннических операций из всех транзакций
20% - в среднем каждая пятая транзакция является мошеннической

# Проверим какие признаки сильнее всего влияют на is_fraud
Обучним случайный лес на признаках 
'is_outside_home_country', 'is_high_risk_vendor', 'max_single_amount',  'num_transactions', 'unique_countries', 'unique_merchants'
и извлечем feature_importances_

![Критерии](/resources/img1.png)

Как видно наиболее важными критериями являются 
is_outside_home_country - нахождение в другой стране
max_single_amount - максимальная сумма за транзакцию 
num_transactions - количество транзакций
