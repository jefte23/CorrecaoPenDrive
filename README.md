# CorrecaoPenDrive
correção de pendrive com problema no windows

Use o diskpart no Windows, abra o cmd ou powershel como Admin e digite:

<ul>
> <li>diskpart </li><br>
> <li>list disk </li><br>
> <li>select disk x (onde x é o número do pendrive) </li><br>
> <li>clean </li><br>
> <li>convert mbr </li><br>
> <li>create partition primary </li><br>
> <li>format </li>fs=fat32 quick (ou fs=ntfs conforme sua escolha) <br>
> <li>assign </li><br>
> <li>active </li><br>
> <li>exit </li><br>
</ul>
