```
mov si,500h;
mov di,6000h;
mov ax,0000h;
mov cx,0004h;

cld;
rep;
movsb;
hlt;
```
