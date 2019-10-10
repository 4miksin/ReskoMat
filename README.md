# ReskoMat
Вединговый аппарат обойменного типа для продажи коробок Рескинола\Ликитар

Описание аппарата:

{позже}

Техническое наполнение (полная версия):
Питание 
1) АКБ 
2) преобразователь напряжения для питания Рескомата 
3) солнечная панель размером до 170 мм на 170 мм
4) преобразователь напряжения для заряда АКБ
Механическая часть (полная версия):
1) двигатель шаговый или сервопривод - 1 или 2 шт
2) соленоидная защелка (питание как правило 6В или 12В, редко есть 5В)
Части для оплат
1) визуальный QR код с подсветкой\екран SPI 1"-2" (питание 3.3В-5В) 
2) модуль NFC PN532 (питание 3.3В-5.4В)
3) сканер штрих кодов QR (питание 5В)
4) в исколючительных случаях будет внешний блок купюроприемника и принтера
Модули безопасности
1) датчик препятствия TCRT5000 (для вывода из спящего режима - питание 5В)
2) датчик удара (питание 3.3В-5В)
3) датчик наклона (питание 3.3В-5В)
4) датчик выдачи (для препятствования заполнению всего блока выдачи)
5) видео-камера с записью (может быть отдельным модулем вообще)
6) датчик герконовый открытия нижней и верхней крышек - 2 шт
Модули комуникации
1) GSM модуль SIM800L (4.2В или 5В)
2) динамик и микрофон
3) сенсорные кнопки TTP223 - 3 шт (вызов диспетчера, вызов экстренный, ? забыл - питание от 3 до 5.5В)
4) GSM антена плоская 
Микропроцессор 
1) Arduino Nano? Pro? 3.3В?5В?

Начальный этап проектировки рескомата
1) Питание:

а) силовая цепь питания - рекомендованная 12В (тестовая 5В или 6В): две соленоидные защелки, шаговый или серво двигатель, цепи освещения и возможно что-то еще

б) цепь питания для GSM - всегда будет находится в диапазоне до 4.2В (всегда ограничена от 3.3В до 4.2 из за питания SIMCard) на 5В модулях стоит преобразователь и для качества связи питание должно быть отдельно

в) питание микроконтроллеров и датчика - 5В 
возможно я что то забыл - подскажите

алгоритм работы Рескомата
