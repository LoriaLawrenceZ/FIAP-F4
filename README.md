<div name="readme-top">
    <h1 align=center>CAPÍTULO 3</h1>
</div>

>**Capítulo 3 - Hardware e os Números**

# DESVENDANDO OS SITEMAS

A base de um sistema de numeração se refere à quantidade de símbolos presentes no sistema. Assim, indo do 0 ao 9, nosso sistema é dito **decimal**, ou de **base 10**, pois possuí 10 simbolos.

>**Algarismos dos Sistemas Numéricos Mais Diretamente Ligados aos Computadores**

Representa os algarismos dos sistemas numéricos mais diretamente ligados à informática.

| Algarismos                                                                                                      | Sistema Numérico        | Qnt. Símbolos   |
|:----------------------------------------------------------------------------------------------------------------|:------------------------|:----------------|
| **0**, **1**, **2**, **3**, **4**, **5**, **6**, **7**, **8**, **9**, **A**, **B**, **C**, **D**, **E** e **F** | Sistema **hexadecimal** | **16** símbolos |
| **0**, **1**, **2**, **3**, **4**, **5**, **6**, **7**, **8** e **9**                                           | Sistema **decimal**     | **10** símbolos |
| **0**, **1**, **2**, **3**, **4**, **5**, **6** e **7**                                                         | Sistema **octal**       | **8** símbolos  |
| **0** e **1**                                                                                                   | Sistema **binário**     | **2** símbolos  |

Uma observação importante sobre a quantidade de símbolos de um sistema e sua potencialidade, é dada pelo seguinte exemplo: **FF** na base **16** é igual a **255** na base **10**, a **377** na base **8** e a **11111111** na base **2**, ou seja, bases maiores tornam a representação dos valores mais compacta.

<p align="right">(<a href="#readme-top">back to top</a>)

# REPRESENTAÇÃO DE UM NÚMERO E SUA BASE

Para discrimar corretamente um número e sua base, escrevemos a base em subscrito juntamente com o número.

![img.png](assets/img/img.png)

## Contagem nas Principais Bases

A contagem começa a partir de zero e vai de um em um nas quatro principais bases, usando:

- Um único algorismo nos números hexadecimais
- Dois algorismos nos números decimais
- Dois algorismos nos números octais
- Quatro algorismos nos números binários

Processo de contagem nas bases apresentadas na tabela anteriormente.

![img.png](assets/img/img2.png)

>**Equivalência entre valores**

Representa equivalência dos valores de 0 até 16 nas quatro bases.

| Base 2 (4 algarismos) | Base 8 (3 algarismos) | Base 10 (2 algarismos) | Base 16 (1 algarismo) |
|:----------------------|:----------------------|:-----------------------|:----------------------|
| 0000                  | 00                    | 00                     | 0                     |
| 0001                  | 01                    | 01                     | 1                     |
| 0010                  | 02                    | 02                     | 2                     |
| 0011                  | 03                    | 03                     | 3                     |
| 0100                  | 04                    | 04                     | 4                     |
| 0101                  | 05                    | 05                     | 5                     |
| 0110                  | 06                    | 06                     | 6                     |
| 0111                  | 07                    | 07                     | 7                     |
| 1000                  | 10                    | 08                     | 8                     |
| 1001                  | 11                    | 09                     | 9                     |
| 1010                  | 12                    | 10                     | A                     |
| 1011                  | 13                    | 11                     | B                     |
| 1100                  | 14                    | 12                     | C                     |
| 1101                  | 15                    | 13                     | D                     |
| 1110                  | 16                    | 14                     | E                     |
| 1111                  | 17                    | 15                     | F                     |

A extensão de um número ou valor em uma determinada base refere-se à quantidade de dígitos ou algarismos que compõem o número. Sendo assim, on números **1(16)**, **11(16)** e **1111(16)** na base **16** possuem, respectivament, extensões de 1, 2 e 4 dígitos. Os números **253(8)**, **12(10)** e **10110101(2)** têm, respectivamente, extensões de 3, 2 e 8 dígitos.

<details close>
    <summary><code>VÍDEO | A Origem da Informação e sua Relação com as Bases Numéricas</code></summary>

### Representação da base 2

A representação na base dois é feita pegando o número e dividindo-o sucessivamente por 2, guardando o resto da divisão. Por exemplo, para o número 214, temos:

> - 214 / 2 = 107 -> 0<br>
> - 107 / 2 = 53 -> 1<br>
> - 53 / 2 = 26 -> 1<br>
> - 26 / 2 = 13 -> 0<br>
> - 13 / 2 = 6 -> 1<br>
> - 6 / 2 = 3 -> 0<br>
> - 3 / 2 = 1 -> 1<br>
> - 1 / 2 = 0 -> 1<br>

>214(10) = 11010110(2)

> Não se esquecer de inverter depois!<br>
> Divisão: 0 - 1 - 1 - 0 - 1 - 0 - 1 - 1<br>
> Representação: 11010110

### Representação da base 8

A representação na base oito é feita pegando o número e dividindo-o sucessivamente por 8, guardando o resto da divisão. Por exemplo, para o número 214, temos:

> - 214 / 8 = 26 -> 6<br>
> - 26 / 8 = 3 -> 2<br>
> - 3 / 8 = 0 -> 3<br>

>214(10) = 326(8)

> Não se esquecer de inverter depois!<br>
> Divisão: 6 - 2 - 3<br>
> Representação: 326

### Representação da base 10

A representação na base dez é feita pegando o número e dividindo-o sucessivamente por 10, guardando o resto da divisão. Por exemplo, para o número 214, temos:

> - 214 / 10 = 21 -> 4<br>
> - 21 / 10 = 2 -> 1<br>
> - 2 / 10 = 0 -> 2<br>

>214(10) = 214(10)

> Não se esquecer de inverter depois!<br>
> Divisão: 4 - 1 - 2<br>
> Representação: 214

### Representação da base 16

A representação na base dezesseis é feita pegando o número e dividindo-o sucessivamente por 16, guardando o resto da divisão. Por exemplo, para o número 214, temos:

> - 214 / 16 = 13 -> 6 (6)<br>
> - 13 / 16 = 0 -> D (13)<br>

>214(10) = D6(16)

> Não se esquecer de inverter depois!<br>
> Divisão: 6 - D<br>
> Representação: D6

</details>

Na base 2, a extensão de um número quase sempre é dada em **bits** em vez de dígitos. Por exemplo, 101001(2) possue 6 bits de extensão. Seja o número 214(10), é possível representar como:

| ![img.png](assets/img/img3.png) | ![img_1.png](assets/img/img4.png) |
|:-------------------------------:|:---------------------------------:|

No qual os números em vermelho, ou seja, as potências de 10 são índices associados a cada dígito do número original.

<p align="right">(<a href="#readme-top">back to top</a>)
