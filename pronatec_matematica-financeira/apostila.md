# Apostila de Matemática Financeira
## Curso FIC: Operador de Microcomputador (20 horas)
### PRONATEC / Formação Inicial e Continuada

---

## 🌟 Apresentação & Contrato Pedagógico

Seja bem-vindo(a) à disciplina de **Matemática Financeira** do curso de **Operador de Microcomputador**!

Se você em algum momento da sua vida sentiu medo, travamento ou frustração ao olhar para fórmulas matemáticas cheias de letras e símbolos estranhos, temos uma boa notícia: **esta apostila foi feita especialmente para você**.

Como futuro **Operador de Computador**, você já possui uma habilidade fundamental: **entender lógica de comandos**. O computador não é uma máquina "mística"; ele é um assistente extremamente obediente que executa instruções escritas em uma sintaxe específica.

A matemática formal funciona exatamente da mesma maneira!
* Um sinal de **$+$** não é um enigma: é o comando de juntar dois valores.
* Um sinal de **$=$** é a instrução de que o lado esquerdo tem o mesmo peso do lado direito.
* Uma fórmula como **$M = C(1+i)^n$** nada mais é do que um **atalho (script)** para não termos que fazer a mesma conta de multiplicar 12 vezes seguidas.

> [!IMPORTANT]
> **O Contrato Pedagógico do Erro:**
> Nesta disciplina, **errar a sintaxe de uma conta não significa errar a inteligência**. Se você errar um sinal ou parêntese, encararemos isso como um *erro de digitação no teclado* (um "typo"). Ajustamos o comando e seguimos em frente!

---

## 📘 Módulo 1: O Número e a Sintaxe do Computador

### 1.1 Os Conjuntos Numéricos no Cotidiano e na Informática

O computador processa dados na forma de números. Para entender como o computador e o mercado financeiro organizam esses dados, dividimos os números em famílias (conjuntos):

| Conjunto | Símbolo | Exemplos no Dia a Dia | Aplicação no Computador / TI |
| :--- | :---: | :--- | :--- |
| **Naturais** | $\mathbb{N}$ | Quantidade de monitores, impressoras ($0, 1, 2, 3 \dots$) | Contagem de arquivos, quantidade de usuários |
| **Inteiros** | $\mathbb{Z}$ | Saldo bancário positivo ou negativo ($\dots -2, -1, 0, 1, 2 \dots$) | Variação de temperatura de CPU, saldos devedores |
| **Racionais** | $\mathbb{Q}$ | Preço de um produto (R\$ 12,50), metade de uma pizza ($\frac{1}{2}$) | Armazenamento usado ($75,5\%$), valor de parcelas |
| **Reais** | $\mathbb{R}$ | Medidas precisas, constantes matemáticas ($\pi = 3,14159\dots$) | Processamento gráfico 3D, simulações financeiras contínuas |

---

### 1.2 O Papel Central do Zero ($0$)

O número zero é uma das maiores invenções da história da humanidade. Para o Operador de Computador, o zero possui 3 funções vitais:

1. **O Zero como Marcador de Posição (O "Slot" Vazio):**
   Sem o zero, não conseguiríamos diferenciar $15$ de $105$ ou $1005$. O zero indica que aquela "gaveta" posicional está vazia. Em informática, representa o **bit desligado (`0`)** ou o estado ausente (`null`).
2. **O Zero como Ponto de Equilíbrio Financeiro:**
   Na Matemática Financeira, o zero é a linha d'água:
   * **Saldo $> 0$ (Positivo):** Lucro, Crédito, Superávit.
   * **Saldo $= 0$ (Zero):** Equilíbrio, Quitação (não devo, não tenho sobressalente).
   * **Saldo $< 0$ (Negativo):** Débito, Prejuízo, Saldo Devedor.
3. **O Zero como Origem (Referência):**
   Em planilhas e gráficos, o zero ($0,0$) é o ponto de partida onde toda contagem ou medição se inicia.

---

### 1.3 Notação Decimal e o Dinheiro (R\$): A Vírgula como Fronteira

No Brasil, a moeda oficial é o **Real (R\$)**. Escrevemos valores monetários usando a notação decimal.

$$\text{R\$ } 125,75$$

* **À esquerda da vírgula ($125$):** A parte inteira (notas de R\$ 1,00, R\$ 10,00, R\$ 100,00).
* **À direita da vírgula ($75$):** A parte fracionária ou centavos (moedas de centavos, ou seja, partes de 1 Real divididas por 100).

