# Конвертеры

Большинство приемников соединяется с полетными контроллерами посредством CRSF-протокола. Если есть необходимость управления ШИМ(PWM)-каналами без использования полетного контроллера, или необходим SBus сигнал для старых полетников, можно использовать конвертеры.

## PWM

### [Matek CRSF-PWM-6 converter](http://www.mateksys.com/?portfolio=crsf-pwm#tab-id-2)
- 6 ШИМ-выходов
- Каждому выходу можно указать значение в случае FS.
- Возможность назначения на 5-й выход 11-й или 12-й канал (так как 5-й канал в ELRS дискретный и предназначен для арма).
- Не имеет встроенного BEC - требует питания 5 вольт.
- Телеметрия:
  - Имеет пин Vbat датчика напряжения батареи до 36 вольт
  - Имеет пин Current - для внешнего датчика тока
  - Позволяет подключить GPS с протоколом NMEA для передачи координат
  - Позволяет подключить барометр SPL06-001 или MS5611

![Изображение](./img/matek_CRSF_PWM_6.jpg)

### [Matek CRSF-PWM-10 converter](http://www.mateksys.com/?portfolio=crsf-pwm#tab-id-2)
- 10 ШИМ-выходов
- Каждому выходу можно указать значение в случае FS.
- Возможность назначения на 5-й выход 11-й или 12-й канал (так как 5-й канал в ELRS дискретный и предназначен для арма).
- 5-10 выход могут питаться от отдельного BEC-а для подключения высоковольтных сервомашинок.
- Не имеет встроенного BEC - требует питания 5 вольт
- Телеметрия:
  - Имеет встроенный датчик напряжения и тока (до 36 вольт и 90 ампер)
  - Позволяет подключить GPS с протоколом NMEA для передачи координат
  - Позволяет подключить барометр SPL06-001 или MS5611

![CRSF-PWM-10](./img/matek_CRSF_PWM_10.jpg)

### [Matek CRSF-PWM-B converter](http://www.mateksys.com/?portfolio=crsf-pwm#tab-id-2)

- 8 ШИМ-выходов
- Каждому выходу можно указать значение в случае FS.
- Возможность назначения на 5-й выход 11-й или 12-й канал (так как 5-й канал в ELRS дискретный и предназначен для арма).
- 5-8 выход могут питаться от отдельного BEC-а для подключения высоковольтных сервомашинок.
- Имеет встроенный BEC на 5 вольт 5 ампер.
- Телеметрия:
  - Имеет встроенный датчик напряжения(до 36 вольт)
  - Имеет пин Current - для внешнего датчика тока
  - Позволяет подключить GPS с протоколом NMEA для передачи координат
  - Позволяет подключить барометр SPL06-001 или MS5611

![CRSF-PWM-B](./img/matek_CRSF_PWM_B.jpg)

## SBus

### [Matek CRSF to SBUS converter](http://www.mateksys.com/?portfolio=crsf-sbus)
 - Преобразует CRSF в SBus.
 - Питается от 5-и вольт и может передавать питание на приемник.
 - Имеет отдельную контактную площадку *Vbat* для снятия напряжения АКБ и передачи его по телеметрии.
 - Может работать в режиме преобразователя SBus в CRSF.

![Подключение](./img/matek_CRSF_SBUS.jpg)
