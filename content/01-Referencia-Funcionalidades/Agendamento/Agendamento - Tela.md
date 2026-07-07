---
tags: [traflog, agendamento, referencia]
---

⬆️ Voltar para [[TRAFLOG - Índice]] | Manual: [[Como fazer um agendamento]]

# Agendamento — Tela

Tela usada para reservar horários nos dias em que um container será alocado em um pátio.

## Campos de seleção

| Campo                               | Descrição                                                                     |
| ----------------------------------- | ----------------------------------------------------------------------------- |
| Empresa                             | Empresa utilizadora (dropdown)                                                |
| Pátio                               | Pátio requisitado (dropdown)                                                  |
| 🗺️ (botão ao lado de Pátio)        | Abre o [[Mapa do Pátio]] do pátio selecionado, para consulta antes de agendar |
| Semana → **Anterior** / **Próxima** | Navega entre semanas no calendário                                            |

## Calendário semanal

- Colunas: dias da semana (segunda a domingo), com a data por extenso no cabeçalho.
	- Linhas: horários em blocos (intervalo definido pelo campo **Duração atendimento** do pátio, ver [[Pátios - Novo Pátio]]), variando conforme a duração de atendimento configurada, no print, blocos de 30 min.
	- Os horários definidos na criação do [[Pátios - Novo Pátio]] são respeitados nessa seleção dos horários agendados, onde, não é possível selecionar horários fora do período permitido. 
- Dias/horários indisponíveis aparecem esmaecidos (cinza).
- Ao clicar em um bloco de horário disponível, ele fica **verde** (selecionado).
- Uma dica na tela indica: **"Selecione um horário por container"**, ou seja, apenas um container será manuseado naquele horário.

## Painel "Horários selecionados"

Localizado na parte inferior da tela:

- Lista, em formato de "chips", cada horário selecionado (data + hora)
- Cada chip tem um **X** para remover a seleção
- Botão **Confirmar horários** (canto inferior direito) efetiva as reservas

## Print

![[agendamento-tela-completa.png]]

> [!warning] Pendente #pendente
> - Descrever o que ocorre ao clicar em **Confirmar horários** (mensagem de sucesso, redirecionamento, etc.).

## Relacionado

- [[Pátios - Novo Pátio]]
- [[Mapa do Pátio]]
- [[Como fazer um agendamento]]