> [!TIP]
> **Dica de Planilha (Excel / LibreOffice Calc):**
> No sistema operacional em português (Brasil), a vírgula `,` separa os decimais e o ponto `.` separa os milhares. No teclado numérico do computador, certifique-se de configurar a célula como estilo **"Moeda"** ou **"Contábil"** para que a formatação `R$` apareça automaticamente!

---

### 1.4 Expressões Numéricas como Algoritmos e Ordem de Precedência

Quando o computador calcula `= 10 + 2 * 5`, qual resultado ele produz? **20** ou **60**?

Para evitar ambiguidades, a matemática e os programas de computador seguem uma **Ordem de Precedência de Operadores**:

1. **Parênteses `( )`:** Executa primeiro o que estiver dentro dos parênteses.
2. **Potenciação / Radiciação (`^`):** Elevação a potências e raízes.
3. **Multiplicação e Divisão (`*` e `/`):** Executadas na ordem em que aparecem (da esquerda para a direita).
4. **Adição e Subtração (`+` e `-`):** Executadas por último.

#### Exemplo Prático de TI:
Um operador precisa comprar 3 teclados de R\$ 50,00 e 2 mouses de R\$ 30,00, com um frete fixo de R\$ 15,00.

$$\text{Total} = 3 \times 50 + 2 \times 30 + 15$$

* **Passo 1 (Multiplicações):** $3 \times 50 = 150$ e $2 \times 30 = 60$.
* **Passo 2 (Somas):** $150 + 60 + 15 = 225$.
* **Fórmula no Excel:** `=3*50 + 2*30 + 15` $\to$ Resultado: `R$ 225,00`.

---

## 📐 Módulo 2: Proporções, Porcentagem e Fatores de Correção

### 2.1 Razão e Proporção

* **Razão:** É a comparação por divisão entre duas grandezas.
  $$\text{Razão} = \frac{A}{B}$$
  *Exemplo:* Se um pendrive de 64 GB custa R\$ 32,00, a razão preço/capacidade é $\frac{32}{64} = 0,50$ (ou seja, R\$ 0,50 por Gigabyte).

* **Proporção:** É a igualdade entre duas razões.
  $$\frac{A}{B} = \frac{C}{D} \implies A \times D = B \times C$$

---

### 2.2 Regra de Três Simples e Composta

A Regra de Três é uma ferramenta prática para descobrir um valor desconhecido ($x$) mantendo a mesma proporção.

#### Exemplo (Regra de Três Simples):
Se um servidor de arquivos realiza o backup de 120 GB de dados em 15 minutos, quantos minutos levará para fazer o backup de 320 GB mantendo a mesma velocidade?

| Dados (GB) | Tempo (minutos) |
| :---: | :---: |
| 120 | 15 |
| 320 | $x$ |

$$\frac{120}{320} = \frac{15}{x} \implies 120 \cdot x = 320 \cdot 15 \implies 120x = 4800 \implies x = \frac{4800}{120} = 40 \text{ minutos}$$

---

### 2.3 Porcentagem como Fração de Base 100

A palavra **porcentagem** significa "por cada cem" (símbolo $\%$).

$$25\% = \frac{25}{100} = 0,25$$

Para converter qualquer porcentagem em número decimal para efetuar cálculos no computador, basta dividir a taxa por $100$:

| Porcentagem (\%) | Fração Centesimal | Número Decimal | Sintaxe no Excel / Calc |
| :---: | :---: | :---: | :---: |
| $5\%$ | $\frac{5}{100}$ | $0,05$ | `5%` ou `0,05` |
| $12\%$ | $\frac{12}{100}$ | $0,12$ | `12%` ou `0,12` |
| $150\%$ | $\frac{150}{100}$ | $1,50$ | `150%` ou `1,5` |

---

### 2.4 Fatores de Correção (Aumento e Desconto Direto)

Calcular a porcentagem e depois somar ou subtrair exige duas etapas de conta. O **Fator de Correção** reduz esse processo a **uma única multiplicação**.

#### 1. Fator de Aumento (Acréscimo):
Quando um valor sofre um aumento de $i\%$, o novo valor corresponderá a $100\% + i\%$.
$$\text{Fator de Aumento} = (1 + i)$$

* **Exemplo:** Aumento de $10\%$ ($i = 0,10$).
  $$\text{Fator} = 1 + 0,10 = 1,10$$
  Se um produto custa R\$ 200,00 e sobe $10\%$, o novo preço é:
  $$\text{Novo Preço} = 200 \times 1,10 = \text{R\$ } 220,00$$

#### 2. Fator de Desconto (Redução):
Quando um valor sofre um desconto de $i\%$, o novo valor corresponderá a $100\% - i\%$.
$$\text{Fator de Desconto} = (1 - i)$$

