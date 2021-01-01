 .model small
.stack 100h
.data
Array db ‘p’,’r’,’i’,’n’,’t’
.code
Main proc
	Mov ax,@data
	Mov ds,ax
	Mov si,offset array
Mov dx,[si+2]
mov ah,2
int 21h
mov ah, 4ch
int 21h
	
main endp
end main
