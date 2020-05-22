# Acer-Nitro-5-AN515-52-Hackintosh-Catalina-10.15.4

Hackintosh para Acer Nitro 5 AN515-52.

Foi utilizado o Notebook Acer Nitro 5 AN515-52 (N17C1), desconheço se funciona em outras variações dessa linha.

## Configurações
CPU: Intel i5-8300H

Memória: 8G * 1

GPU: UHD630

Placa de rede: DW1560 (também pode ser usada para DW1820A)

Versão do BIOS: V1.28

## Procedimento
Formatar normalmente

Inserir o arquivo boot da EFI do pendrive de formatação

Inserir a pasta EFI do Git abaixo

Alterar o input de audio para 30

Dar update nas kexts pelo clover

Entrar no modo recovery e no terminal inserir o comandos:

csrutil disable

Inserir os seguintes comandos no terminal:

sudo pmset -a hibernatemode 0

sudo rm /var/vm/sleepimage

sudo mkdir /var/vm/sleepimage

sudo pmset -a standby 0

sudo pmset -a autopoweroff 0

Executar o "ritual do audio"

## Referências
Baseado nas informações/arquivos encontrados aqui:

https://github.com/JackyZHZ/Acer-Nitro-5-hackintosh

"Ritual do audio"

https://drive.google.com/file/d/1l_4FbVODxf9646i8WVPmJl1gsenFXwhj/view?fbclid=IwAR3cqZc5ztKfl4EmRfFEJ-Of6FIuIHbBuQUh5KcjVhZt8SITqIqS2EIraNc
