# ReskoMat
Вединговый аппарат обойменного типа для продажи коробок Рескинола\Ликитар (обновлено 18/10/2020)

Описание аппарата:

{позже}

Техническое наполнение (полная версия):
Питание 
1) АКБ LiON 3.7-4.4в в копусе от свинцового 12в 7AH
2) преобразователь напряжения для питания Рескомата? питание 3.3в 
3) солнечная панель размером до 170 мм на 170 мм (4й этап)
4) преобразователь напряжения для заряда АКБ (3й этап)
Механическая часть (полная версия):
1) сервопривод SG90s - 8 шт
2) соленоидная защелка (питание как правило 6В или 12В) - 2шт
Части для оплат
1) визуальный QR код с подсветкой\екран SPI 1"-2" (питание 3.3В) 
2) модуль NFC PN532 (питание 3.3В)
3) сканер штрих кодов QR (питание 5В?)
4) в исколючительных случаях будет внешний блок купюроприемника и принтера
Модули безопасности
1) датчик препятствия TCRT5000 (для вывода из спящего режима - питание 3.3В)
2) датчик удара (питание 3.3В)?
3) датчик наклона (питание 3.3В)?
4) датчик выдачи TCRT5000 (для препятствования заполнению всего блока выдачи)
5) видео-камера с записью (отдельный модулем вообще)
6) датчик герконовый открытия нижней и верхней крышек - 2 шт
Модули комуникации
1) GSM модуль SIM800L (4.2В )
2) динамик и микрофон
3) сенсорные кнопки TTP223 - 6 шт (вызов диспетчера, вызов экстренный, ? забыл - питание от 3.3В)
4) GSM антена плоская 
 
1) Микропроцессор Arduino Nano? Pro? 3.3В?5В?

Начальный этап проектировки рескомата
1) Питание:

а) силовая цепь питания - рекомендованная 4В (LiON 3.7В-4.4В): две соленоидные защелки требуют 6В-12В, шаговый двигатель >6В , цепи освещения и возможно что-то еще ??В

б) цепь питания для GSM - всегда будет находится в диапазоне до 4.2В (всегда ограничена от 3.3В до 4.2 из за питания SIMCard) и прямое питание от АКБ даст возможность контролировать цепь питания

в) питание микроконтроллеров и датчика - 3.3В 
возможно я что то забыл - подскажите

алгоритм работы Рескомата