* **Exemplo:** Desconto de $15\%$ à vista ($i = 0,15$).
  $$\text{Fator} = 1 - 0,15 = 0,85$$
  Se um nobreak custa R\$ 400,00 com $15\%$ de desconto:
  $$\text{Preço à Vista} = 400 \times 0,85 = \text{R\$ } 340,00$$

---

## ⏳ Módulo 3: O Valor do Dinheiro no Tempo e Juros Simples

### 3.1 O Tempo e o Valor do Dinheiro

R\$ 1.000,00 hoje **não valem o mesmo** que R\$ 1.000,00 daqui a 1 ano. Isso ocorre por 3 razões principais:
1. **Inflação:** Perda do poder de compra da moeda com o passar do tempo.
2. **Risco:** Incerteza sobre se o dinheiro futuro será realmente recebido.
3. **Custo de Oportunidade:** Ao emprestar ou investir o dinheiro hoje, abre-se mão de utilizá-lo imediatamente.

Para compensar o tempo, o risco e a oportunidade, cobra-se uma taxa chamada **Juros**.

---

### 3.2 O Conceito de Juros Simples (Capitalização Linear)

No regime de **Juros Simples**, a taxa de juros incide **apenas sobre o Capital Inicial (Principal)** em todos os períodos. O valor dos juros produzidos é constante a cada mês.

#### Variáveis Financeiras Padrão:
* $C$ (ou $PV$): Capital Inicial / Valor Presente (*Present Value*).
* $i$: Taxa de juros (expressa em forma decimal na fórmula).
* $n$ (ou $t$): Tempo / Número de períodos.
* $J$: Valor dos Juros acumulados em R\$.
* $M$ (ou $FV$): Montante Final / Valor Futuro (*Future Value*).

---

### 3.3 As Fórmulas dos Juros Simples

$$\text{Juros: } J = C \cdot i \cdot n$$

$$\text{Montante: } M = C + J \implies M = C(1 + i \cdot n)$$

> [!CAUTION]
> **Regra de Ouro do Tempo e da Taxa:**
> A taxa de juros ($i$) e o tempo ($n$) **DEVEM ESTAR NA MESMA UNIDADE DE TEMPO**!
> * Se a taxa for ao mês (% a.m.), o tempo deve ser digitado em meses.
> * Se a taxa for ao ano (% a.a.), o tempo deve ser digitado em anos.

#### Exemplo Prático:
Uma empresa de informática tomou um empréstimo de R\$ 5.000,00 a uma taxa de juros simples de $2\%$ ao mês, para ser quitado em 6 meses. Qual o valor dos juros e o montante final pago?

* **Dados:** $C = 5000$, $i = 2\% \text{ a.m.} = 0,02$, $n = 6 \text{ meses}$.
* **Cálculo dos Juros ($J$):**
  $$J = 5000 \times 0,02 \times 6 = 100 \times 6 = \text{R\$ } 600,00$$
* **Cálculo do Montante ($M$):**
  $$M = 5000 + 600 = \text{R\$ } 5.600,00$$
* **Fórmula na Planilha:** `=5000*(1 + 0,02*6)` $\to$ `R$ 5.600,00`.

---

### 3.4 Desconto Simples Comercial (Bancário)

No comércio e nos bancos, ao antecipar um título de crédito (duplicata ou cheque pré-datado), o desconto é calculado sobre o valor nominal futuro ($N$):

$$D = N \cdot d \cdot n$$
$$V_L = N - D = N(1 - d \cdot n)$$

Onde:
* $N$: Valor Nominal (valor impresso no título para o futuro).
* $d$: Taxa de desconto comercial.
* $n$: Período de antecipação.
* $V_L$: Valor Líquido recebido hoje.

---

## 🚀 Módulo 4: Juros Compostos e Crescimento Exponencial

### 4.1 Potenciação: O Atalho da Multiplicação Repetida

Assim como a multiplicação é um atalho para somar o mesmo número várias vezes ($5 + 5 + 5 = 3 \times 5$), a **potenciação** é o atalho para multiplicar o mesmo fator várias vezes:

$$1,10 \times 1,10 \times 1,10 = 1,10^3 = 1,331$$

No teclado do computador e no Excel, o operador de potenciação é o **acento circunflexo (`^`)**.
* `1,10^3` produz `1,331`.

---

### 4.2 Construção Indutiva dos Juros Compostos

Nos **Juros Compostos**, os juros de cada período são incorporados ao capital para o cálculo dos juros do período seguinte (**"Juros sobre Juros"**).

