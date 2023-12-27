```mov [4000H],108H;
mov [4001h],30H;

mov al,[4000h];
mov bl,[4001h];

sub al,bl;
das;
mov [4002h],al;
mov al,00h;

adc al,al;

mov [4003h],al;
hlt;
```
