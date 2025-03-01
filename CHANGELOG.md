## v3.6.2
* Добавлена валидация валют при настройке модуля

## v3.6.1
* Добавлены тесты для новых версий PrestaShop

## v3.6.0
* Добавлена поддержка PrestaShop 1.7.8.10

## v3.5.8
* Реализована передача характеристик товара в ICML каталог

## v3.5.7
* Изменены минимально поддерживаемые версии PrestaShop и PHP

## v3.5.6
* Исправление передачи брошенных корзин

## v3.5.5
* Доработан маппинг доставок и оплат в соответствии с доступностью по магазинам

## v3.5.4
* Доработано сохранение ошибок в экспорте заказов

## v3.5.3
* Оптимизирован алгоритм получения истории заказов и клиентов

## v3.5.2
* Добавлен признак корзины при создании заказа

## v3.5.1
* Обновление формата даты в корзинах

## v3.5.0
* Реализована поддержка новой логики работы с брошенными корзинами.

## v3.4.14
* Исправлен баг при передаче брошенных корзин.

## v3.4.13
* Добавлена передача информации о модуле в CRM при его установке

## v3.4.12
* Исправлена ошибка получения настроек при деактивации модуля
* Оптимизирован процесс генерации Icml файла каталога
* Добавлен поиск клиента по email, если не найден по id
* Переработан блок информации о каталоге на странице настроек
* Добавлено отображение всех WebJob на странице настроек

## v3.4.11
* Добавлено отображение ошибок валидации при открытии страницы настроек
* Добавлено сохранение данных заказа в таблицу "Работа с заказами" при обратной синхронизации

## v3.4.10
* Исправлена ошибка при ручной выгрузке заказов

## v3.4.9
* Добавлены api методы для работы с файлами

## v3.4.8
* Исправлена синхронизация заказов при ненастроенном маппинге статусов

## v3.4.7
* Исправлена ошибка в работе воркеров публичной части сайта

## v3.4.6
* Добавлена проверка наличия новой версии модуля

## v3.4.5
* Исправлена работа воркеров публичной части сайта

## v3.4.4
* Улучшена горячая подгрузка данных на странице настроек модуля
* Исправлены ошибки при отсутствующем или невалидном api-ключе
* Рефакторинг контроллера RetailcrmSettingsController. Добавление контроллеров RetailcrmReferencesController и RetailcrmCatalogController 
* Рефакторинг frontend части

## v3.4.3
* Добавлена валидация данных для подключения к CRM
* Исправлен пропуск товаров корневой категории при генерации ICML

## v3.4.2
* Переработан механизм постраничной обработки истории изменений на использование sinceId вместо page

## v3.4.1
* Исправлено стили страницы настроек для старых версий PS
* Исправлена сортировка файлов журналов на странице настроек 

## v3.4.0
* Обновлен дизайн настроек модуля
* Добавлена возможность выгружать в CRM только невыгруженные заказы
* Рефакторинг RetailcrmHistory, улучшена работа с адресами
* Добавлена очистка старых файлов модуля при обновлении
* Добавлен фильтр RetailcrmFilterOrderStatusUpdate
* Улучшена обработка исключений на новых версиях PHP

## v3.3.5
* Рефакторинг RetailcrmProxy для работы с API
* Улучшена синхронизация типов оплат
* Атрибуты товаров добавлены в ICML
* Добавлено списание остатков товаров при обратной синхронизации заказов
* Рефакторинг выгрузки заказов в CRM
* Добавлен CS Fixer в проект
* Добавлено конвертирование единиц измерения веса товаров при генерации ICML
* Добавлена страница для анализа и управления выгруженными заказами в настройках модуля
* Улучшена работа JobManager на новых версиях PHP и PrestaShop

## v3.3.4
* Добавлена возможность генерации ICML каталога на странице настроек
* Исправлен порядок изображений товара при генерации каталога
* Добавлена опция передачи/получения номера заказа из/в CRM
* Добавлено поддержка новых типов оплат на странице настроек
* Добавлена возможность управления web jobs на странице настроек
* Добавлен фильтр для интервалов JobManager
* Улучшена работа с адресами при передаче заказов из CRM

## v3.3.3
* Улучшена обработка адреса доставки заказа в обратной синхронизации
* Исправлен порядок габаритов товаров в ICML

## v3.3.2
* Ребрендинг модуля RetailCRM --> Simla.com
* Улучшена работа с историей изменений заказов из Simla.com
* Добавлена проверка наличия папки логов
* Добавлена индикация ошибок в настройках модуля

## v3.3.1
* Исправлена ошибка в работе с файлами логов на старых версиях PrestaShop
* Изменена сортировка статусов заказов RetailCRM в настройках модуля
* Неактивные статусы заказов, типы доставок и оплат скрыты в настройках модуля
* Удалены интервалы менее 15 минут из настроек синхронизации брошенных корзин
* Добавлен параметр vatRate в ICML
* Исправлена ошибка при сохранении пола клиента в RetailCRM
* Добавлена дополнительная валидация для выгружаемых в RetailCRM заказов

