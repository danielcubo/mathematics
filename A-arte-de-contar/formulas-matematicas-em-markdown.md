## 💡 Dica de Visualização

\begin{aligned} ... \end{aligned} separado por & (para alinhar) e \\ (para quebrar a linha).

### Distância entre Dois Pontos no Plano $R^2$
A distância $d$ entre os pontos $A(x_1, y_1)$ e $B(x_2, y_2)$ é dada por:

$$d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}$$

### Sistema Linear em Forma Matricial
Podemos representar um sistema de equações lineares através do produto matricial:

$$\begin{pmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{pmatrix} \begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} b_1 \\ b_2 \end{pmatrix}$$

O determinante da matriz principal $A$ é calculado por:
$$\det(A) = a_{11}a_{22} - a_{12}a_{21}$$

### Equações de Matemática Financeira

* **Juros Simples:** O montante final $M$ é linear:
  $$M = P \cdot (1 + i \cdot t)$$

* **Juros Compostos:** O valor cresce exponencialmente ao longo do tempo:
  $$M = P \cdot (1 + i)^t$$

> **Legenda:** $M$ = Montante, $P$ = Capital Principal, $i$ = Taxa de juros, $t$ = Tempo.

### Elasticidade-Preço da Demanda ($\epsilon_d$)
Mede a sensibilidade da quantidade demandada ($Q$) em relação às mudanças no preço ($P$):

$$\epsilon_d = \frac{\% \Delta Q}{\% \Delta P} = \frac{\Delta Q}{\Delta P} \cdot \frac{P}{Q}$$

### Fundamentos do Cálculo

* **Definição de Derivada:** A derivada de $f(x)$ em relação a $x$ é o limite da taxa de variação média:
  $$f'(x) = \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}$$

* **Regra da Cadeia:** Para funções compostas $f(g(x))$:
  $$\frac{dy}{dx} = \frac{dy}{du} \cdot \frac{du}{dx}$$

### Integração
O **Teorema Fundamental do Cálculo** estabelece a relação entre a diferenciação e a integração:

$$\int_{a}^{b} f(x) \, dx = F(b) - F(a)$$

Onde $F'(x) = f(x)$. A integral indefinida inclui a constante de integração:
$$\int x^n \, dx = \frac{x^{n+1}}{n+1} + C \quad (\text{para } n \neq -1)$$

### Análise Estatística

* **Média Amostral ($\bar{x}$):**
  $$\bar{x} = \frac{1}{n} \sum_{i=1}^{n} x_i$$

* **Função de Densidade de Probabilidade (Distribuição Normal):**
  $$f(x) = \frac{1}{\sigma \sqrt{2\pi}} e^{-\frac{1}{2}\left(\frac{x-\mu}{\sigma}\right)^2}$$


# Relatório Técnico: Análise de Otimização Financeira e Cálculo de Produção

**Autor:** Seu Nome Completo  
**Instituição:** Nome da Organização ou Universidade  
**Data:** 23 de maio de 2026  

---

## 1. Introdução
Este relatório apresenta a modelagem matemática para a otimização de lucros em cenários de produção industrial, integrando conceitos de Cálculo Diferencial e Matemática Financeira (Juros Compostos). O objetivo é determinar o ponto de máximo retorno e projetar o valor futuro dos ativos gerados.

## 2. Definição de Variáveis e Parâmetros
A tabela abaixo descreve as variáveis utilizadas nas equações deste documento:


| Símbolo | Descrição | Unidade de Medida |
| :---: | :--- | :---: |
| $L(x)$ | Função Lucro Líquido | R$ |
| $R(x)$ | Função Receita Total | R$ |
| $C(x)$ | Função Custo Total de Produção | R$ |
| $x$ | Quantidade de unidades produzidas | Unidades |
| $V_f$ | Valor Futuro (Montante acumulado) | R$ |
| $i$ | Taxa de juros por período | % |
| $t$ | Tempo de aplicação | Meses |

---

## 3. Modelagem e Otimização (Cálculo)
Considerando que a receita e o custo de produção seguem comportamentos quadráticos e lineares, respectivamente, definimos as funções abaixo:

$$R(x) = -2x^2 + 120x$$
$$C(x) = 20x + 300$$

