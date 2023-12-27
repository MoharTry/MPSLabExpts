```
mov [4000H],7879H;
mov [4002h],7773H;

mov al,[4000h];
mov bl,[4002h];

add al,bl;
daa;
mov [4011h],al;
mov al,[4001h];
mov bl,[4003h];
adc al,bl;
daa;

mov [4012h],al;
mov al,00;
adc al,al;
mov [4010h],al;



hlt;
```
