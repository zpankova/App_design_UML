## Краткое описание системы, для которой сделаны диаграммы

Проектируемой системой в данной работе является приложение для заказа и доставки еды. Для того, чтобы перейти к составлению диаграмм, обозначим основных акторов и общие бизнес-процессы, которые происходят через приложение.

# Акторами являются: 

1. Пользователь: желает заказать еду через приложение.
2. Ресторан: предоставляет меню и готовит заказы
3. Курьер: доставляет заказы клиентам
4. Система приложения: выполняет операции с данными пользователей и предоставляет функционал

## Опишем основные варианты использования, которые будут детализированы с помощью use-case диаграммы, а также будут браться за основу для процессов, описываемых в других диаграммах.

1. Заказ еды: пользователь выбирает ресторан и блюда, оформляет заказ.
2. Подтверждение заказа: ресторан получает заказ и подтверждает его.
3. Подготовка заказа: ресторан готовит блюда.
4. Доставка заказа: курьер получает заказ и доставляет его клиенту.
5. Отслеживание заказа: пользователь может отслеживать статус своего заказа.

## Далее углубимся в сам процесс заказа, который будет описан с помощью диаграммы последовательностей.

1. Пользователь открывает приложение и выбирает ресторан.
2. Приложение отображает меню ресторана.
3. Пользователь выбирает желаемые блюда и добавляет их в корзину.
4. Приложение вычисляет общую сумму заказа и предоставляет пользователю возможность оформить заказ.
5. Пользователь подтверждает заказ и вводит адрес доставки.
6. Приложение отправляет заказ в систему ресторана.
7. Ресторан подтверждает получение заказа и начинает его готовить.
8. После готовности заказа, курьер забирает его из ресторана и отправляется по адресу доставки.
9. Приложение отслеживает местоположение курьера и предоставляет пользователю информацию о статусе доставки.
10. Курьер доставляет заказ пользователю.
11. Пользователь получает заказ и оплачивает его, если с заказом все хорошо.
12. Пользователь завершает процесс доставки.

## Основным объектом, с которым все акторы выполняют свои действия является заказ. Обозначим его основные статусы. Переход из между состояниями и их иерархия уточнены на диаграммы состояний.

1. Новый заказ: заказ еще не обработан системой и не назначен курьеру.
2. Подтвержденный заказ: заказ был принят системой и назначен курьеру для доставки.
3. Заказ в процессе доставки: курьер находится в пути к месту получения заказа.
4. Заказ доставлен: заказ был успешно доставлен клиенту.
5. Заказ получен клиентом: если с заказом все хорошо, то клиент оплачивает его и забирает
6. Отмененный заказ: заказ был отменен  клиентом на одном из шагов

Детализация взаимодействия акторов и работы всех процессов также представлена на диаграммах деятельности и классов.
Диаграммы лежат вв файлах с названиями, соответствующими типу диаграммы.
Для создания диаграмм использовался [LucidChart](https://www.lucidchart.com/pages/examples/uml_diagram_tool)
