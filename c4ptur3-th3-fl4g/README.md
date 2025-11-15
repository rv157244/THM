# c4ptur3-th3-fl4g
[ROOM](https://tryhackme.com/room/c4ptur3th3fl4g)
## Intro
Esse CTF tem o intuito de mostrar como é um CTF de verdade e as diversas tecnologias e adversidades que podem ser encontradas nesse caminho. Ele tambem, promove de maneira educativa a pequisa e a busca por informações.
## Translation & Shifting
Traduza, desloque e decodifique o seguinte:

Todas as respostas diferenciam maiúsculas de minúsculas.
## Cap 1
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
Base32 é uma codificação binária para texto baseada no sistema numérico de base 32. Utiliza um alfabeto de 32 dígitos , cada um representando uma combinação diferente de 5 bits (2⁵ ) . Como o Base32 não é amplamente adotado, a questão da notação, ou seja, quais caracteres usar para representar os 32 dígitos, não é tão definida quanto no caso de sistemas numéricos mais conhecidos (como o hexadecimal ), embora existam RFCs e padrões não oficiais e de facto. Uma maneira de representar números em Base32 de forma legível por humanos é usando os dígitos 0 a 9 seguidos pelas 22 letras maiúsculas A a V. No entanto, muitas outras variações são usadas em diferentes contextos. Historicamente, o código Baudot pode ser considerado um código Base32 modificado ( com estado ). O Base32 é frequentemente usado para representar cadeias de bytes.


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
### 5 -Hexadecimal
O sistema hexadecimal ( ou simplesmente hex ) é um sistema numérico posicional que representa um valor numérico na base 16. Na convenção mais comum, um dígito é representado por "0" a "9", como no sistema decimal , e por uma letra do alfabeto de "A" a "F" (maiúscula ou minúscula) para os dígitos com valor decimal de 10 a 15.
       
        68 65 78 61 64 65 63 69 6d 61 6c 20 6f 72 20 62 61 73 65 31 36 3f

Resposta: hexadecimal or base16?

Ferraenta: [decoder](https://cryptii.com/pipes/hex-decoder)

**Referencia: [wikipedia](https://en.wikipedia.org/wiki/Hexadecimal)
### 6 - Cezar
 Em criptografia , a cifra de César , também conhecida como cifra de César , cifra de deslocamento , código de César ou deslocamento de César , é uma das técnicas de criptografia mais simples e amplamente conhecidas . É um tipo de cifra de substituição na qual cada letra do texto simples é substituída por uma letra que se encontra um número fixo de posições abaixo no alfabeto . Por exemplo, com um deslocamento para a esquerda de 3, D seria substituído por A , E se tornaria B e assim por diante. [ 1 ] O método recebeu o nome de Júlio César , que o utilizou em sua correspondência privada.

        Ebgngr zr 13 cynprf!
        
Ferramenta: [decoder](https://cryptii.com/pipes/caesar-cipher)

Resposta: Rotate me 13 places!

Referencia: [wiki](https://en.wikipedia.org/wiki/Caesar_cipher)
## Cap 2 - Espectograma!
Um espectrograma , ou sonograma, é o resultado do cálculo do espectro de frequência de um sinal analógico através da análise de janelas temporais. Ele produz um gráfico tridimensional que representa a energia do conteúdo de frequência do sinal à medida que varia ao longo do tempo. [wiki](https://es.wikipedia.org/wiki/Espectrograma)

Abrindo o audio que nos foi fornecido pela plataforma no software audacity, mudamos a vizualização de onda sonora para espctograma

Resposta: Super Secret Message
## Cap 3 - Steganography
Esteganografia é a prática de representar informações dentro de outra mensagem. [wiki](https://pt.wikipedia.org/wiki/Esteganografia)

A ferramenta que usei e o stegcracker. Ela está ultrapassada e a sua sucessora e o Stegseek. O Stegseek e muito mais rapido, mas eu ainda escolhi usar o antigo por se tratar de um ctf silmples.

    Embora eu tenha gostado de construir esta ferramenta, ela foi e sempre será construída sobre bases ruins. O StegCracker começou como uma gambiarra para um problema que não tinha soluções boas ou fáceis de usar; seu maior fator limitante, no entanto, é que ele depende de simplesmente enviar milhares de chamadas de subprocessos por segundo, o que (apesar de ser ligeiramente otimizado com múltiplas threads) é péssimo para o desempenho. Notas do autor...
 
No fim ele gera um arquivo img.png.out que contem a senha. 

### usem o stegseek
## Cap 4 -  Security through obscurity
Segurança por obscuridade é a dependência, na  engenharia de segurança  , do sigilo do projeto ou da implementação como principal método para garantir  a segurança. 

Pesquisando no google, encontrei o site [stegOnline](https://www.georgeom.net/StegOnline/image) quando pedir as strings ele me mostrou. No terminal certas palvras ficaram ocultas.
# Hack The World!
