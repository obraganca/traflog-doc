---
tags: [traflog, patios, referencia]
---

⬆️ Voltar para [[Pátios]] | [[TRAFLOG - Índice]] | Parte de [[Ruas]]

# Quadras

Sub-componente de [[Ruas]]. Representa as porções de terra dentro de uma rua, onde os containers são efetivamente armazenados.

> [!info] Modelo matemático
> Para o detalhamento formal (fila × posição × nível, capacidade, endereçamento), veja [[YMS/Quadras/Representação matemática das quadras]].

## Campos ao criar/editar uma quadra

| Campo | Descrição |
|---|---|
| Código | Código identificador da quadra |
| Descrição | Nome/descrição da quadra |
| Qtd. Fila Esq. | Quantidade de filas no **lado esquerdo** |
| Qtd. Posições Fila Esq. | Quantidade de posições por fila, lado esquerdo |
| Qtd. Níveis Fila Esq. | Quantidade de níveis (altura de empilhamento) por fila, lado esquerdo |
| Qtd. Fila Dir. | Quantidade de filas no **lado direito** |
| Qtd. Posições Fila Dir. | Quantidade de posições por fila, lado direito |
| Qtd. Níveis Fila Dir. | Quantidade de níveis por fila, lado direito |

Esses 6 valores (3 para cada lado) definem completamente a geometria da quadra — ver [[YMS/Quadras/Representação matemática das quadras]] para a fórmula de capacidade.

## Tabela de quadras (dentro da rua)

| Coluna | Observação |
|---|---|
| Código | Editável inline |
| Descrição | Editável inline |
| Qtd. Fila E... / Qtd. Posições Fila Esq. / Qtd. Níveis Fila Esq. | Valores numéricos, padrão `0` |
| Qtd. Fila Dir. / Qtd. Posições Fila Dir. / Qtd. Níveis Fila Dir. | Valores numéricos, padrão `0` |
| Ações | ❌ remove a linha |

Rodapé da tabela mostra **Linhas** e **Total de Linhas**.

## Ações

| Botão | Função |
|---|---|
| **Novo** (seção Quadras) | Adiciona uma nova linha de quadra (valores começam zerados, "Sem linhas para mostrar" quando vazia) |
| ❌ por linha | Remove aquela quadra |

## Prints

**Seção vazia:**
![[patios-novo-patio-rua-quadras-vazio.png]]

**Com quadras adicionadas:**
![[patios-quadras-tabela-preenchida.png]]

> [!warning] Pendente #pendente
> Confirmar se há validação mínima (ex: não permitir salvar com todas as quantidades zeradas) e se os campos "Fila E..." truncados na tabela têm tooltip com o nome completo.

## Relacionado

- [[YMS/Quadras/Representação matemática das quadras]]
- [[Mapa do Pátio]] — é onde a geometria definida aqui é exibida visualmente
- [[Ruas]]
