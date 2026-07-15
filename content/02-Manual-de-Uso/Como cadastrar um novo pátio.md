---
tags: [traflog, manual, patios]
---

⬆️ Voltar para [[TRAFLOG - Índice]] | [[Início]]

# Como cadastrar um novo pátio

> [!info] Objetivo
> Cadastrar um pátio completo: dados gerais, endereço, ruas e quadras.

> [!note] Referências de campos
> Este manual assume que você já sabe **o que** cada campo faz. Para o detalhamento de cada um, consulte:
> [[Pátios - Novo Pátio]] · [[Ruas]] · [[Quadras]]

## Passo a passo

### 1. Acessar a listagem de pátios

Menu **Cadastros → Pátios**. Você verá a tabela descrita em [[Pátios - Listagem]].

### 2. Iniciar um novo pátio

Clique no botão **Novo** (canto superior direito). Você será direcionado ao formulário [[Pátios - Novo Pátio]].

![[patios-novo-patio-formulario.png]]

### 3. Preencher os dados gerais e o endereço

Preencha: Descrição, Hora início, Hora fim, Duração atendimento, Cap. atend. simultâneo, e os campos de endereço (CEP, Endereço, Bairro, N°, Cidade, Complemento).

> [!tip] Dica
> A **Duração atendimento** e a **Cap. atend. simultâneo** definem o tamanho e a quantidade de blocos disponíveis no calendário de [[Agendamento - Tela]], defina com cuidado.

### 4. Cadastrar as ruas

Na seção **Ruas**, clique em **Novo** para adicionar uma rua. Preencha **Código** e **Descrição** da rua (ver [[Ruas]]).

Repita para quantas ruas o pátio tiver.

### 5. Cadastrar as quadras de cada rua

Dentro de cada rua expandida, na seção **Quadras**, clique em **Novo** para cada quadra e preencha:

- Código, Descrição
- Qtd. Fila Esq. / Posições Esq. / Níveis Esq.
- Qtd. Fila Dir. / Posições Dir. / Níveis Dir.

Consulte [[Quadras]] para o significado de cada quantidade, e [[YMS/Quadras/Representação matemática das quadras]] se quiser entender a lógica de capacidade antes de definir os números.

![[patios-quadras-tabela-preenchida.png]]

### 6. Salvar

Clique em **Inserir** no rodapé da tela. O pátio, com todas as ruas e quadras, será criado.

### 7. Conferir o resultado

Volte para [[Pátios - Listagem]] e confirme que o pátio aparece na tabela.

![[patios-listagem-preenchida.png]]

Opcionalmente, use o ícone de mapa (🗺️) na linha do pátio para conferir visualmente a estrutura criada, veja [[Como consultar o mapa do pátio]].

## Erros comuns

> [!warning] Cambos obrigatorios
> Como detalhando anteriormente em [[Pátios - Novo Pátio]], alguns campos são obrigatorios, e se não forem preenchidos, não conseguirar criar o pátio.
>

## Próximos passos

- [[Como cadastrar tipos de container e lacre]] — necessário antes de operar o pátio no dia a dia
- [[Como fazer um agendamento]]