### 3.1 Determinação do Lucro Máximo
O lucro é dado por $L(x) = R(x) - C(x)$. Para encontrar o ponto de produção ideal, aplicamos a primeira derivada ($L'(x) = 0$):

$$\begin{aligned}
L(x) &= (-2x^2 + 120x) - (20x + 300) \\
L(x) &= -2x^2 + 100x - 300 \\
\\
L'(x) &= \frac{dL}{dx} = -4x + 100 \\
\\
0 &= -4x + 100 \\
4x &= 100 \\
x_{otimo} &= 25 \text{ unidades}
\end{aligned}$$

> 💡 **Conclusão Parcial:** A empresa atinge o lucro máximo quando produz exatamente **25 unidades**. Qualquer valor acima ou abaixo reduz a eficiência econômica.

---

## 4. Projeção Financeira (Economia e Juros)
O lucro obtido no ponto ótimo ($L(25)$) será reinvestido em um fundo de investimento de alta liquidez sob o regime de **juros compostos**.

### 4.1 Cálculo do Capital Inicial ($P$)
$$\begin{aligned}
L(25) &= -2(25)^2 + 100(25) - 300 \\
L(25) &= -2(625) + 2500 - 300 \\
L(25) &= -1250 + 2500 - 300 \\
P &= 950 \text{ R\$}
\end{aligned}$$

### 4.2 Projeção do Valor Futuro ($V_f$)
Utilizando a fórmula clássica de juros compostos para uma taxa $i = 1\%$ ao mês ($0,01$) durante um período de $t = 12$ meses:

$$V_f = P \cdot (1 + i)^t$$

$$\begin{aligned}
V_f &= 950 \cdot (1 + 0,01)^{12} \\
V_f &= 950 \cdot (1,01)^{12} \\
V_f &\approx 950 \cdot 1,126825 \\
V_f &\approx 1.070,48 \text{ R\$}
\end{aligned}$$

---

## 5. Considerações Finais
A aplicação do cálculo diferencial permitiu identificar com precisão o teto de eficiência produtiva da operação. Complementarmente, a projeção financeira indica que o reinvestimento do lucro gerará um ganho passivo bruto de **R$ 120,48** ao final de um ano.


# 🧮 Fórmulas Estruturais e Conceitos Matemáticos

Coleção de blocos de equações e matrizes para documentação de fundamentos lógicos e geométricos.

---

## 📐 1. Trigonometria Básica e Triângulos

Essencial para o cálculo de ângulos e movimentação de eixos no desenvolvimento de robótica e motores.

### Teorema de Pitágoras
$$a^2 = b^2 + c^2$$

### Relação Fundamental da Trigonometria
$$\operatorname{sen}^2(\theta) + \cos^2(\theta) = 1$$

### Lei dos Cossenos
$$a^2 = b^2 + c^2 - 2bc \cdot \cos(\alpha)$$

---

## 📈 2. Álgebra Linear e Sistemas de Coordenadas

Utilizado na renderização de gráficos em duas dimensões (Front-end) e posicionamento espacial.

### Função Afim (Equação da Reta)
$$f(x) = ax + b$$

### Distância entre Dois Pontos no Plano Cartesiano
$$d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}$$

### Equação Geral da Circunferência
$$(x - x_0)^2 + (y - y_0)^2 = R^2$$

---

## 🧮 3. Álgebra e Equações Polinomiais

Estruturas clássicas de cálculo de trajetórias e raízes.

### Equação de Segundo Grau (Fórmula de Bhaskara)
$$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

### Produto Notável (Diferença de Quadrados)
$$(a + b)(a - b) = a^2 - b^2$$

---

## 🧠 4. Lógica Booleana e Teoria dos Conjuntos

A base matemática oculta por trás das portas lógicas do processador e das consultas em bancos de dados (`SQL`).

### Operações de Conjuntos (União e Interseção)
$$A \cup B = \{x \mid x \in A \text{ ou } x \in B\}$$
$$A \cap B = \{x \mid x \in A \text{ e } x \in B\}$$

### Leis de De Morgan (Lógica de Programação)
$$\neg(P \land Q) \iff (\neg P \lor \neg Q)$$
$$\neg(P \lor Q) \iff (\neg P \land \neg Q)$$

---

## ⚡ 5. Cálculo Diferencial (Fundamentos)

A base para entender taxas de variação contínua e otimização de algoritmos complexos.

### Definição de Derivada por Limite
$$f'(x) = \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}$$

### Regra da Cadeia (Derivada Composta)
$$\frac{dy}{dx} = \frac{dy}{du} \cdot \frac{du}{dx}$$

## 📐 6. Estruturas e Notações de Funções

### Definição Formal de Função (Domínio e Imagem)
Define o mapeamento de um conjunto de entrada (A) para um conjunto de saída (B).

$$f: A \to B$$
$$x \mapsto f(x)$$

---

### Função Definida por Partes (Condicionais / IF-ELSE)
A estrutura `\begin{cases}` é o equivalente matemático aos blocos condicionais (`if/else`) da programação. Ela agrupa as regras da função.

$$f(x) = \begin{cases} 
x, & \text{se } x \ge 0 \\ 
-x, & \text{se } x < 0 
\end{cases}$$

---

### Função Modular (Exemplo de Sintaxe)
$$\lvert x \rvert = \begin{cases} 
x, & \text{se } x \ge 0 \\ 
-x, & \text{se } x < 0 
\end{cases}$$

---

### Função Composta (Função dentro de Função)
$$(f \circ g)(x) = f(g(x))$$

---

### Notação de Limite de uma Função
$$\lim_{x \to a} f(x) = L$$



## ⨍ 6. Notação e Estruturas de Funções

Modelos matemáticos para representação de escopos, domínios, e funções definidas por condições (condicionais lógicas).

