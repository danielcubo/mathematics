Enquanto funções lidam com o que é **previsível e determinístico** (se eu acelerar a uma velocidade constante, sei exatamente onde vou chegar), a **Análise Combinatória**, a **Probabilidade** e a **Estatística** formam o tripé que nos permite lidar com o **imprevisível**, **incerto** e o **caos**.

## ⚖️ Álgebra e equações ($ax+b=0$)
O termo "*álgebra*" vem do árabe `al-jabr`, que significa "*reunião das partes quebradas*", "*restauração*" ou "*complementação*".
 
Em aproximadamente 820 d.C., o matemático Persa **Abdallah Muhammad ibn Musa al-Khwarizmi** (seu sobrenome **al-Khwarizmi** significa "*nativo de Khwarizmi*", região do atual Uzbequistão), publicou seu famoso livro *`Al-Kitab al-Mukhtasar fi Hisab al-Jabr wal-Muqabala`* que significa *`O livro conciso sobre cálculo algébrico`*, referindo-se à transposição de termos subtraídos para o outro lado da equação.

O termo `al-Jabr` que está no título do livro, significa "*reunião das partes*". Originalmente descrevia o tratamento de ossos fraturados, sendo um termo médico antes de ser matemático.

A obra tratava da resolução de equações (*igualar* em latim) por meio da *restauração* (passar de uma lado para o outro) e *balanço* (redução).

Quando a obra foi traduzida para latim no século XII, o termo foi adaptado para `álgebra`, consolidando o nome da disciplina.

Em suma, `álgebra` é a técnica de *consertar equações*, movendo termos negativos para o outro lado para torná-los positivos, criando assim um equilíbrio.

1. `Al-Jabr` (Restauração)
A técnica da restauração consistia em eliminar um termo negativo de uma lado da equação, movendo-o para o outro lado. Isso restaurava a quantidade que estava sendo subtraída, transformando-a em algo positivo e inteiro.

$$x^2-10 = 15$$
$$x^2 = 15+10$$
$$x^2= 25$$

2. `Al-Muqabala` (Redução ou Balanço)
Após restaurar os termos, vinha a *redução*. Isso significava simplifica simplificar a equação eliminando quantidades iguais de ambos os lados (como tirar o mesmo peso dos dois pratos da balança) ou agrupar termos semelhantes.

$$x^2= 25$$
$$5^2= 25$$
$$x= 5$$

### 💡Dica
Expressões algébricas e equações não são sinônimos. Equação é a técnica de igualar duas expressões algébricas.
- **Expressão algébrica**
$$2+x-5$$
- **Equação (isolar o $x$)**: igualando o resultado (técnica do balanço) do lado esquerdo e do lado direito, eu defino um valor fixo de $x$.
$$x=5-2$$
$$x=3$$
### O real problema
As equações surgiram da necessidade prática de resolver problemas que envolviam quantidades desconhecidas, como transações comerciais, divisões de herança e medições de terras.

Elas eram uma ferramenta para:
- Calcular o preço de uma mercadoria individual quando se sabia apenas o valor total de um lote.
- Determinar as dimensões de um terreno (como o comprimento de um muro) para que ele tivesse uma área específica.
- Calcular heranças, para dividir bens entre vários herdeiros

### A junção da álgebra com a geometria

Ver [Mathematics/geometria.md](/Mathematics/geometria.md)

### O que significa "Grau"?
Antes de existirem os símbolos que usamos hoje, os matemáticos usavam palavras como "*a coisa*" (em árabe *shay*, que deu origem ao nosso $x$) para representar o valor desconhecido.

O termo "grau" refere-se ao expoente do "*coisa*" ou "$x$" (incógnita). Se a incógnita tiver o expoente 1, a equação é considerada de 1º grau, se a incógnita tiver o expoente 2, a equação é considerada de 2º grau, e assim sucessivamente.

Historicamente, as de 2º grau eram essenciais para problemas de geometria, enquanto as de 1º grau resolviam questões de proporção e contabilidade.

O fato de chamarmos de equação linear ou espacial, vem mais tarde quando colocamos as equações dentro de uma plano cartesiano, que daí chamaremos de função.

### A forma geral de uma equação linear com uma incógnita é definida por:

$$ax + b = 0$$

Onde:
* **$x$**: é a incógnita (o valor que buscamos encontrar).
* **$a$**: é o coeficiente angular (deve ser $\neq 0$).
* **$b$**: é o termo constante (ou coeficiente linear).

### A forma geral de uma equação de segundo grau é definida por:

$$ax^2 + bx + c = 0$$

Onde:
* **$x$**: é a incógnita.
* **$a, b, c$**: são coeficientes reais, com a condição obrigatória de $a \neq 0$.

---

#### A técnica de Completar quadrados

![Completar Quadrados](/assets/completar-quadrado.png)

