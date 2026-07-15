---
tags: [traflog, patios, matematica, conceitos]
---

⬆️ Voltar para [[TRAFLOG - Índice]] | Relacionado: [[Quadras]] · [[Pátios]]

# Modelo matemático da quadra de um pátio de contêineres

> [!info] Contexto
> Esta nota formaliza matematicamente a estrutura de armazenagem de uma [[Quadras|Quadra]] dentro de um [[Pátios|Pátio]], usando **fila**, **posição** e **nível** como as três dimensões de endereçamento. Serve de base conceitual para os campos descritos em [[Quadras]] e para a visualização em [[Mapa do Pátio]].

---

## 1. Variáveis fundamentais

Para cada lado $s \in {E, D}$ (Esquerdo, Direito) de uma quadra, definimos três parâmetros inteiros positivos:

$$ F_s = \text{quantidade de filas} $$ $$ P_s = \text{quantidade de posições por fila} $$ $$ N_s = \text{quantidade de níveis por fila} $$

> [!example] Exemplo cadastrado $$F_E = 2,\quad P_E = 3,\quad N_E = 4$$ $$F_D = 3,\quad P_D = 2,\quad N_D = 1$$

---

## 2. A fila como matriz

Cada fila individual $f$, dentro do lado $s$, é uma **matriz** de slots de armazenagem:

$$ M_{s,f} \in {0,1}^{N_s \times P_s} $$

onde cada elemento $M_{s,f}[n,p]$ indica se o slot está ocupado ($1$) ou vazio ($0$):

$$ M_{s,f}[n,p] = \begin{cases} 1 & \text{se há contêiner no nível } n\text{, posição } p \ 0 & \text{caso contrário} \end{cases} $$

com $n \in {1, \dots, N_s}$ e $p \in {1, \dots, P_s}$.

---

## 3. O lado como tensor de ordem 3

O lado $s$ inteiro é a coleção de todas as suas filas — um **tensor de ordem 3** (rank-3):

$$ T_s \in {0,1}^{F_s \times N_s \times P_s} $$

$$ T_s[f, n, p] = M_{s,f}[n,p] $$

> [!note] Interpretação
> 
> - Eixo $f$ → **largura** (qual fila)
> - Eixo $n$ → **altura** (nível de empilhamento)
> - Eixo $p$ → **comprimento** (posição/baia)

---

## 4. A quadra como união dos dois tensores

A quadra completa $Q$ é a união dos tensores dos dois lados:

$$ Q = T_E \cup T_D $$

Como $T_E$ e $T_D$ podem ter dimensões diferentes ($F_E \neq F_D$, $N_E \neq N_D$, etc.), $Q$ **não é um único tensor retangular** — é um par de tensores independentes:

$$ Q = (T_E,\ T_D) $$

---

## 5. Endereço de um contêiner

O endereço de qualquer contêiner armazenado é a tupla:

$$ \text{end} = (s,\ f,\ p,\ n) $$

sujeito às restrições:

$$ s \in {E,D},\quad f \in [1, F_s],\quad p \in [1, P_s],\quad n \in [1, N_s] $$

Essa tupla é uma **bijeção** com um índice linear único no espaço de armazenagem — é o que o YMS (sistema de gerenciamento do pátio) usa internamente.

---

## 6. Capacidade da quadra

A capacidade de cada lado é o produto das três dimensões:

$$ \text{Cap}(s) = F_s \cdot P_s \cdot N_s $$

A capacidade total da quadra é a soma dos dois lados:

$$ \text{Cap}(Q) = \text{Cap}(E) + \text{Cap}(D) = \sum_{s \in {E,D}} F_s \cdot P_s \cdot N_s $$



---

## 7. Resumo em notação compacta

|Símbolo|Significado|
|---|---|
|$s$|lado (E ou D)|
|$f$|índice da fila|
|$p$|índice da posição|
|$n$|índice do nível|
|$F_s, P_s, N_s$|dimensões do lado $s$|
|$M_{s,f}$|matriz $N_s \times P_s$ de uma fila|
|$T_s$|tensor $F_s \times N_s \times P_s$ do lado|
|$Q$|par $(T_E, T_D)$ — a quadra completa|

---

## Ver também

- [[Pátios]]
- [[Quadras]]
- [[Mapa do Pátio]]