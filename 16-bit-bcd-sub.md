```mov [4000H],7879H;
mov [4002h],7773H;

mov al,[4000h];
mov bl,[4002h];

sub al,bl;
das;
mov [4012h],al;
mov al,[4001h];
mov bl,[4003h];
sbb al,bl;
das;

mov [4011h],al;
mov al,00;
```