O método de completar quadrados transforma uma equação quadrática comum em uma identidade baseada no **Trinômio Quadrado Perfeito**: 

$$(x + k)^2 = x^2 + 2kx + k^2$$

---

##### 🧮 Dedução e Passo a Passo Geral

Partindo da forma geral $ax^2 + bx + c = 0$ (considerando $a = 1$ para simplificar a demonstração, ou seja, $x^2 + bx + c = 0$):

$$\begin{aligned}
x^2 + bx + c &= 0 \\
x^2 + bx &= -c \quad \text{(Isola o termo constante)} \\
\\
\text{Adiciona } \left(\frac{b}{2}\right)^2 \text{ em ambos os lados:} \\
x^2 + bx + \left(\frac{b}{2}\right)^2 &= -c + \left(\frac{b}{2}\right)^2 \\
\\
\text{Fatora o lado esquerdo:} \\
\left(x + \frac{b}{2}\right)^2 &= \frac{b^2}{4} - c \\
\\
\text{Aplica a raiz quadrada:} \\
x + \frac{b}{2} &= \pm\sqrt{\frac{b^2 - 4c}{4}} \\
\\
x &= -\frac{b}{2} \pm \frac{\sqrt{b^2 - 4c}}{2}
\end{aligned}$$

---

##### 📝 Exemplo prático resolvido

Na época de Al-Khwarizmi, resolver uma equação do 2º grau era, literalmente, completar um quadrado desenhado no chão ou no papiro.

**O problema da Herança**

Imagine que um pai deixou um terreno quadrado para o seu filho. No testamento diz:

> "O terreno original é um quadrado, mas você deve adicionar uma faixa retangular de $6m$ de largura ao lado dele. A área total final (o quadrado original mais a faixa) deve ser de $16m^2$

Qual é o tamanho do lado do terreno original?

- **Montando a equação**
1. Área do quadrado original: $x \cdot x = x^2$ (Termo principal)
2. Área da faixa adicionada: $6 \cdot x = 6x$ (Termo secundário)
3. Área total desejada: 16

Equação: $x^2 + 6x = 16$

$$\begin{aligned}
x^2 + 6x = 16 \\
\text{Somamos 9 em ambos os lados:} \\
x^2 + 6x \blue{+ 9} &= 16 \blue{+ 9} \\
\text{Fatorando o trinômio perfeito:} \\
(x + 3)^2 &= 25 \\
\text{Extraindo a raiz quadrada:} \\
x + 3 &= \pm\sqrt{25} \\
x + 3 &= \pm 5 \\
\text{Separando as soluções:} \\
x_1 &= + 5 - 3 = 2 \\
x_2 &= - 5 - 3 = -8 \\
\end{aligned}$$

**Conjunto Solução:** $S = \{1, 5\}$

#### 🧮 A técnica de Bhaskara

A resolução é dividida em duas etapas principais: o cálculo do discriminante ($\Delta$) e a determinação das raízes.

##### 1. Cálculo do Discriminante ($\Delta$)
$$\Delta = b^2 - 4ac$$

> 💡 **Análise do $\Delta$:**
> * Se $\Delta > 0$: A equação possui **duas raízes reais e distintas** ($x_1 \neq x_2$).
> * Se $\Delta = 0$: A equação possui **duas raízes reais e iguais** ($x_1 = x_2$).
> * Se $\Delta < 0$: A equação **não possui raízes reais** (raízes complexas).

##### 2. Determinação das Raízes ($x$)
$$x = \frac{-b \pm \sqrt{\Delta}}{2a}$$

---

##### 📝 Exemplo Prático Resolvido
Resolva a equação $x^2 - 5x + 6 = 0$:

$$\begin{aligned}
\text{Identificando os coeficientes:} \quad & a = 1, \ b = -5, \ c = 6 \\
\\
\text{Calculando o } \Delta: \quad & \Delta = (-5)^2 - 4 \cdot 1 \cdot 6 \\
& \Delta = 25 - 24 \\
& \Delta = 1 \\
\\
\text{Calculando as raízes } (x): \quad & x = \frac{-(-5) \pm \sqrt{1}}{2 \cdot 1} \\
& x = \frac{5 \pm 1}{2} \\
\\
x_1 = \frac{5 + 1}{2} = 3 & \quad \text{e} \quad x_2 = \frac{5 - 1}{2} = 2
\end{aligned}$$

**Conjunto Solução:** $S = \{2, 3\}$

#### Curiosidades
A palavra **algoritmo** vem da latinização do nome de **Abdallah Muhammad ibn Musa al-Khwarizmi. Com o tempo o termo passou por alterações (influenciado pelo grego *arithmos*, que significa número) até se tornar "algoritmo"

A palavra **fórmula** vem do latim *formula* que é o diminutivo de *forma*. Originalmente significa "pequena forma", "molde" ou "modelo". O termo era usado na antiguidade para designar uma regra, um padrão ou método estabelecido para resolver problemas ou padronizar prodecimentos.

