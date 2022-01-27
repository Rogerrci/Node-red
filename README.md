# Node-red
Node-red + ifm multicode reader (O2I500) + .txt file

Objetivo:
Armazenamento local (.txt) dos dados de leitura do rótulo traseiro do listerine, utilizando o leitor de códigos ifm O2I500.

- Comunicação TCP/IP
  - Trigger via comando de rede
  - leitura de 2 códigos simultâneos EAN-13/Data Matrix
  - envio para node-red TCP/IP
  - escrita em arquivo .txt armazenamento local 
  - conteúdo (;Result:1;Code:556423;Code:7891010973902;time:319;)
 
Arquivos:
Node-Red 
  fluxo => "ifm multicodereader write .txt file.json"

ifm Vision Assistat
  interface de comunicação TCP/IP => "TCP_IP_interface_node-red_write_txt_file.o2xpcic"
  aplicação => "1 - O2I500 + Listerine Back Label.o2i5xxapp" 

Softwares:
Node-red => https://nodered.org/

ifm vision Assistant => https://www.ifm.com/br/pt/product/O2I500?tab=documents

Hardware:
ifm multicode reader O2I500 => https://www.ifm.com/br/pt/product/O2I500
