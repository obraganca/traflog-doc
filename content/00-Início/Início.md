---
tags: [traflog, início, overview]
---

# TRAFLOG (YMS) — Início

> [!info] Sobre o TRAFLOG
> TRAFLOG é um sistema de tecnologia para **gestão de transporte**, com visão corporativa, operacional e fiscal. Este vault documenta o módulo de **YMS (Yard Management System)** — gestão de pátios, quadras e agendamento de containers.

---

## Como esta documentação está organizada

A documentação é dividida em **duas camadas**, para servir a dois propósitos diferentes:

```
00-Início/                          → você está aqui
01-Referencia-Funcionalidades/      → o que cada tela/campo/botão FAZ
   Patios/
   Cadastros-Auxiliares/
   Agendamento/
02-Manual-de-Uso/                   → COMO usar o sistema, passo a passo
03-Conceitos/                       → fundamentos teóricos (ex: modelo matemático das quadras)
Anexos/                             → prints de tela usados nas notas
```

> [!tip] Por que separar Referência de Manual?
> - **Referência de Funcionalidades**: é a "planta baixa" do sistema. Cada nota descreve uma tela, seus campos, botões e regras — sem se preocupar com o "fluxo" de uso. É o material que você consulta quando quer saber "o que faz esse campo?".
> - **Manual de Uso**: é orientado a **tarefas** ("Como cadastro um pátio novo?"). Cada manual é um passo a passo que **linka** para as notas de referência correspondentes, evitando duplicar conteúdo.

---

## Por onde começar

| Se você quer... | Vá para |
|---|---|
| Entender o que existe em cada tela, campo a campo | [[01-Referencia-Funcionalidades]] (ou o índice geral abaixo) |
| Aprender a executar uma tarefa (cadastrar, agendar etc.) | [[02-Manual-de-Uso]] |
| Entender o modelo lógico/matemático por trás das quadras | [[YMS/Quadras/Representação matemática das quadras]] |
| Ver o mapa geral do sistema | [[TRAFLOG - Índice]] |

---

## Módulos documentados

- 🏗️ **Pátios** — cadastro de pátios, ruas e quadras; visualização em mapa
- 🧰 **Cadastros Auxiliares** — tipos de container, tipos de lacre
- 📅 **Agendamento** — reserva de horários para alocação de containers

## Glossário rápido

| Termo | Significado |
|---|---|
| **Pátio** | Local físico onde os containers ficam armazenados |
| **Rua** | Subdivisão do pátio; agrupa uma ou mais quadras |
| **Quadra** | Porção de terra dentro de uma rua, dividida em Lado Esquerdo/Direito, Filas, Posições e Níveis |
| **Fila** | Subdivisão de um lado da quadra (ex: Fila 1, Fila 2) |
| **Posição** | "Coluna" dentro de uma fila (ex: P1, P2, P3) |
| **Nível** | Altura de empilhamento dentro de uma posição |
| **TOS/YMS** | Sistema de gerenciamento de pátio/terminal (o próprio TRAFLOG, neste contexto) |

> [!warning] Pendente #pendente
> Confirmar se existem **perfis de usuário** distintos (admin, operador de pátio, motorista/transportadora agendando) e se as permissões variam entre eles. Ainda não documentado.

---

## Legenda de status usada nas tabelas

- 🟢 Completo
- 🟡 Em construção / parcialmente documentado
- 🔴 Não iniciado
- `#pendente` — trecho que precisa de confirmação ou complemento seu