Toda *fórmula* matemática pode ser considerada um *algoritmo*, mas nem todo algoritmo é uma fórmula.

Características | Fórmula | Algoritmo
-|-|-
Definição | relação matemática expressa em símbolos | sequência de instruções lógicas (passo-a-passo) 
Foco | resultado | como chegar ao resultado (processo)
Estrutura | equação (expressão expressa em símbolos) | fluxo dinâmico com condições, decisões e repetições
Contexto | Matemática pura, Física, Química e Estatística descritiva | Programação, Contas matemáticas

- **A fórmula expressa uma lei universal e estática**: Ela condensa uma verdade matemática pura em uma única linha. Ela não diz ao seu cérebro ou ao computador como fazer a conta, ela apenas diz qual é a proporção exata que rege aquele fenômeno. Por exemplo, a fórmula da área do Círculo ($A = \pi \cdot r^2$) apenas aponta os elementos necessários.

- **O algoritmo resolve processos complexos e dinâmicos**: Computadores e sistemas de automação não conseguem "advinhar" regras estáticas; eles precisam de um roteiro operacional de ações ordenadas no tempo. Um algoritmo lida com tomada de decisões e repetições de tarefas até que uma condição seja atingida, algo que a fórmula matemática simples não consegue expressar de forma isolada.

## $f(x)$ Funções

No séc XVII e XVIII, com a invenção dos telescópios e dos canhões, Isaac Newton e Leibniz precisavam calcular a velocidade das coisas que mudavam a cada milissegundo (planetas orbitando ou balas de canhão voando)

Eles usaram a Geometria Analítica de Descartes para criar o conceito de **Função**. O gráfico mostrava uma linha que representava o tempo ($x$) mudando o espaço ($y$). A função virou a linguagem oficial da física.


Enquanto a equação é uma pergunda estática (Ex: Qual o lado do quadrado para a área ser 16?), a função é uma relação dinâmica.

- **Na equação**: $x^2+6x=16$ Você quer achar o $x$ específico.
- **Na função**: $f(x)=x^2+6x$ Aqui você quer ver o que acontece com a área se você mudar o valor de $x$ livremente.

### O gráfico
- A **Equação** de 2º grau é apenas o momento exato em que a curva cruza a linha do zero (o "chão")
- A **Função** mostra o movimento completo da curva subindo e descendo.

As funções são consideradas ferramentas que "preveem o futuro" porque permitem criar **modelos matemáticos** para descrever o comportamento de situações reais ao longo do tempo.

Um **modelo** é uma representação simplificada da realidade. A função é o "**molde**". Quando você coloca um dado nela (o valor de $x$), ela devolve o que vai acontecer (o valor de $y$).

Quando você descobre a "lei de formação" a (**fórmula**) de uma função, você pode projetar resultados que ainda não aconteceram. Por exemplo:

- **Na Física**: Se você sabe a velocidade de um carro, consegue calcular exatamente onde ele estará daqui a 2 horas.
- **Na Economia**: Se uma empresa sabe como suas vendas crescem mensalmente, ela usa funções para prever o lucro do próximo ano ou quando atingirá uma meta.
- **No cotidiano**: Ao saber o preço fixo da bandeirada de um táxi e o valor por quilômetro, você "prevê" o custo total da viagem antes mesmo de entrar no carro.

Dizer que funções "preveem o futuro" é uma forma de explicar que elas permitem **antecipar resultados** sem precisar esperar que algo aconteça.

Na matemática chamamos isso de **projeção** ou **predição**.

**Pense assim**: Uma função cria um **padrão**. Se você descobre o padrão, você domina o que vem depois.

A sequência **álgebra → funções** existe para que o aluno primeiro entenda como manipular letras e números e, só então, veja como isso se transforma em um desenho no plano cartesiano. É a unição da conta com o visual.


### O trauma do f(x)

O $f(x) = ax + b$. é uma representação algébrica.

Uma função é apenas uma máquina de processar dados. Alguém percebeu uma regra no mundo real e quis automatizá-la para não ter que fazer a conta toda vez.

- **Exemplo 1**"Taxi"

"Imagine que você é o dono de uma frota de táxis em 1920. Você precisa cobrar os clientes de forma justa.

Você decide: todo mundo paga R$ $5,00$ fixos só de entrar no carro (bandeirada) mais R$ $2,00$ por quilômetro rodado.
- Se o cliente roda $1 km \rightarrow 5 + 2\cdot(1) = 7$
- Se o cliente roda $5 km \rightarrow 5 + 2\cdot(5) = 15$
- Se o cliente roda $x km \rightarrow 5 + 2\cdot(x)$

### Função Afim (Progressão Aritmética)

### Função Exponencial (Progressão Geométrica)


