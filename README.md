# yandex_practicum
Пет-проекты написанные на курсе data science bootcamp

| Названия проектов | Описание | Использованные инструменты |
| :--------------------: | :---------------------: |:---------------------------:|
| Телекоммуникации | В данном выпускном проекте решалась задача борьбы с оттоком клиентов. Проект направлен на разработку и внедрение модели, которая позволит предложить клиентам специальные условия и промокоды для удержания на основе предиктивного анализа данных о поведении абонентов. | <ul>**Обработка и визуализация данных**: <li>`pandas`: Основная библиотека для манипуляции с данными и анализа.</li> <li>`numpy` : Используется для числовых операций и работы с массивами. </li> <li> `matplotlib.pyplot` и `seaborn`: Библиотеки для визуализации данных </li> </ul> <ul>**Предобработка данных и моделирование:**</ul> <li>`sklearn` - Использовался для кодирования, нормализации, преобразования признаков, а так же для использования базовых моделей "из коробки"</li><li> `lightgbm` - для создания модели классификации с помощью градиентного бустинга</li><li>  `boxcox`, `yeojohnson` (из `scipy.stats`): Преобразования для стабилизации дисперсии и нормализации распределения переменных.</li><ul>**Оценка и оптимизация моделей:**</ul> <li> `roc_curve`, `roc_auc`: Метрики для оценки производительности моделей.</li> <li>`BayesSearchCV`: Оптимизация гиперпараметров моделей с использованием байесовского подхода.</li> <ul>**Расширенный анализ данных:** </ul> <li>`phik`: Инструмент для оценки корреляции между переменными, включая числовые и категориальные данные. </li><li>`shap`: Библиотека для интерпретации прогнозов моделей, позволяющая понять вклад каждой переменной в итоговый прогноз.</li>|
|Прогнозирование заказов такси|Компания «Чётенькое такси» разрабатывает модель машинного обучения для прогнозирования количества заказов такси на следующий час, используя исторические данные заказов в аэропортах. Проект направлен на оптимизацию распределения водителей на линии в периоды пиковой нагрузки. Модель должна достичь значения метрики RMSE < 48 на тестовой выборке. Этапы проекта включают загрузку и ресемплирование данных по часам, анализ данных, обучение различных моделей с подбором гиперпараметров и оценку результатов на тестовой выборке.|<ul>**Обработка и визуализация данных**: <li>`pandas`</li> <li>`numpy` </li> <li> `matplotlib.pyplot` и `seaborn`</li> </ul> <ul>**Анализ временных рядов:** <li>`kpss` и `adfuller` из `statsmodels.tsa.stattools`: Тесты для проверки стационарности временных рядов</li> <li>`seasonal_decompose` из `statsmodels.tsa.seasonal`: Разложение временных рядов на тренд, сезонность и остаток. </li> <li> `SimpleExpSmoothing` из `statsmodels.tsa.holtwinters`:Модель экспоненциального сглаживания для прогнозирования временных рядов.</li> </ul> <ul>**Моделирование и машинное обучение:**: <li>`lightgbm`</li> <li>`RandomForestRegressor` </li> </ul> <ul>**Оценка моделей:**: <li>`mean_squared_error`</li> </ul>|
|Определение стоимости автомобилей|Сервис по продаже подержанных автомобилей «Не бит, не крашен» разрабатывает приложение для оценки рыночной стоимости автомобилей, используя исторические данные о технических характеристиках, комплектациях и ценах. Цель проекта — создать модель машинного обучения, которая быстро и точно определяет стоимость автомобиля. Основные требования заказчика к модели включают высокое качество предсказания, минимальное время обучения и скорость выполнения предсказаний, при этом значение RMSE должно быть меньше 2500. В процессе разработки предлагается исследовать различные типы моделей, включая, но не ограничиваясь, градиентным бустингом с использованием библиотеки LightGBM.|<ul>**Обработка и визуализация данных**: <li>`pandas`</li> <li>`numpy` </li> <li> `matplotlib.pyplot` и `seaborn`</li> </ul><ul>**Подготовка признаков и предобработка данных**: <li>`sklearn`: нормализация, кодирование, создания GroupKFold валидации, а также предоставления ML алгоритмов  </li> <li>`imblearn.pipeline`: для создания пайплайнов обработки-обучения </li> </ul> <ul>**Модели**: <li>`LinearRegression`, `Ridge`: Линейные модели для регрессии.</li> <li>`lightgbm` </li> </ul><ul>**Оценка моделей**: <li>`mean_squared_error`</li> <li>`shap`-обеспечивает интерпретируемость моделей машинного обучения. </li> </ul>|
|Защита персональных данных клиентов|Страховая компания «Хоть потоп» стремится защитить персональные данные своих клиентов, разрабатывая метод преобразования данных, который усложняет восстановление личной информации, не влияя при этом на качество моделей машинного обучения. Проект включает разработку алгоритма, использующего обратимые матричные операции для преобразования признаков, обоснование его эффективности, и верификацию того, что такое преобразование не влияет на результативность линейной регрессии по метрике R2. Основные этапы работы: изучение данных, обоснование выбора алгоритма, программирование преобразований и проверка качества модели до и после преобразования данных.|<ul>**Обработка и визуализация данных**: <li>`pandas`</li> <li>`numpy` </li> <li> `matplotlib.pyplot` и `seaborn`</li> </ul><ul>**Моделирование и машинное обучение**: <li>`LinearRegression`</li> <li>`train_test_split` </li> </ul><ul>**Оценка моделей**: <li>`r2_score`</li>  </ul> |
