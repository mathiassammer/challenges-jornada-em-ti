# Desafio da Criptografia

Um texto em inglês precisa ser criptografado usando o seguinte esquema de criptografia.

Primeiro, os espaços são removidos do texto. Deixar ***L*** seja o comprimento deste texto.  

Em seguida, os caracteres são escritos em uma grade, cujas linhas e colunas possuem as seguintes restrições:
[raíz quadrada de ***L***] <= linha <= coluna <= [raíz quadrada de ***L***]

**Exemplo**

Depois de remover os espaços, a string é **54** caracteres longos. A raíz quadrada de 54 está entre **7** e **8**, por isso é escrito na forma de uma grade com 7 linhas e 8 colunas.

```
ifmanwas  
meanttos          
tayonthe  
groundgo  
dwouldha  
vegivenu  
sroots
```

- Garanta que **linhas x colunas** >= ***L***
- Se várias grades satisfizerem as condições acima, escolha aquela com a área mínima, ou seja, **linhas x colunas**.

A mensagem codificada é obtida exibindo os caracteres de cada coluna, com um espaço entre os textos das colunas. A mensagem codificada para a grade acima é:

`imtgdvs fearwer mayoogo anouuio ntnnlvt wttddes aohghn sseoau`

Crie uma função para codificar uma mensagem.

**Descrição da função**

Complete a função de _criptografia_ no editor abaixo.

criptografia tem os seguintes parâmetros:

-   _string s:_ uma string para criptografar

**Devoluções**

-   _string:_ a string criptografada

**Formato de entrada**

Uma linha de texto, a string ***s***

**Restrições**

1 <= length of ***s*** <= 81
***s*** contém caracteres no intervalo ascii[az] e espaço, ascii(32).

**Entrada de amostra**
```
haveaniceday

```

**Saída de Amostra**
```
hae and via ecy
```

**Explicação 1**

***L*** = 12, raíz quadrada de 12 está entre 3 e 4.
Reescrito com 3 linhas e 4 colunas:
```
have
anic
eday

```

**Entrada de Amostra 1**
```
feedthedog    

```

**Saída de Amostra 1**
```
fto ehg ee dd
```

**Explicação 2**

L = 10, raíz quadrada de 10 está entre 3 e 4.
Reescrito com 3 linhas e 4 colunas:
```
feed
thed
og

```

**Entrada de Amostra 2**
```
chillout

```

**Saída de Amostra 2**
```
clu hlt io
```

**Explicação 3**

L = 8, raíz quadrada de 8 está entre 2 e 3.
Reescrito com 3 colunas e 3 linhas (2 * 3 = 6 < 8 então temos que usar 3 x 3.)
```
chi
llo
ut
```