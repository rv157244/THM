# c4ptur3-th3-fl4g
## Intro
Esse CTF tem o intuito de mostrar como é um CTF de verdade e as diversas tecnologias e adversidades que podem ser encontradas nesse caminho. Ele tambem, promove de maneira educativa a pequisa e a busca por informações.
## Translation & Shifting
Traduza, desloque e decodifique o seguinte:

Todas as respostas diferenciam maiúsculas de minúsculas.
### 1 - L33T   
Leet (ou L33t ) é uma linguagem de programação esotérica baseada livremente em Brainfuck e cujo nome deriva da semelhança de seu código-fonte com a linguagem simbólica " L33t 5p34k ". L33t foi projetada por Stephen McGreal [ 1 ] e Alex Mole para ser o mais confusa possível. É Turing-completa e possui a possibilidade de código automodificável . Softwares escritos nessa linguagem podem estabelecer conexões de rede e, portanto, podem ser usados ​​para escrever malware. 

    c4n y0u c4p7u23 7h3 f149?

Resposta: can you capture the flag?

**Referência: [Wikipedia](https://en.wikipedia.org/wiki/Leet_(programming_language))**
### 2 - Binary
Um número binário é um número expresso no sistema numérico de base 2, ou sistema numérico binário , um método de representação numérica que utiliza apenas dois símbolos para os números naturais: 0 e 1. 

    01101100 01100101 01110100 01110011 00100000 01110100 01110010 01111001 00100000 01110011 01101111 01101101 01100101 00100000 01100010 01101001 01101110 01100001 01110010 01111001 00100000 01101111 01110101 01110100 00100001

Resposta:lets try some binary out!

**Referências: [Wikipedia](https://en.wikipedia.org/wiki/Binary_number) - [Leia-me](https://github.com/rv157244/Assembly-Language/blob/main/foundation/binary-numbers.md) - Ferramenta usada: [bin decoder](https://www.rapidtables.com/convert/number/binary-to-ascii.html)**
### 3 - Base 32
        MJQXGZJTGIQGS4ZAON2XAZLSEBRW63LNN5XCA2LOEBBVIRRHOM======

Resposta: base32 is super common in CTF's

Ferramerta usada: [chef](https://cyberchef.org/)

**Referencia: [wikipedia](https://en.wikipedia.org/wiki/Base32)**
### 4 - Base 64
Base64 é uma codificação binária para texto que usa 64 caracteres imprimíveis para representar cada segmento de 6 bits de uma sequência de valores de byte [ 1 ] . Como todas as codificações binárias para texto, a codificação Base64 permite a transmissão de dados binários em um canal de comunicação que suporta apenas texto.
   
    RWFjaCBCYXNlNjQgZGlnaXQgcmVwcmVzZW50cyBleGFjdGx5IDYgYml0cyBvZiBkYXRhLg==
#### Resolução:
    echo"RWFjaCBCYXNlNjQgZGlnaXQgcmVwcmVzZW50cyBleGFjdGx5IDYgYml0cyBvZiBkYXRhLg==" | base64 -d
Resposta:Each Base64 digit represents exactly 6 bits of data.

**Referẽncia: [Wikipedia](https://en.wikipedia.org/wiki/Base64)**
