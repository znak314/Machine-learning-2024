# Machine-learning-2024
Machine learning course 2024 in Kyiv Polytechnic Institute
## Лабораторна 1: "Введення в data science"
На сайті http://www.ukrstat.gov.ua/ оберати дані які для Вас є цікавими, можна використати будь-який ресурс з відкритими даними, та завантажте дані.
Знайти математичне сподівання, медіану, моду, дисперсію, середньоквадратичне відхилення (поясніть їх зміст).
Візуалізувати завантажені дані за допомогою гістограми.
Для цих даних проробити всі дії з пункту колекції Series і DataFrame бібліотеки pandas.
Виконати первинну обробку даних.
Прочитати набір даних катастрофи «Титаніка».
Завантажити набір даних катастрофи «Титаніка» за URL- адресою.
Переглянути рядки набору даних катастрофи «Титаніка».
Налаштувати назви стовпців.
Провести простий аналіз даних.
Побудувати гістограму віку пасажирів.


## Лабораторна 2: "Часові ряди і проста лінійна регресія"
Завантажити метеорологічні дані в 1895-2022 роках з CSV-файлу в DataFrame. Після цього дані треба буде відформатувати для використання.
Бібліотеку Seaborn використати для графічного представлення даних DataFrame у вигляді регресійної прямої, що представляє графік зміни обраних показників за період 1895-2018 років.
Спрогнозуйте дані на 2019, 2020, 2021 та 2022 рік.
Оцініть за формулою, якою могли б бути показники до 1895 року.
Скористайтесь функцією regplot бібліотеки Seaborn для виведення всіх точок даних.
Виконайте маштабування осі у від (приклад від 10 до 70 градусів).
Порівняйте отриманий прогноз для 2019, 2020, 2021 та за 2022 роки з даними на NOAA «Climate at a Glance»: https://www.ncdc.noaa.gov/cag/ і зробити висновок.


## Лабораторна 3: "Класифікація, регресія і кластеризація з використанням бібліотеки scikit-learn"
Повторити дії описані в пункті «Часові ряди і проста лінійна регресія частина 2» даної лабораторної роботи та порівняти з результатом попередньої лабораторної роботи.
Аналогічно з прикладом з лекції 7 згенеруйте набір даних та класифікуйте його використавши класифікатор SVC (слайд 95).
Порівняти декілька класифікаційних оцінювачів наприклад KNeighborsClassifier, SVC та GaussianNB для вбудованого в scikit-learn одного набору даних (вибрати довільний за бажанням).


## Лабораторна 4: "Класифікація методом k найближчих сусідів і набір даних Digits"
Для дослідження даних, візуалізуйте їх. Виведіть зображення перших 24 і 36 цифр з набору.
Розбийте дані на навчальні та тестові, за замовчуванням train_test_split резервує 75% даних для навчання і 25% для тестування, змініть це.
Створити та навчити модель.
Виконайте прогнозування класів.
Порівняйте прогнозовані цифри з очікуваними для перших 20, 24, 36 тестових зразків.
Поясніть результат, застосуйте метрики точності моделі.
Виведіть звіт класифікації.
Використайте декілька моделей KNeighborsClassifier, SVC та GaussianNB для пошуку найкращої.
Налаштуйте гіперпараметр K у KNeighborsClassifier.


## Лабораторна 5: "Проектування та навчання штучної нейронної мережi для задач класифiкацiї"
Виконати завдання iз прикладу i отримати файл iз навченою моделлю для розпiзнавання рукописних цифр. В будь якому графiчному редакторi створити файл iз рукописною цифрою i розпiзнати її. Пояснити результат.
Спроектувати i розробити нейронну мережу на основi таких наборiв даних iмплементованих в Keras:
Cifar10;
FMNIST. Потрiбно розробити архiтектуру нейронної мережi, навчити її на тестових прикладах, i продемонструвати її роботу на кількох зображеннях.


## Лабораторна 6: "Прикладна задача машинного навчання"
Створити, навчити і апробувати багатошарову нейронну мережу з прямою передачею сигналу для ухвалення рішення про зарахування до Університету абітурієнтів, які здали вступні іспити з математики, англійської та української мови.
Правила прийому наступні:

Рейтинг абітурієнтів формується за формулою 0,4 БМ+0,3БА+0,3БУ, де БМ-бал з іспиту з математики, БА-бал з іспиту з англійської мови, БУ-бал з іспиту з української мови.
Мінімальний прохідний бал на вступ 160 для абітурієнтів без пільг.
З математики для абітурієнтів без пільг мінімальний бал іспиту не може бути менший 140 балів.
бітурієнти, які мають пільги, зараховуються при мінімумі 120 балів з усіх іспитів і їх рейтинг не може бути меншим ніж 144 бали
Університет може прийняти на навчання 350 абітурієнтів, з них не більше 10% це абітурієнти з пільгами.
Статистика минулих років показує, що в середньому до Університету подають документи 1500 абітурієнтів.
Для навчання мережі слід використовувати всі вивчені методи адаптації та навчання та провести аналіз їх ефективності. Слід також визначити мінімальну кількість шарів і нейронів, що забезпечує задовільне рішення поставленої задачі. У звіті навести архітектуру мережі та код реалізації. Результат має бути візуалізований та представлений у формі Еxcel таблиці, як список зарахованих абітурієнтів.