Vamos acompanhar o investimento de **R\$ 1.000,00** a **$10\%$ ao mês ($i = 0,10$)** durante **3 meses**:

#### Método 1: Passo a passo (manual longo)
* **Fim do Mês 1:** $1000 + (1000 \times 0,10) = 1000 + 100 = \text{R\$ } 1.100,00$
* **Fim do Mês 2:** $1100 + (1100 \times 0,10) = 1100 + 110 = \text{R\$ } 1.210,00$
* **Fim do Mês 3:** $1210 + (1210 \times 0,10) = 1210 + 121 = \text{R\$ } 1.331,00$

#### Método 2: Usando o Fator de Correção ($1,10$) em Cadeia
* **Mês 1:** $1000 \times 1,10 = 1100$
* **Mês 2:** $(1000 \times 1,10) \times 1,10 = 1000 \times 1,10^2 = 1210$
* **Mês 3:** $(1000 \times 1,10 \times 1,10) \times 1,10 = 1000 \times 1,10^3 = 1331$

Observe o padrão! Para 3 meses, multiplicamos por $1,10^3$. Para 12 meses, seriam $1,10^{12}$.

---

### 4.3 A Fórmula Geral do Montante Composto

Substituindo os números pelas variáveis financeiras, chegamos à fórmula universal dos Juros Compostos:

$$M = C \cdot (1 + i)^n \quad \text{ou} \quad FV = PV \cdot (1 + i)^n$$

* **$M$ ou $FV$:** Montante Final / Valor Futuro.
* **$C$ ou $PV$:** Capital Inicial / Valor Presente.
* **$i$:** Taxa de juros em forma decimal.
* **$n$:** Número de períodos.

---

### 4.4 Valor Presente ($PV$) vs. Valor Futuro ($FV$)

Se quisermos saber quanto precisamos investir **HOJE ($PV$)** para obter um determinado valor no **FUTURO ($FV$)**, basta inverter a fórmula multiplicando pelo fator divisor:

$$PV = \frac{FV}{(1 + i)^n} = FV \cdot (1 + i)^{-n}$$

#### Exemplo Prático:
Você quer comprar um servidor novo de R\$ 12.100,00 daqui a 2 anos. Quanto precisa aplicar hoje em um investimento que rende $10\%$ ao ano em juros compostos?

* **Dados:** $FV = 12100$, $i = 0,10 \text{ a.a.}$, $n = 2 \text{ anos}$.
* **Cálculo:**
  $$PV = \frac{12100}{(1 + 0,10)^2} = \frac{12100}{1,10^2} = \frac{12100}{1,21} = \text{R\$ } 10.000,00$$
* **No Excel:** `=12100 / (1,10^2)` $\to$ `R$ 10.000,00`.

---

## 📊 Módulo 5: Séries de Pagamentos, Planilhas Eletrônicas e Tomada de Decisão

### 5.1 Noções de Progressões (PA e PG) nas Finanças

* **Progressão Aritmética (PA):** Ocorre quando adicionamos uma quantidade constante a cada termo.
  * *Aplicação:* Amortização constante de dívidas ou depósitos simples de valor fixo sem rendimento acumulado.
* **Progressão Geométrica (PG):** Ocorre quando multiplicamos o termo anterior por um fator constante ($q = 1+i$).
  * *Aplicação:* Evolução de saldo de juros compostos e parcelamentos em séries de pagamentos (anuidades).

---

### 5.2 As Funções Financeiras das Planilhas Eletrônicas (Excel / LibreOffice Calc)

No dia a dia do Operador de Computador, os cálculos financeiros não precisam ser feitos à mão. As planilhas possuem funções prontas em Português:

| Função no Excel | O que ela calcula? | Sintaxe da Fórmula |
| :--- | :--- | :--- |
| **`=VF(taxa; nper; pgto; [vp])`** | Valor Futuro ($FV$) de uma aplicação | `=VF(0,01; 12; 0; -1000)` |
| **`=VP(taxa; nper; pgto; [vf])`** | Valor Presente ($PV$) atual de um valor futuro | `=VP(0,01; 12; 0; 1126,83)` |
| **`=PGTO(taxa; nper; vp; [vf])`** | Valor da parcela periódica de um empréstimo | `=PGTO(0,02; 10; -5000)` |
| **`=NPER(taxa; pgto; vp; [vf])`** | Número de parcelas/períodos necessários | `=NPER(0,02; -550; 5000)` |
| **`=TAXA(nper; pgto; vp; [vf])`** | Taxa de juros cobrada em um financiamento | `=TAXA(12; -100; 1000)` |

