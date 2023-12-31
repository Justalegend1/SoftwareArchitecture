**Заинтересованные лица:**
  * Парки, в которых будут установлены автоматы
  * Фонд содействия инновациям
  * Производители пледов
  * Посетители парков

**Функциональные требования:**
  * Система должна отображать номер ячейки автомата при взаимодействии специалиста с ней
  * Система должна позволять выбирать автомат один раз для выполнения нескольких операций
  * Система должна организовать изъятие использованных пледов из автомата
  * Система должна позволять отмечать отсутствие пледа в ячейке (данное действие требует подтверждения)
  * Система должна организовать выкладывание чистых пледов в автомат
  * Система должна позволять открывать определенную ячейку автомата
  * Система должна позволять закрывать определенную ячейку автомата
  * Система должна позволять блокировать доступ к определенной ячейке автомата
  * Система должна проводить авторизацию специалистов технического обслуживания, аналитиков, системных администраторов

**Диаграмма вариантов использования:**

_Для специалистов технического обслуживания_

![image](https://github.com/Justalegend1/SoftwareArchitecture/assets/74319066/29fa510f-d17f-48f4-ae40-b205b76b950f)

_Для аналитиков и системных администраторов_

![image](https://github.com/Justalegend1/SoftwareArchitecture/assets/74319066/a0806811-5e07-4e43-bdaa-5b556dc862b0)

**Допущения о ограничения:**
Старт происходит в городе Москва из-за высокой концентрации капитала. 
Источник финансирования - Средства гранта "Студенческого стартапа", ограничение бюджета - 1 000 000 рублей. Технологии, используемые в разработке, должны быть свободно распространяемые и не должны быть подвержены влиянию санкций. Временные ограничения обусловлены техническим заданием, они не должны быть позже сдачи командного проекта и должны соответствовать календарному плану проекта. 
Разработка технического задания должна осуществляться в соответствии с законодательством РФ: № 152-ФЗ “О персональных данных”, № 395-1 ”О банках и банковской деятельности”, № 115-ФЗ “О противодействии легализации (отмыванию) доходов, полученных преступным путем, и финансированию терроризма”. 
Санкционные ограничения не позволяют выложить мобильное приложение в сервисы play market и app store, поэтому было принято решение разработать веб-решение с интерфейсом мобильного приложения. 
На этапе разработки системы отсутствует доступ к вендинговому аппарату. Применение аппарата должно производиться на этапе тестовой эксплуатации. 
Необходимо наладить взаимодействие разработанного программного обеспечения и аппаратов.

**Нефункциональные требования**
  * Открытие ячейки должно происходить не позднее, чем через 1 секунду после оплаты
  * Система должна позволять пользователю открывать только одну ячейку за один запрос
  * Система должна позволять устанавливать таймеры для операций взятия и сдачи пледа, которые не будут считаться в время аренды
  * Система должна быть реализована в соответствии с федеральными законами РФ: № 152-ФЗ “О персональных данных”, № 395-1 ”О банках и банковской деятельности”, № 115-ФЗ “О противодействии легализации (отмыванию) доходов, полученных преступным путем, и финансированию терроризма”
  * Авторизация персонала должна производиться посредством LDAP протокола
