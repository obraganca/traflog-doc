---
tags: [traflog, patios, referencia]
---
 
⬆️ Voltar para [[Pátios]] | [[TRAFLOG - Índice]]

# Mapa do Pátio

Visualização gráfica das quadras de um pátio. Acessada pelo ícone de mapa (🗺️) na linha de um pátio em [[Pátios - Listagem]], ou pelo botão de mapa ao lado do campo Pátio em [[Agendamento - Tela]].

## Visão geral do mapa

Mostra cada quadra do pátio como um bloco identificado pelo seu **código** (ex: "1"). O título da tela mostra "Mapa - {nome do pátio}".

![[patios-mapa-visao-geral.png]]

## Detalhe de uma quadra

Ao clicar em um bloco de quadra, abre-se um painel de detalhe mostrando a estrutura completa configurada em [[Quadras]]:

- **Lado Esquerdo** e **Lado Direito**, cada um exibido como seção própria (a seção do lado só aparece se houver filas cadastradas para aquele lado)
- Dentro de cada lado, uma caixa por **Fila** (Fila 1, Fila 2, Fila 3...)
- Dentro de cada fila, uma grade de células: colunas = **Posições** (P1, P2, P3...), linhas = **Níveis** (empilhamento)
- Se a quantidade de filas/posições ultrapassar a largura da tela, surge uma **barra de rolagem horizontal** para navegar entre as filas
- Painel **Aguardando** à direita: área lateral fixa, reservada a containers aguardando alocação naquela quadra #pendente confirmar quando/como um container aparece aqui (ex: containers que chegaram mas ainda não foram alocados em uma posição específica?)

![[patios-mapa-quadra-detalhe.png]]

### Endereço de cada célula

Cada célula (posição+nível) tem um **código de endereço** próprio, no formato:

```
{Lado}{Fila}{Posição}{Nível}
```

Exemplo: **EF1P1N5** = Lado **E**squerdo, **F**ila 1, **P**osição 1, **N**ível 5.

> [!info] Isso é a aplicação prática do modelo formal
> Esse código é exatamente a tupla de endereço $(s, f, p, n)$ descrita em [[Representação matemática das quadras]] — o sistema apenas a exibe de forma compacta.

### Menu de ações da célula

Ao clicar em uma célula, abre-se um menu de contexto com três ações:

| Ação | Ícone | Função |
|---|---|---|
| **Alocar container** | + | Aloca um container naquela posição/nível específico |
| **Remover Container** | − | Remove o container atualmente alocado naquela célula |
| **Detalhes** | 🔍 | Consulta os detalhes do container alocado naquela célula #pendente confirmar quais informações aparecem (número do container, tipo, lacre, data de entrada, empresa, etc.) |

### Células ocupadas

- Células **ocupadas** exibem o **número do container** (ex: `MRKU1234567`) escrito dentro do bloco, no lugar do preenchimento cinza padrão.
- A célula selecionada/em foco fica destacada em **azul**.
- Células **vazias** permanecem no preenchimento cinza padrão (listrado), sem texto.

### Mover um container (drag and drop)

É possível **arrastar um container de uma célula para outra**, movendo-o de posição/nível dentro da mesma quadra (ou possivelmente entre quadras — #pendente confirmar se o drag funciona entre filas/quadras diferentes ou só dentro da mesma fila).

> [!warning] Pendente #pendente
> - O drag and drop tem alguma validação (ex: impedir mover para uma célula já ocupada, ou empilhar sem ter nível abaixo preenchido)?
> - O que aparece na tela **Detalhes** do container?
> - Qual a lógica/regra exata da área **Aguardando** (o que faz um container aparecer/sair dali)?

![[patios-mapa-celula-acoes-container.png]]

> [!note] Relação com o cadastro
> A quantidade de filas, posições e níveis exibida aqui é exatamente a configurada nos campos Qtd. Fila Esq./Dir., Qtd. Posições Fila Esq./Dir. e Qtd. Níveis Fila Esq./Dir. em [[Quadras]]. Ver também [[Representação matemática das quadras]] para a lógica de endereçamento (lado, fila, posição, nível).

## Relacionado

- [[Quadras]]
- [[Pátios - Listagem]]
- [[Agendamento - Tela]]
