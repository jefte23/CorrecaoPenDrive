# CorrecaoPenDrive
correção de pendrive com problema no windows

Use o diskpart no Windows, abra o cmd ou powershel como Admin e digite:

> diskpart <br>
> list disk <br>
> select disk x (onde x é o número do pendrive) <br>
> clean <br>
> convert mbr <br>
> create partition primary <br>
> format fs=fat32 quick (ou fs=ntfs conforme sua escolha) <br>
> assign <br>
> active <br>
> exit <br>
