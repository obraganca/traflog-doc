---
tags: [traflog, patios, referencia]
---

⬆️ Voltar para [[Pátios]] | [[TRAFLOG - Índice]]

# Pátios — Novo Pátio

Formulário de criação (e edição) de um pátio. Acessado pelo botão **Novo** em [[Pátios - Listagem]].

## Campos

| Campo                  | Descrição                                                                             | Obrigatório | Padrão   |
| ---------------------- | ------------------------------------------------------------------------------------- | ----------- | -------- |
| Descrição              | Nome do pátio                                                                         | Sim         | —        |
| Hora início            | Horário de início do funcionamento                                                    | Sim         | 06:00    |
| Hora fim               | Horário de fim do funcionamento                                                       | Sim         | 18:00    |
| Duração atendimento    | Duração de cada janela de atendimento (usada no calendário de [[Agendamento - Tela]]) | Sim         | 00:30:00 |
| Cap. atend. simultâneo | Quantidade de atendimentos simultâneos permitidos por janela de horário               | Sim         | 1        |
| CEP                    | CEP do endereço                                                                       | Sim         | —        |
| Endereço               | Logradouro                                                                            | Sim         | —        |
| Bairro                 | Bairro                                                                                | Sim         | —        |
| N°                     | Número                                                                                | Sim         | —        |
| Cidade                 | Cidade (campo de seleção/busca)                                                       | Sim         | —        |
| Complemento            | Complemento do endereço                                                               | Não         | —        |


## Seção Ruas

Abaixo dos dados do pátio, há a seção **Ruas**, onde se cadastra uma ou mais ruas que compõem o pátio.

- Botão **Novo** cria uma nova rua ("Nova Rua"), que pode ser expandida/recolhida (seta ▾).
- Cada rua possui um **X** vermelho para remoção.
- Dentro de cada rua, ver [[Ruas]] para os campos e a seção **Quadras**.

## Botão de ação

| Botão | Função |
|---|---|
| **Inserir** (rodapé, verde) | Salva o pátio e todas as ruas/quadras cadastradas |

## Prints

**Formulário vazio:**
![[patios-novo-patio-formulario.png]]

**Formulário com seção campos obrigatorios:**
![[patios-novo-obrigatorio-vazio.png]]

**Formulário com seção campos obrigatorios:**
![[patios-novo-patio-rua-quadras-vazio.png]]
## Relacionado

- [[Ruas]]
- [[Quadras]]
- [[Pátios - Listagem]]
