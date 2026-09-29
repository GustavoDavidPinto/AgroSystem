# AgroGestor

**Sistema de Gestão de Insumos e Safras para Produtores Rurais**

---

## 1. Problema Identificado

Pequenos e médios produtores agrícolas enfrentam grandes dificuldades para controlar o estoque de insumos (sementes, fertilizantes e defensivos), registrar as aplicações realizadas nas lavouras e acompanhar o desenvolvimento das safras.

Atualmente, a maioria desses produtores utiliza cadernos de papel, anotações soltas ou planilhas desorganizadas. Isso gera:

- Perda de informações importantes
- Dificuldade de saber o que já foi aplicado e quando
- Risco de sobreaplicação ou subaplicação de produtos
- Falta de histórico confiável para tomada de decisão
- Dificuldade de comprovar rastreabilidade da produção
- Desperdício de insumos e aumento de custos

**Quem enfrenta o problema?**  
Pequenos e médios produtores rurais, técnicos agrícolas e gestores de propriedades.

**Como é resolvido atualmente?**  
Cadernos manuais, anotações em papel e planilhas do Excel (quando existem).

**Principais dificuldades do processo atual:**  
Falta de padronização, risco de perda de dados, dificuldade de consulta rápida e ausência de alertas ou histórico organizado.

---

## 2. Proposta da Solução

### Nome do sistema
**AgroGestor**

### Descrição
O AgroGestor é uma plataforma web (com possibilidade de uso via celular) desenvolvida para ajudar produtores rurais a gerenciar de forma simples e organizada o estoque de insumos, o registro de aplicações nas lavouras e o acompanhamento das safras. O sistema permite cadastrar propriedades, talhões, culturas, insumos e registrar todas as atividades realizadas no campo, gerando histórico e relatórios úteis para a tomada de decisão.

### Objetivo geral
Facilitar o controle e a organização das atividades agrícolas, reduzindo perdas, melhorando o uso de insumos e aumentando a eficiência da propriedade rural.

### Público-alvo
- Pequenos e médios produtores rurais
- Técnicos agrícolas
- Gestores de propriedades rurais
- Cooperativas e assistentes técnicos

### Principais benefícios esperados
- Redução de desperdício de insumos
- Histórico organizado das aplicações e atividades
- Melhor planejamento das safras
- Facilidade de consulta e geração de relatórios
- Apoio à rastreabilidade da produção
- Maior controle e profissionalização da gestão da propriedade

---

## 3. Técnica de Levantamento de Requisitos

**Técnica escolhida:** Entrevista semiestruturada + Análise de documentos

**Justificativa:**  
A entrevista permite compreender diretamente as dores e a rotina real dos produtores. A análise dos cadernos e planilhas atuais ajuda a identificar quais informações já são registradas e quais faltam.

**Como seria aplicada:**
- Entrevistas individuais com 4 a 6 produtores rurais de diferentes portes
- Análise dos cadernos de campo e planilhas utilizadas atualmente
- Observação da rotina de registro de aplicações (quando possível)

**Principais informações a serem obtidas:**
- Quais dados eles registram hoje
- Quais informações mais sentem falta
- Como fazem o controle de estoque atualmente
- Quais dificuldades mais prejudicam o dia a dia
- Quais funcionalidades consideram prioritárias

**Instrumento utilizado (Roteiro de Entrevista):**

1. Como você controla atualmente o estoque de insumos da propriedade?
2. Você registra as aplicações de fertilizantes e defensivos? De que forma?
3. Quais informações você mais precisa consultar no dia a dia?
4. Já aconteceu de perder informação importante por causa do controle manual?
5. Quais seriam as três funcionalidades mais importantes em um sistema digital para você?
6. Você utilizaria o sistema pelo celular no campo?

---

## 4. Requisitos

### Requisitos Funcionais

| ID    | Descrição                                                                 |
|-------|---------------------------------------------------------------------------|
| RF01  | O sistema deverá permitir o cadastro de propriedades rurais               |
| RF02  | O sistema deverá permitir o cadastro de talhões/áreas da propriedade      |
| RF03  | O sistema deverá permitir o cadastro de culturas e safras                 |
| RF04  | O sistema deverá permitir o cadastro de insumos (sementes, fertilizantes e defensivos) |
| RF05  | O sistema deverá controlar a entrada e saída de insumos do estoque        |
| RF06  | O sistema deverá permitir o registro de aplicações de insumos nas lavouras |
| RF07  | O sistema deverá permitir o registro de atividades agrícolas (plantio, colheita, etc.) |
| RF08  | O sistema deverá gerar histórico de aplicações por talhão e por cultura   |
| RF09  | O sistema deverá emitir alertas de estoque baixo                          |
| RF10  | O sistema deverá gerar relatórios simples de consumo de insumos e atividades |

### Requisitos Não Funcionais

| ID     | Descrição                                                                 |
|--------|---------------------------------------------------------------------------|
| RNF01  | O sistema deverá ser responsivo e utilizável em smartphones               |
| RNF02  | O sistema deverá ter interface simples e intuitiva, adequada para usuários com baixa familiaridade tecnológica |
| RNF03  | O sistema deverá garantir a segurança e privacidade dos dados da propriedade |
| RNF04  | O sistema deverá estar disponível 24 horas por dia (alta disponibilidade) |
| RNF05  | O tempo de resposta das principais telas não deverá ultrapassar 3 segundos |

---

## 5. Usuários e Funcionalidades

### 1. Produtor Rural / Proprietário
- **Necessidade:** Controlar insumos, registrar atividades e acompanhar as safras de forma organizada.
- **Principais ações:** Cadastrar propriedade e talhões, registrar entradas/saídas de estoque, registrar aplicações, consultar histórico e relatórios.