### Definição Formal de Domínio e Imagem
Esta notação indica que a função $f$ mapeia elementos do conjunto de partida $A$ (Domínio) para o conjunto de chegada $B$ (Contradomínio).

$$f: A \to B$$

### Função Definida por Partes (Condicionais / If-Else Matemático)
Esta estrutura usa o ambiente `cases` para definir comportamentos diferentes da função baseados em restrições do domínio (o equivalente direto à lógica `if/else` na programação).

$$f(x) = \begin{cases} -x, & \text{se } x < 0 \\ 0, & \text{se } x = 0 \\ x, & \text{se } x > 0 \end{cases}$$

### Composição de Funções (Função Composta)
Representação de uma função aplicada dentro de outra função, conceito fundamental no desenvolvimento de arquiteturas de software e programação funcional.

$$(f \circ g)(x) = f(g(x))$$

### Definição de Limite de uma Função
A base do cálculo diferencial para analisar o comportamento de uma função quando a variável se aproxima de um determinado ponto.

$$\lim_{x \to a} f(x) = L$$

# 🎛️ Portas Lógicas Digitais e Comandos de Sincronização Git

Este documento registra a lógica booleana que governa o hardware (circuitos elétricos do Z80 e Arduino) e os comandos necessários para salvar esta documentação no GitHub.

---

## ⚡ 1. As Portas Lógicas Fundamentais

No nível do hardware, as informações são apenas tensões elétricas: `0` (0V / FALSE) ou `1` (5V ou 3.3V / TRUE). As portas lógicas manipulam esses bits.

### Porta NOT (Inversora)
Inverte o sinal de entrada. Se entra 1, sai 0. Se entra 0, sai 1.
*   **Expressão Matemática:** $Y = \bar{A}$ ou $Y = \neg A$
*   **Tabela Verdade:**
    $$\begin{array}{|c|c|} \hline A & Y \\ \hline 0 & 1 \\ 1 & 0 \\ \hline \end{array}$$

### Porta AND (E)
A saída só será 1 se **todas** as entradas forem iguais a 1. Funciona como uma multiplicação binária.
*   **Expressão Matemática:** $Y = A \cdot B$ ou $Y = A \land B$
*   **Tabela Verdade:**
    $$\begin{array}{|c|c|c|} \hline A & B & Y \\ \hline 0 & 0 & 0 \\ 0 & 1 & 0 \\ 1 & 0 & 0 \\ 1 & 1 & 1 \\ \hline \end{array}$$

### Porta OR (OU)
A saída será 1 se **pelo menos uma** das entradas for igual a 1. Funciona como uma soma lógica.
*   **Expressão Matemática:** $Y = A + B$ ou $Y = A \lor B$
*   **Tabela Verdade:**
    $$\begin{array}{|c|c|c|} \hline A & B & Y \\ \hline 0 & 0 & 0 \\ 0 & 1 & 1 \\ 1 & 0 & 1 \\ 1 & 1 & 1 \\ \hline \end{array}$$

### Porta XOR (OU Exclusivo)
A saída será 1 apenas se as entradas forem **diferentes**. Muito utilizada em circuitos somadores de CPU.
*   **Expressão Matemática:** $Y = A \oplus B$
*   **Tabela Verdade:**
    $$\begin{array}{|c|c|c|} \hline A & B & Y \\ \hline 0 & 0 & 0 \\ 0 & 1 & 1 \\ 1 & 0 & 1 \\ 1 & 1 & 0 \\ \hline \end{array}$$

---

## 🚀 2. Aplicação Prática no Arduino

No código do Arduino, essas portas se traduzem em **Operadores Booleanos** dentro das condicionais (`if/else`):

```cpp
// Exemplo de lógica AND (&&) e NOT (!) no Arduino
if (digitalRead(pino_sensor) == HIGH && !sistema_bloqueado) {
    digitalWrite(pino_motor, HIGH); // Liga o motor se o sensor ativar E o sistema NÃO estiver bloqueado
}
```

---

## 📂 3. Comandos Git para Sincronizar esta Documentação

Use estes comandos no terminal do seu computador para salvar este arquivo diretamente na sua pasta `Building-my-computer` e enviar para o celular através do GitHub:

### Passo 1: Entrar na pasta do repositório
```bash
cd /caminho/do/seu/repositorio/Documentation/Building-my-computer
```

### Passo 2: Verificar o status do repositório
Mostra se o Git identificou o novo arquivo que você criou.
```bash
git status
```

### Passo 3: Adicionar o arquivo para a esteira de envio
```bash
git add portas-logicas-e-fundamentos.md
```

### Passo 4: Criar o ponto de salvamento (Commit)
O commit precisa de uma mensagem direta e clara, sem rodeios.
```bash
git commit -m "feat: add documentacao de portas logicas"
```

### Passo 5: Enviar os dados para o servidor do GitHub
Depois desse comando, o arquivo estará disponível para você ler no seu celular.
```bash
git push origin main
```
