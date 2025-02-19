
# Домашняя работа по теме "Заключительная лекция"

### Перечень автоматизируемых сценариев

1. Переход с [главной страницы](https://netology.ru/#/) на [страницу с формой](https://netology.ru/programs/qa#/order)) через вкладку Каталог курсов, при выборе раздела ["Программирование"](https://netology.ru/development)

2. Переход с [главной страницы](https://netology.ru/#/) на [страницу с формой](https://netology.ru/programs/qa#/order)) через вкладку Каталог курсов, при поиске по части названия или по полному названию курса в поисковой строке

3. Переход с [главной страницы](https://netology.ru/#/) на [страницу с формой](https://netology.ru/programs/qa#/order) через виджет в разделе Направления обучения, при выборе раздела ["Программирование"](https://netology.ru/development)

4. Переход с [главной страницы](https://netology.ru/#/) на [страницу с формой](https://netology.ru/programs/qa#/order) через виджет в разделе Направления обучения, при нажатии на кнопку Полный каталог и поиске курса в списке.

5. Переход с [главной страницы](https://netology.ru/#/) на [страницу с формой](https://netology.ru/programs/qa#/order) через виджет в разделе Направления обучения, при нажатии на кнопку Полный каталог и поиске через поисковую строку по названию или по части названия курса.

6. Переход с [главной страницы](https://netology.ru/#/) на [страницу с формой](https://netology.ru/programs/qa#/order) через рекламу вверху страницы - ко всем курсам, и поиске курса в списке.

7. Переход с Footer сайта на страницу каталога курсов, с последующим выбором нужного курса.

8. Переход с Footer сайта на страницу популярных курсов, с последующим выбором нужного курса.

9. Переход с Footer сайта на страницу Программирование, с последующим выбором нужного курса.

10. Переход со [страницы курса](https://netology.ru/programs/qa#/) к [форме](https://netology.ru/programs/qa#/order) по нажатию на кнопку Записаться.

11. Переход со [страницы курса](https://netology.ru/programs/qa#/) к [форме](https://netology.ru/programs/qa#/order) по нажатию на кнопку Записаться вверху страницы, рядом с колокольчиком и аватаром.

# **Тестирование форм**

### _**Позитивный сценарий**_

**Заполнения формы заявки на курс "Инженер по тестированию"**

 1.Вводим в поле "Имя" любое имя состоящее не менее чем 2 буквы, например: Иван
 
_Ожидаемый результат_:

Поле заполнено сообщений об ошибке нет

2.Водим в поле "Телефон" валидный номер телефона +79991236587

_Ожидаемый результат_:

Поле заполнено сообщений об ошибке нет

3.Вводим в поле "Электронная почта" валидное значение IvanovIvan777@gmail.com

_Ожидаемый результат_:

Поле заполнено сообщений об ошибке нет

4.Нажать кнопку "Записаться на курс"

_Ожидаемый результат_:

Отображено окно с информацией об успешной отправки заявки на курс

**Валидация с заполненным полем "Имя" на латинице**

1.Вводим в поле "Имя" на латинице ,например: Tomas

_Ожидаемый результат_:

Поле заполнено сообщений об ошибке нет

### _**Негативные сценарии**_


**Валидация с не заполненным полем "Имя"**

1.Оставляем поле "Имя не заполненным"

_Ожидаемый результат_:

Поле "Имя" подчеркивает красным цветом, сообщение об ошибке "Обязательное поле"


 **Валидация поля "Имя" с использованием цифр**
 
1.Вводим в поле "Имя" цифры ,например: Иван08

_Ожидаемый результат_:

Поле "Имя" подчеркивает красным цветом, сообщение об ошибке "Должно состоять из букв"

2.Водим в поле "Телефон" валидный номер, например: +79991236587

_Ожидаемый результат_:

Поле заполняется сообщений об ошибке нет


**Валидация с не заполненным полем "Телефон"**

1.Водим в поле "Имя" мужское имя, например: Иван

_Ожидаемый результат_:

Поле заполняется сообщений об ошибке нет

2.Оставляем поле "Телефон" не заполненным

_Ожидаемый результат_:

Поле "Телефон" подчеркивает красным цветом, сообщение об ошибке "Обязательное поле"


**Валидация поля "Телефон" менее 10 цифр**

1.Вводим в поле "Телефон" менее десяти цифр, например: +7977990

_Ожидаемый результат_:

Поле "Телефон" подчеркивает красным цветом, сообщение об ошибке "Неверный формат"


**Валидация поля "Телефон" более 10 цифр**

1.Вводим в поле "Телефон" более десяти цифр, например: +7977999955767888

_Ожидаемый результат_:

Поле "Телефон" подчеркивает красным цветом, сообщение об ошибке "Неверный формат"


**Валидация с не заполненным полем "Электронная почта"**

1.Оставляем поле "Электронная почта" не заполненным

_Ожидаемый результат_:

Поле "Электронная почта" подчеркивает красным цветом, сообщение об ошибке "Поле обязательно для заполнения"


**Валидация поля "Электронная почта" на кириллице**

1.Вводим в поле "Электронная почта" адрес с пробелом доменной части, например: ИвановIvan77@bk.ru

_Ожидаемый результат_:

Поле "Электронная почта" подчеркивает красным цветом, сообщение об ошибке "Поле обязательно для заполнения"


**Валидация поля "Электронная почта" с пробелом в доменной части**

1.Ввести в поле "Электронная почта" адрес с пробелом доменной части, например: IvanIvanow77@ gmail.com

_Ожидаемый результат_:

Поле "Электронная почта" подчеркивает красным цветом, сообщение об ошибке "Поле обязательно для заполнения"


## Перечень используемых инструментов с обоснованием выбора.

1.**IntelliJ IDEA 2023.2.5 (Community Edition)**  - это версия интегрированной среды разработки (IDE) от компании JetBrains, используется для разработки программного обеспечения на различных языках программирования, таких как Java, Java, JavaScript, Python,Scala и других. Эта версия включает в себя множество улучшений и новых функций, направленных на повышение производительности и удобства работы разработчиков.

2.**Веб-браузер Google Chrome**  бесплатный веб-браузер, разработанный компанией Google.Вот некоторые ключевые особенности: быстрота, безопасность, простота использования, синхронизация. Так же он доступен для различных операционных систем, включая Windows, macOS, Linux, Android и iOS.


3.**Java JDK 11**  это одна из версий комплекта разработчика для языка программирования Java. JDK включает в себя все необходимые инструменты для разработки, компиляции и выполнения Java-программ.


4.**Gradle** это современная система автоматизации сборки, используемая для управления проектами и их зависимостями. Она широко используется в разработке программного обеспечения, особенно для проектов на языке Java


5.**Git**  Она используется для отслеживания изменений в исходном коде во время разработки программного обеспечения.


7.**GitHub**  это веб-сервис для хостинга репозиториев Git, который предоставляет дополнительные функции для совместной работы и управления проектами.


8.**Docker**  это платформа для разработки, доставки и запуска приложений в контейнерах. Контейнеры позволяют упаковать приложение и все его зависимости в единый образ, который можно запускать на любой системе, поддерживающей Docker.


9.**DBeaver и Valentina Studio**  это универсальный инструмент для работы с базами данных, который поддерживает множество различных СУБД (систем управления базами данных), таких как MySQL, PostgreSQL, Oracle, SQL Server, SQLite.

## Перечень необходимых разрешений, данных и доступов.


1.Доступ к системе управления версиями (например, Git):

- Разрешение на чтение и запись в репозитории.
- Доступ к веткам, связанным с тестируемыми функциями.


2.Доступ к тестовой среде:

- Разрешение на создание, изменение и удаление тестовых данных.
- Доступ к серверам и базам данных, используемым для тестирования.
- Доступ к конфигурационным файлам и настройкам среды.


3.Доступ к системе управления тестированием (например, TestRail, JIRA):


- Разрешение на создание, изменение и удаление тест-кейсов.
- Доступ к отчетам о тестировании и результатам тестов.
- Доступ к задачам и багам, связанным с тестируемыми функциями.


4.Доступ к системе непрерывной интеграции и доставки (например, Jenkins, GitLab CI/CD):

- Разрешение на запуск и мониторинг тестовых сборок.
- Доступ к логам и отчетам о выполнении тестов.
- Доступ к настройкам и конфигурациям пайплайнов.


5.Доступ к документации и спецификациям:

- Доступ к технической документации, описывающей тестируемые функции.
- Доступ к спецификациям требований и дизайна системы.

6.Доступ к инструментам автоматизации тестирования (например, Selenium, Appium):

- Разрешение на создание, изменение и выполнение автотестов.
- Доступ к логам и отчетам о выполнении автотестов.
- Доступ к настройкам и конфигурациям инструментов автоматизации.


7.Доступ к средам разработки и тестирования:

- Разрешение на установку и настройку необходимых инструментов и библиотек.
- Доступ к исходному коду и сборкам тестируемых приложений.


8.Доступ к системам мониторинга и логирования (например, ELK Stack, Splunk):

- Доступ к логам и метрикам, связанным с тестируемыми функциями.
- Разрешение на создание и настройку дашбордов и отчетов.



## Перечень и описание возможных рисков при автоматизации

1. Нагрузка на сервер может быть значительно увеличена.

3. В БД могут появиться "ненужные"  данные .

3. Технические сбои и ошибки: Автоматизированные системы могут быть подвержены техническим сбоям и ошибкам, что может привести к остановке производства или другим проблемам.

4. Кибербезопасность: Автоматизированные системы могут быть уязвимы для кибератак и взломов

5. Сложность интеграции: Интеграция новых автоматизированных систем с существующими процессами и инфраструктурой может быть сложной задачей

6. Зависимость от технологий: Организации могут стать слишком зависимыми от автоматизированных систем, что может привести к проблемам в случае их выхода из строя или устаревания.


## Перечень необходимых специалистов для автоматизации

**Инженер по автоматизации тестирования (Automation Test Engineer):**

- [ ] 1. Разрабатывает и поддерживает автоматизированные тесты.
- [ ] 2. Настраивает и использует инструменты автоматизации (например, Selenium, Appium).
- [ ] 3. Анализирует результаты тестов и сообщает о найденных дефектах.

**Разработчик (Software Developer):**

- [ ] 1. Пишет и поддерживает код приложения.
- [ ] 2. Взаимодействует с инженерами по автоматизации для интеграции тестов в процесс разработки.
- [ ] 3. Обеспечивает качество кода и его соответствие требованиям.

**DevOps-инженер (DevOps Engineer):**


- [ ] 1. Настраивает и поддерживает инфраструктуру для автоматизации.
- [ ] 2. Работает с системами непрерывной интеграции и доставки (например, Jenkins, GitLab CI/CD).
- [ ] 3. Обеспечивает автоматизацию развертывания и мониторинга приложений. 

**Аналитик по качеству (Quality Analyst):**

- [ ] Разрабатывает стратегии тестирования и планы тестирования.
- [ ] Анализирует требования и создает тест-кейсы.
- [ ] Работает с инженерами по автоматизации для обеспечения покрытия тестами всех функциональных областей.
 

**Системный администратор (System Administrator):**

- [ ] Управляет серверами и сетевой инфраструктурой.
- [ ] Обеспечивает доступность и безопасность тестовых и производственных сред.
- [ ] Настраивает и поддерживает базы данных и другие компоненты инфраструктуры.


**Менеджер проекта (Project Manager):**

- [ ] Координирует работу команды автоматизации.
- [ ] Следит за выполнением сроков и бюджетов проекта.
- [ ] Обеспечивает коммуникацию между различными участниками проекта.

**Бизнес-аналитик (Business Analyst):**

- [ ] Анализирует бизнес-требования и переводит их в технические задания.
- [ ] Работает с командой разработки и тестирования для обеспечения соответствия решений бизнес-требованиям.
- [ ] Участвует в планировании и оценке проектов автоматизации.


_Эти специалисты обеспечивают комплексный подход к автоматизации, что позволяет повысить эффективность и качество процессов в работе._

## Интервальная оценка с учётом рисков в часах

1. Анализ требований и планирование тестов:

- Без рисков: 4-8 часов
- С учётом рисков (неполные или изменяющиеся требования): 6-12 часов


2. Разработка тестовых сценариев и тест-кейсов:

- Без рисков: 8-16 часов
- С учётом рисков (сложность сценариев, изменения в требованиях): 12-24 часа


3. Настройка тестовой среды:

- Без рисков: 2-4 часа
- С учётом рисков (проблемы с конфигурацией, несовместимость): 4-8 часов

4.Разработка автотестов:

- Без рисков: 16-32 часа
- С учётом рисков (сложность тестов, проблемы с инструментами): 24-48 часов

5.Запуск и мониторинг автотестов:

- Без рисков: 4-8 часов
- С учётом рисков (технические сбои, нестабильность системы): 6-12 часов


6.Анализ результатов и отчетность:

- Без рисков: 4-8 часов
- С учётом рисков (ложные срабатывания, необходимость повторного тестирования): 6-12 часов

7.Поддержка и обновление автотестов:

- Без рисков: 8-16 часов
- С учётом рисков (изменения в системе, устаревание тестов): 12-24 часа

Таким образом, общая оценка времени для выполнения всех задач автотестировщиком может составлять:

Без рисков: 46-92 часа
С учётом рисков: 70-140 часов
