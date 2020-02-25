# Simple tester for BLE UART
## Usage
1. Make sure power or battery is connected. Red LED flashing next to SDA pins (lower right).
2. Connect to Adafruit Bluefruit via BLE. Solid blue LED turns on when connected successfully.
3. Press any key to send keystroke.

## LED Feedback
### Upper right corner - red LED
- **Blink**: Keydown recognised
- **3x longer blink**: Keydown sent over to BLE master and transmission successfull
- **10x rapid blink**: ERROR: BLE transmission NOT successful.
- **Pulse**: Resetting

### Upper left corner - orange LED
- **Solid**: Charging

### Lower right corner - red LED
- **Blink**: Charging

### Lower left corner - blue LED
- **Solid**: Connected to BLE master

## Setup
### Software
- nRF51822 BLE UART Service UUID: `6e400001-b5a3-f393-e0a9-e50e24dcca9e`
- nRF51822 BLE UART Characteristic UUID: `6e400003-b5a3-f393-e0a9-e50e24dcca9e`

### Hardware
- Adafruit Bluefruit 32u4
- 4x4 Keypad
- 250 mAh 3.7V LiPo battery

## Pinout
Keypad : Adafruit Bluefruit 32u4  
1 : 5  
2 : 6  
3 : 9  
4 : 10  
5 : 11  
6 : 12  
7 : 23  
8 : 22  
### 4x4 Keypad pinout
![4x4 Keypad pinout](http://www.theorycircuit.com/wp-content/uploads/2015/12/4x4-keypad-matrix.jpg)
### Adafruit Bluefruit 32u4 Pinout
![Adafruit Bluefruit 32u4 pinout](https://cdn-learn.adafruit.com/assets/assets/000/046/242/original/adafruit_products_Feather_32u4_Bluefruit_v2.3-1.png?1504885170)

