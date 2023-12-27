```
mov [4000H],14H;
mov [4001h],28H;

mov al,[4000h];
mov bl,[4001h];

add al,bl;
daa;
mov [4002h],al;
hlt;
```
