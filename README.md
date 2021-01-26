# CorrecaoPenDrive
correção de pendrive com problema no windows

Use o diskpart no Windows, abra o cmd ou powershel como Admin e digite:

<ul>
> <li>diskpart </li>
> <li>list disk </li>
> <li>select disk x (onde x é o número do pendrive) </li>
> <li>clean </li>
> <li>convert mbr </li>
> <li>create partition primary </li>
> <li>format fs=fat32 quick (ou fs=ntfs conforme sua escolha)</li>
> <li>assign </li>
> <li>active </li>
> <li>exit </li>
</ul>
