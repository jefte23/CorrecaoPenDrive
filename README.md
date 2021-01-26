# CorrecaoPenDrive
correção de pendrive com problema no windows

Use o diskpart no Windows, abra o cmd ou powershel como Admin e digite:

> diskpart
> list disk
> select disk x (onde x é o número do pendrive)
> clean
> convert mbr
> create partition primary
> format fs=fat32 quick (ou fs=ntfs conforme sua escolha)
> assign
> active
> exit
