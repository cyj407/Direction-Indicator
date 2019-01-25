# Direction Indicator
A bicycle direction indicator controlled by the button or [Android APP](https://github.com/cyj407/Voice-Controller).
</br>
Besides, use a buzzer to play music when the indicator is on.

## Circuit Diagram
![](https://i.imgur.com/7kpzjct.png)

## Demo Photo
<img width="330" height="250" src="https://i.imgur.com/5CPq6mR.jpg">
</br>
<img width="330" height="250" src="https://i.imgur.com/CQ47c7l.jpg">

## Environment Setting
* MPLAB IDE v5(XC8 compiler)
* Write in C language.

## Library & API
**SPI**</br>
```signed char WriteSPI(unsigned char);```
</br>
**max7219**</br>
```void init_MAX7219(void);```
```void MAX7219_1Unit(unsigned char , unsigned char);```
</br>
**dot_matrix**</br>
```void Draw(unsigned short *, int);```
```void TurnRight(void);```
```void TurnLeft(void);```
```void Close(void);```
```void Stop(int)```
```void TurnOff()```
</br>
**sound**</br>
```void delay_ms(unsigned int milliseconds);```
```void PWM1_Init(long desired_frequency);```
```int PWM_Max_Duty();```
```void PWM1_Duty(unsigned int duty);```
```void PWM1_Mode_On();```
```void PWM1_Start();```
```void PWM1_Stop();```
```void playTone();```
</br>
**hc-05**</br>
```void HC_05_Init();```
```void receiveMsg();```
</br>
**uart**</br>
```void USART_Init(long);```
```char USART_ReceiveChar(void);```
```char USART_ReceiveChar_RCREG(void);```
</br>
**dot_matrix**</br>
```void External_Interrupt_Init();```