### 2. Técnico Agrícola / Assistente
- **Necessidade:** Acompanhar as atividades da propriedade e orientar o produtor com base em dados reais.
- **Principais ações:** Visualizar registros, cadastrar aplicações, gerar relatórios e acompanhar o histórico das safras.

### 3. Administrador do Sistema
- **Necessidade:** Gerenciar usuários e manter o sistema funcionando.
- **Principais ações:** Gerenciar usuários, permissões e configurações gerais.

---

## 6. Histórias de Usuário

### US01 – Cadastrar propriedade
**Como** produtor rural,  
**quero** cadastrar minha propriedade e seus talhões  
**para** organizar as informações da minha área de produção.

**Critérios de aceitação:**
- Deve ser possível informar nome, localização e tamanho da propriedade
- Deve ser possível cadastrar vários talhões vinculados à propriedade
- Os dados devem ser salvos e listados corretamente

### US02 – Controlar estoque de insumos
**Como** produtor rural,  
**quero** registrar entradas e saídas de insumos  
**para** saber exatamente o que tenho disponível na propriedade.

**Critérios de aceitação:**
- Deve permitir cadastrar o insumo (nome, tipo, unidade de medida)
- Deve registrar quantidade de entrada e saída
- O saldo atual deve ser atualizado automaticamente
- Deve alertar quando o estoque estiver baixo

### US03 – Registrar aplicação de insumos
**Como** produtor rural,  
**quero** registrar as aplicações de fertilizantes e defensivos  
**para** manter o histórico correto do que foi aplicado em cada talhão.

**Critérios de aceitação:**
- Deve permitir selecionar o talhão e a cultura
- Deve permitir informar o insumo, dose e data da aplicação
- A quantidade utilizada deve ser descontada do estoque
- O registro deve aparecer no histórico do talhão

### US04 – Registrar atividades da safra
**Como** produtor rural,  
**quero** registrar as principais atividades (plantio, tratos culturais, colheita)  
**para** ter um histórico completo da safra.

**Critérios de aceitação:**
- Deve permitir selecionar o tipo de atividade
- Deve vincular a atividade ao talhão e à cultura
- Deve permitir informar data e observações
- As atividades devem ser listadas em ordem cronológica

### US05 – Consultar histórico por talhão
**Como** produtor rural,  
**quero** consultar todo o histórico de um talhão  
**para** tomar decisões com base no que já foi feito.

**Critérios de aceitação:**
- Deve listar todas as aplicações e atividades do talhão
- Deve permitir filtrar por período e por tipo de registro
- As informações devem estar claras e organizadas

### US06 – Gerar relatório simples
**Como** produtor rural,  
**quero** gerar relatórios de consumo de insumos e atividades  
**para** analisar o desempenho da safra e os custos.

**Critérios de aceitação:**
- Deve permitir escolher o período e o talhão/cultura
- Deve apresentar os dados de forma clara (tabela ou resumo)
- Deve ser possível visualizar ou exportar o relatório

### US07 – Receber alerta de estoque baixo
**Como** produtor rural,  
**quero** ser alertado quando um insumo estiver acabando  
**para** conseguir repor o estoque a tempo.

**Critérios de aceitação:**
- O sistema deve permitir definir a quantidade mínima de cada insumo
- Quando o saldo ficar abaixo do mínimo, deve gerar um alerta
- O alerta deve ser visível na tela principal

---

## 7. Priorização e MVP

### Prioridade Alta (MVP)
- Cadastro de propriedade e talhões
- Cadastro e controle de estoque de insumos
- Registro de aplicações de insumos
- Consulta de histórico por talhão
- Alerta de estoque baixo

### Prioridade Média
- Registro de outras atividades da safra (plantio, colheita etc.)
- Geração de relatórios simples
- Cadastro de múltiplas culturas/safras

### Prioridade Baixa
- Exportação de relatórios em PDF
- Dashboard com indicadores avançados
- Integração com previsões climáticas
- Aplicativo mobile nativo

### Definição do MVP
O MVP do AgroGestor será composto pelas funcionalidades de prioridade **Alta**, permitindo que o produtor já consiga controlar o estoque de insumos, registrar as aplicações e consultar o histórico de forma organizada.

---

## 8. Organização do Projeto (GitHub)

- **Repositório:** AgroGestor
- **Quadro (GitHub Project):** Backlog → A Fazer → Em Andamento → Em Revisão → Concluído
- As User Stories foram cadastradas como Issues e organizadas no quadro conforme a prioridade.

---

## 9. Planejamento da Primeira Sprint

**Objetivo da Sprint:**  
Entregar a base do sistema com cadastro de propriedade, talhões e controle inicial de estoque de insumos.

**Funcionalidades selecionadas:**
- Cadastro de propriedade e talhões (US01)
- Cadastro de insumos e controle de estoque (US02)
- Tela inicial com visão geral do estoque

**Issues da Sprint:**
- Issue #1 – Cadastro de propriedade
- Issue #2 – Cadastro de talhões
- Issue #3 – Cadastro de insumos
- Issue #4 – Registro de entrada e saída de estoque
- Issue #5 – Listagem de estoque atual

**Resultado esperado ao final da Sprint:**  
O usuário consegue cadastrar sua propriedade, seus talhões e já controlar o estoque básico de insumos, visualizando o saldo atualizado.

---

## Como contribuir / Próximos passos

Este repositório representa a fase de concepção e organização inicial do projeto. O desenvolvimento do código será iniciado a partir da primeira Sprint.
