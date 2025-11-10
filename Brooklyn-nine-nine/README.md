# Brooklyn Nine Nine
Existem duas maneiras principais de obter acesso root.
## objetivo
Conseguir Explorar a aplicação web.

Conseguir Root de duas ou mais maneiras.

Aprender o máximo.
# Recon
Recebemos o $IP. Dei uma olhada na pagina web, mas não havia nada. Fui ao código fonte e encontrei um Comentario HTML.
```HTML
<!-- Have you ever heard of steganography? -->
```
Ok... Não e nada surprendente.
```BASH
wget http://$IP/brooklyn99.jpg
--2025-11-10 18:22:02--  http://10.201.109.170/brooklyn99.jpg
Conectando-se a 10.201.109.170:80... conectado.
A requisição HTTP foi enviada, aguardando resposta... 200 OK
Tamanho: 69685 (68K) [image/jpeg]
Salvando em: “brooklyn99.jpg”

brooklyn99.jpg      100%[===================>]  68,05K   119KB/s    em 0,6s    

2025-11-10 18:22:04 (119 KB/s) - “brooklyn99.jpg” salvo [69685/69685]
```
Bom, verifiquei com as ferramentas **Strings** e **Binwalk**: NADA.

Então pesquisei como esconder e extrair coisas de imagens. Achei esse artigo no [Medium](https://medium.com/@ria.banerjee005/steganography-tools-techniques-bba3f95c7148). Thanks Medium!

#### Steghide
Eu não a possuia. Então tive que instalar.
```BASH
sudo apt install steghide
steghide extract -sf brooklyn99.jpg 
Enter passphrase: 
wrote extracted data to "note.txt".
```
A senha era padrão: admin.
```BASH
cat note.txt 
Holts Password:
[REDACTED]

Enjoy!!
```
