```
mov [4500h],96h;
mov [4501h],68h;
mov [4502h],70h;
mov [4503h],60h;
mov [4504h],40h;
mov [4505h],55h;
mov [4506h],76h;
mov [4507h],20h;
mov [4508h],11h;
mov [4509h],38h;

mov di,4500h;
mov si,4500h;
mov cl,09h;
mov ch,00h;

loop2:
mov bx,si;
mov al,[si];
mov ah,cl;
inc si;

loop1:
cmp al,[si];
jc skip;
mov bx,si;
mov al,[si];

skip:
inc si;
dec ah;
jnz loop1;

mov dl,[bx];
xchg dl,[di];
xchg dl,[bx];
inc di;
mov si,di;
loop loop2;
hlt
```