## v3.3.0
* Добавлена возможность ручной выгрузки архива клиентов и заказов в RetailCRM
* Добавлены фильтры для упрощенной модификации данных
* Изменен путь хранения логов, добавлена автоматическая очистка старых логов
* Изменен путь для файлов кастомизации модуля, файлы необходимо размещать в папке /custom/classes внутри модуля
* Включение debug-режима в модуле перенесено в настройки в базе данных
* Улучшена работа JobManager, добавлена страница с отладочной информацией о работе
* Добавлена команда для сброса метки истории из RetailCRM
* Добавлена команда для очистки старых файлов логов
* Исправлена ошибка с форматом тегов при обновлении клиентов

## v3.2.6
* Исправлена ошибка при сохранении настроек модуля на старых версиях PrestaShop

## v3.2.5
* Исправлена ошибка брошенных корзин для Prestashop версии ниже 1.7.1
* Исправлена ошибка при проверке адреса клиента
* Исправлена ошибка подключения к базе данных при запуске тестов

## v3.2.4
* Доработана выгрузка Releases архивов в Git Actions

## v3.2.3
* Улучшена работа select в настройках модуля
* Исправлена ошибка при работе с настройкам модуля для версии 1.7.7
* Доработаны команды выгрузки архивных клиентов и заказов
* Доработана передача статуса оплаты в RetailCRM

## v3.2.2
* GitHub actions

## v3.2.1
* Ребрендинг RetailCRM

## v3.2.0
* Добавлена возможность кастомизации классов модуля
* Доработан механизм очистки пустых полей при отправке данных по API
* Доработан поиск клиента в RetailCRM при создании заказа
* Доработан расчет стоимости доставки с учетом скидки на заказ
* Исправлена ошибка дублирования адресов клиентов
* Исправлена генерация дерева категорий каталога товаров в ICML
* Исправлена ошибка затирания данных клиента при обратной синхронизации после его удалении в RetailCRM

## v3.1.1
* Улучшена работа джобов

## v3.1.0
* Поддержка смены клиента в заказе

## v3.0.6
* Улучшена работа CLI

## v3.0.5
* Возможность установки регулярных задач в `cron`, CLI-интерфейс для запуска задач вручную
* Теперь при отсутствии редактируемого заказа в RetailCRM он будет создаваться (ранее попытка редактирования приводила к ошибке)
* Доработана механика выгрузки брошенных корзин для большего соответствия ожиданиям API PrestaShop
* Исправление ошибки округления скидки в заказе

## v3.0.4
* Проверка корректности генерации категорий в ICML

## v3.0.3
* Исправлена ошибка при обновлении со старой версии для некоторых клиентов

## v3.0.2
* Подкатегории неактивной категории и товары в них больше не попадают в ICML

## v3.0.1
* Исправлена ошибка, приводившая к приостановке работы системы регулярных задач

## v3.0.0
* Новый интерфейс в модуле
* Добавлена возможность подключения онлайн-консультанта

## v2.5.1
* Исправлена ошибка с некорректным значением скидки в заказе по истории

## v2.5.0
* Добавлена возможность выгрузки брошенных корзин

## v2.4.0
* Добавлена поддержка передачи одинаковых товаров в заказе как разных товарных позиций

## v2.3.2
* Добавлен учет настройки включения НДС в стоимость товара

## v2.3.1
* Исправлены баги, связанные с передачей заказов при их оформлении

## v2.3.0
* Добавлена возможность выгрузки заказов вручную

## v2.2.11
* Добавлена валидация доменов pro и es в адресах RetailCRM

## v2.2.10
* исправление передачи цены доставки в RetailCRM

## v2.2.9
* Добавлена выгрузка габаритов в специальный тег dimensions
* Добавлена выгрузка остатков из RetailCRM
* Добавлена передача номера заказа
* Добавлена настройка Daemon Collector

## v2.2.8
* Добавлена выгрузка картинок категорий товаров в ICML

## v2.2.7
* Добавлена отправка адреса клиента при обновлении покупателя на стороне сайта
* Добавлены методы получения адреса и телефона

## v2.2.6
* Добавлена активация модуля в маркетплейсе RetailCRM

## v.2.2.5
* Добавлена передача страны при создании заказа для заказа и покупателя
* Добавлен метод для загрузки сущностей с перехватом исключений
* Для версии 1.7 добавлена передача адреса при заполнении его на стороне сайта.
* Получение адреса и телефона вынесено в отдельные методы.

## v.2.2.4
* Добавлена установка дефолтной валюты для оплаты при получении истории
* Добавлено получение суммы оплаты из заказа в CMS, если она не передается по истории

## v2.2.3
* добавлена обработка исключений при обновлении пользователя на стороне CMS

## v2.2.2
* Добавлена передача комментария клиента при создании заказа
* Добавлена передача дополнительного номера телефона в заказе и клиенте при создании заказа
* Добавлен перевод на испанкий язык

## v2.2.0
* Добавлена выгрузка истории изменений по клиентам
* Добавлена проверка имени и значения свойств товара перед отправкой заказа
* Выгрузка изменений из СРМ теперь происходит по идетификатору истории