> [!NOTE]
> **Convenção de Sinal do Fluxo de Caixa no Excel:**
> * Valores cobrados / saídas de caixa entram com sinal **NEGATIVO (`-`)**.
> * Valores recebidos / entradas de caixa entram com sinal **POSITIVO (`+`)**.

---

### 5.3 Interpretação de Gráficos e Tomada de Decisão

Como Operador de Computador, você frequentemente apresentará relatórios e gráficos para gerentes e clientes:

1. **Gráfico de Colunas / Barras:** Ideal para comparar custos de fornecedores de TI (ex: comparar orçamento de 3 lojas de suprimentos).
2. **Gráfico de Linha:** Perfeito para mostrar a **evolução do saldo no tempo** (comparando o crescimento linear de juros simples com a curva exponencial de juros compostos).

```
  Montante (R$)
    ^
    |                                 * (Juros Compostos - Exponencial)
    |                         *
    |                 *       + (Juros Simples - Linear)
    |         *       +
    | *       +
    +---------+-------+-------+-------> Tempo (n)
```

---

## 📝 Caderno de Exercícios Práticos & Gabarito Comentado

### Lista de Exercícios

#### 1. Sintaxe de Precedência (Módulo 1)
Um técnico comprou 4 memórias RAM por R\$ 120,00 cada, 2 SSDs por R\$ 250,00 cada e obteve um desconto promocional total de R\$ 80,00.
* **a)** Escreva a expressão numérica correspondente ao valor final.
* **b)** Qual o resultado final calculado?

#### 2. Porcentagem e Fator de Correção (Módulo 2)
Um computador gamer custava R\$ 4.000,00. Na Black Friday, a loja ofereceu um desconto de $12\%$ para pagamento à vista via PIX.
* **a)** Qual é o fator de desconto aplicado?
* **b)** Qual o valor final a ser pago à vista?

#### 3. Juros Simples (Módulo 3)
Um microempresário tomou um empréstimo de R\$ 3.000,00 para trocar os cabos de rede de sua empresa, a uma taxa de juros simples de $3\%$ ao mês, para pagamento total após 5 meses.
* **a)** Qual o valor dos juros cobrados?
* **b)** Qual o montante final quitado?

#### 4. Juros Compostos (Módulo 4)
Se você aplicar R\$ 2.000,00 em uma caderneta ou fundo de renda fixa que rende $1\%$ ao mês em juros compostos, quanto terá ao final de 4 meses?
*(Dica: Use a fórmula $M = C(1+i)^n$ e calcule $(1,01)^4$).*

#### 5. Planilha Eletrônica (Módulo 5)
Qual fórmula você digitaria no Excel para descobrir a prestação mensal de um financiamento de R\$ 10.000,00 feito em 12 parcelas a uma taxa de $1,5\%$ ao mês?

---

### 🔑 Gabarito Comentado

#### Resolução do Exercício 1:
* **a) Expressão Numérica:** $4 \times 120 + 2 \times 250 - 80$
* **b) Cálculo:**
  * Multiplicações: $480 + 500 - 80$
  * Operações finais: $980 - 80 = \text{R\$ } 900,00$
  * *No Excel:* `=4*120 + 2*250 - 80`

#### Resolução do Exercício 2:
* **a) Fator de Desconto:** $1 - 0,12 = 0,88$
* **b) Valor Final:** $4000 \times 0,88 = \text{R\$ } 3.520,00$
  * *No Excel:* `=4000 * (1 - 0,12)`

#### Resolução do Exercício 3:
* **a) Juros:** $J = C \cdot i \cdot n = 3000 \times 0,03 \times 5 = \text{R\$ } 450,00$
* **b) Montante:** $M = C + J = 3000 + 450 = \text{R\$ } 3.450,00$

#### Resolução do Exercício 4:
* **Dados:** $C = 2000$, $i = 0,01$, $n = 4$.
* **Fórmula:** $M = 2000 \times (1 + 0,01)^4 = 2000 \times (1,01)^4$
* **Cálculo da Potência:** $1,01^4 \approx 1,040604$
* **Montante:** $M = 2000 \times 1,040604 = \text{R\$ } 2.081,21$
* *No Excel:* `=2000 * (1,01^4)` ou `=VF(1%; 4; 0; -2000)`

#### Resolução do Exercício 5:
* **Fórmula no Excel:** `=PGTO(1,5%; 12; -10000)`
* **Resultado aproximado:** `R$ 916,80` por mês.

---
*Apostila desenvolvida para o Curso de Operador de Microcomputador - PRONATEC / FIC.*
