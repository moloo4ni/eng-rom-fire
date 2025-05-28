# Engineering Firmware for Redmi 12 4G (fire)
# Инженерная прошивка для Redmi 12 4G (fire)

## Critical Warnings / Важные предупреждения
**EN:**  
1. Never flash `preloader.bin` unless absolutely necessary - this will permanently brick your device  
2. Use only original USB cable and reliable power source  
3. Backup your original firmware before flashing  

**RU:**  
1. Никогда не прошивайте `preloader.bin` без крайней необходимости - это навсегда превратит устройство в кирпич  
2. Используйте только оригинальный USB-кабель и надежный источник питания  
3. Сделайте резервную копию оригинальной прошивки перед прошивкой  

## Requirements / Требования
**EN:**  
- Device: Redmi 12 4G (codename fire)  
- Tools:  
  - SP Flash Tool v5.2316 or newer  
  - MTK USB VCOM Drivers  
- Computer: Windows 10/11 (64-bit)  
- Battery: Minimum 70% charge  

**RU:**  
- Устройство: Redmi 12 4G (кодовое имя fire)  
- Инструменты:  
  - SP Flash Tool v5.2316 или новее  
  - Драйверы MTK USB VCOM  
- Компьютер: Windows 10/11 (64-бит)  
- Заряд батареи: Не менее 70%  

## Installation Guide / Руководство по установке
### Preparation / Подготовка
**EN:**  
1. Install MTK VCOM drivers (disable driver signature enforcement)  
2. Extract firmware to path without spaces  

**RU:**  
1. Установите драйверы MTK VCOM (отключите проверку цифровой подписи)  
2. Распакуйте прошивку в путь без пробелов  

### Flashing Process / Процесс прошивки
**EN:**  
1. Launch SP Flash Tool as Administrator  
2. Load scatter file: `MT6768_Android_scatter.txt`  
3. Verify that preloader.bin is UNCHECKED  
4. Select Download Only mode  
5. Click Download button  
6. With device POWERED OFF:  
   - Hold Volume Down, Volume Up and Power buttons
   - Connect USB cable  
7. Release button when flashing starts  
8. Wait for green checkmark (Download OK)  

**RU:**  
1. Запустите SP Flash Tool от имени Администратора  
2. Загрузите scatter-файл: `MT6768_Android_scatter.txt`  
3. Убедитесь, что preloader.bin ОТКЛЮЧЕН  
4. Выберите режим Download Only  
5. Нажмите кнопку Download  
6. При ВЫКЛЮЧЕННОМ устройстве:  
   - Удерживайте кнопку громкости вниз, вверх и питания
   - Подключите USB-кабель  
7. Отпустите кнопку при начале прошивки  
8. Дождитесь зеленой галочки (Download OK)  

## Post-Flash Instructions / После прошивки
**EN:**  
- First boot may take 10-15 minutes  
- Perform factory reset in recovery mode  
- Access engineer menu: Dial `*#*#3646633#*#*`  
- DO NOT lock bootloader after flashing  

**RU:**  
- Первая загрузка может занять 10-15 минут  
- Выполните сброс до заводских настроек в recovery  
- Откройте инженерное меню: Наберите `*#*#3646633#*#*`  
- НЕ блокируйте загрузчик после прошивки  

## Troubleshooting / Решение проблем
**EN:**  
| Error       | Solution                          |
|-------------|-----------------------------------|
| BROM ERROR  | Reinstall drivers, try different USB port |
| S_FT_ENABLE_DRAM_FAIL | Use SP Flash Tool v5.2316 |
| Hash mismatch | Verify firmware integrity         |
| 0% freezing | Replace USB cable, check battery |

**RU:**  
| Ошибка      | Решение                           |
|-------------|-----------------------------------|
| BROM ERROR  | Переустановите драйверы, попробуйте другой USB-порт |
| S_FT_ENABLE_DRAM_FAIL | Используйте SP Flash Tool v5.2316 |
| Hash mismatch | Проверьте целостность прошивки   |
| Зависание 0% | Замените USB-кабель, проверьте заряд |
