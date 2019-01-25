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
```signed char WriteSPI(unsigned char);```</br>
</br>
**max7219**</br>
```void init_MAX7219(void);```</br>
```void MAX7219_1Unit(unsigned char , unsigned char);```</br>
</br>
**dot_matrix**</br>
```void Draw(unsigned short *, int);```</br>
```void TurnRight(void);```</br>
```void TurnLeft(void);```</br>
```void Close(void);```</br>
```void Stop(int)```</br>
```void TurnOff()```</br>
</br>
**sound**</br>
```void delay_ms(unsigned int milliseconds);```</br>
```void PWM1_Init(long desired_frequency);```</br>
```int PWM_Max_Duty();```</br>
```void PWM1_Duty(unsigned int duty);```</br>
```void PWM1_Mode_On();```</br>
```void PWM1_Start();```</br>
```void PWM1_Stop();```</br>
```void playTone();```</br>
</br>
**hc-05**</br>
```void HC_05_Init();```</br>
```void receiveMsg();```</br>
</br>
**uart**</br>
```void USART_Init(long);```</br>
```char USART_ReceiveChar(void);```</br>
```char USART_ReceiveChar_RCREG(void);```</br>
</br>
**dot_matrix**</br>
```void External_Interrupt_Init();```