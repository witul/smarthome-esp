# smarthome-esp


## ESP8266
### Standard pinout

| Port | Group | Type |
|---|---|---|
| GPIO1 | UART | TX |
| GPIO3 | UART | RX |
| GPIO4 | I2C | SDA |
| GPIO5 | I2C | SCL |
| GPIO12 | SPI | MISO |
| GPIO13 | SPI | MOSI |
| GPIO14 | SPI | CLK |
| GPIO15 | SPI | CS |
| GPIO16 | RTC | - |
| GPIO17 | ADC | - |
| GPIO0 | Boot | ? |
| GPIO2 | Boot | ? |
| GPIO6   | SDIO | - |
| GPIO7   | SDIO | - |
| GPIO8   | SDIO | - |
| GPIO9   | SDIO | - |
| GPIO10 | SDIO | - |
| GPIO11 | SDIO | - |

***


## Zalecane Częstotliwośco dla LEDC

| Frequency | Bit depth | steps |
|-----------|-----------|-------|
| 1220Hz    | 16        |65536  |
| 2441Hz    | 15        |32768  |
| 4882Hz    | 14        |16384  |
| 9765Hz    | 13        | 8192  |
| 19531Hz   | 12        | 4096  |


### Łazienka

Kontroler oświetlenia

**Static IP: 10.1.30.24**

ESP32-C6-Devkit-1

- 4 wejścia
    - SW-1
    - SW-2
    - SW-3
    - SW-4

- 3 wyjścia PWM (open drain) (2 obecnie + 1 w przyszłości)
    - 13.4V (Lampa)
    - 12.0V (LED)
    - 12.0V (Oświetlenie blatu, potencjalnie)

- Sygnalizacja błędów kolorami diody na płytce

## Obsługiwane wejście

| Input | PIN       | steps |
|-----------|-----------|-------|
| SW-1   | 16       |65536  |
| SW-2   | 15       |32768  |
| SW-3   | 14       |16384  |
| SW-3   | 13       | 8192  |

## Obsługiwane wyjścia
| Output | PIN  |
|--------|------|
|PWM-1   | GPIO4|
|PWM-2   | GPIO5|
|PWM-3   | GPIO6|