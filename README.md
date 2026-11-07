# ⚡ ANÁLISE DE DADOS DE ENERGIA E PRODUÇÃO INDUSTRIAL

**Projeto acadêmico | Dados sintéticos | Excel | Power Pivot | Modelagem Relacional | Tabelas Dinâmicas**

## 📌 Visão Geral

Quanto da energia consumida por uma máquina está realmente relacionado à produção?

Essa foi a principal pergunta que orientou o desenvolvimento deste projeto de análise de dados aplicado a um processo industrial.

O objetivo foi estruturar um modelo relacional capaz de integrar informações de produção, consumo de energia, manutenção e vendas, permitindo analisar indicadores operacionais e identificar relações entre desempenho produtivo e utilização de recursos energéticos.

Utilizando dados sintéticos, foi desenvolvido um modelo de dados no **Power Pivot**, com tabelas fato e dimensão relacionadas por chaves primárias e estrangeiras.

A partir dessa estrutura, foram criadas tabelas dinâmicas para explorar diferentes perspectivas do processo industrial, conectando consumo energético, produtividade, qualidade e manutenção.

## 🎯 Objetivos do Projeto

- Relacionar o consumo de energia com o volume produzido.
- Avaliar o consumo específico de energia por peça (kWh/peça).
- Comparar a produção entre equipamentos.
- Analisar a distribuição das vendas por segmento de clientes.
- Identificar a geração de refugos por turno.
- Avaliar o impacto das paradas de manutenção.
- Relacionar a criticidade dos equipamentos com as horas de indisponibilidade.
- Demonstrar como a integração de dados pode apoiar decisões de eficiência energética e operacional.

## 🏗️ 1. Modelagem Relacional dos Dados

Foi desenvolvido um modelo relacional utilizando o Power Pivot, estruturado em tabelas fato e tabelas dimensão.

### 📊 Tabelas Fato

As tabelas fato concentram os registros quantitativos das operações analisadas.

| Tabela | Informações |
|---|---|
| FAT_VENDAS | Registros de vendas e quantidades comercializadas |
| FAT_PRODUCAO | Quantidade produzida por equipamento |
| FAT_MANUTENCAO | Registros de manutenção e horas de parada |
| FAT_ENERGIA | Consumo energético dos equipamentos |

### 🧩 Tabelas Dimensão

As tabelas dimensão fornecem informações descritivas para segmentação e análise dos dados.

| Tabela | Informações |
|---|---|
| DIM_CLIENTES | Cadastro e segmentação de clientes |
| DIM_PRODUTOS | Identificação e características dos produtos |
| DIM_EQUIPAMENTOS | Cadastro e características dos equipamentos |

### 🔗 Relacionamentos

A integração foi realizada por meio de chaves primárias (PK) e estrangeiras (FK), permitindo conectar os registros das tabelas fato às respectivas dimensões.

Essa estrutura possibilita análises integradas por equipamento, produto, cliente e demais atributos disponíveis.

**Benefício da modelagem:** evitar a duplicação desnecessária de informações, organizar os relacionamentos e facilitar a criação de indicadores e análises multidimensionais.

## ⚡ 2. Análises Desenvolvidas

### 2.1 🔋 Consumo Específico de Energia – kWh/Peça

Análise da relação entre energia consumida e quantidade produzida.

**Indicador:**

\[
kWh/peça = \frac{\text{Energia consumida (kWh)}}{\text{Quantidade produzida}}
\]

Objetivos:
- Comparar o consumo específico entre equipamentos.
- Identificar máquinas com maior consumo energético por unidade produzida.
- Avaliar oportunidades de melhoria na eficiência energética.
- Apoiar a identificação de desvios no desempenho energético.

Essa análise é especialmente importante porque o consumo absoluto de energia, isoladamente, não permite avaliar a eficiência de um equipamento. Uma máquina pode consumir mais energia simplesmente porque produziu mais.

### 2.2 🏭 Quantidade de Produtos Produzidos por Equipamento

Análise da distribuição do volume produzido entre os equipamentos.

**Objetivos:**
- Comparar a contribuição produtiva das máquinas.
- Identificar a distribuição da carga de produção.
- Relacionar produtividade e consumo energético.
- Apoiar avaliações de capacidade e utilização dos equipamentos.

### 2.3 📦 Quantidade de Produtos Vendidos por Segmento

Análise das quantidades comercializadas, segmentadas por perfil de cliente.

**Objetivos:**
- Avaliar a distribuição das vendas por segmento.
- Identificar os segmentos com maior participação comercial.
- Relacionar informações comerciais com o planejamento produtivo.

### 2.4 🗑️ Quantidade de Refugos por Turno

Análise da geração de produtos não conformes em cada turno de produção.

**Objetivos:**
- Identificar diferenças na geração de refugos entre turnos.
- Investigar possíveis variações de processo.
- Apoiar ações de qualidade e melhoria contínua.
- Relacionar perdas produtivas com a utilização de recursos.

### 2.5 🛠️ Horas de Paradas por Tipo de Manutenção

Análise das horas de indisponibilidade classificadas conforme o tipo de manutenção.

**Objetivos:**
- Avaliar a distribuição das paradas entre modalidades de manutenção.
- Identificar quais categorias representam maior tempo de indisponibilidade.
- Apoiar o planejamento das atividades de manutenção.
- Investigar oportunidades de redução das perdas operacionais.

### 2.6 🚨 Horas Paradas por Equipamento e Criticidade

Análise do tempo de parada dos equipamentos considerando seus níveis de criticidade.

**Objetivos:**
- Identificar equipamentos críticos com maior impacto operacional.
- Priorizar recursos e intervenções de manutenção.
- Relacionar criticidade e indisponibilidade.
- Apoiar decisões de planejamento e gestão de ativos.

## 📈 3. Indicadores e Conceitos Aplicados

| Indicador / Conceito | Aplicação |
|---|---|
| kWh/peça | Consumo específico de energia |
| Volume produzido | Produtividade por equipamento |
| Volume vendido | Análise comercial por segmento |
| Refugo | Indicador de perdas de qualidade |
| Horas de parada | Indisponibilidade operacional |
| Tipo de manutenção | Classificação das intervenções |
| Criticidade | Priorização dos equipamentos |
| Modelagem relacional | Integração entre diferentes fontes de dados |

## 💡 4. Aplicação dos Resultados na Gestão Industrial

A integração das informações permite desenvolver uma visão mais abrangente do processo produtivo.

**Eficiência energética**
- Identificar equipamentos com maior consumo específico.
- Comparar consumo e volume de produção.
- Investigar possíveis desperdícios energéticos.
- Apoiar a definição de oportunidades de melhoria.

**Gestão da produção**
- Avaliar a distribuição da produção entre equipamentos.
- Relacionar volume produzido e demanda comercial.
- Identificar perdas associadas à geração de refugos.

**Gestão da manutenção**
- Identificar equipamentos com maior tempo de parada.
- Priorizar intervenções conforme a criticidade.
- Avaliar a participação dos diferentes tipos de manutenção nas perdas operacionais.

**Tomada de decisão integrada**

A principal contribuição do modelo está na possibilidade de analisar energia, produção, qualidade, vendas e manutenção de forma relacionada, em vez de avaliar cada indicador isoladamente.

## 🛠️ 5. Ferramentas e Tecnologias

| Ferramenta | Aplicação |
|---|---|
| Microsoft Excel | Organização e análise dos dados |
| Power Pivot | Modelagem relacional e integração das tabelas |
| Tabelas Dinâmicas | Análise multidimensional |
| Chaves PK/FK | Estruturação dos relacionamentos |

## ⚠️ 6. Considerações Metodológicas

Os dados utilizados são sintéticos e foram desenvolvidos para fins acadêmicos e de demonstração técnica.

O indicador kWh/peça representa uma relação entre consumo e volume produzido, mas não significa necessariamente que todo o consumo energético seja causado diretamente pela produção.

Para uma avaliação energética mais precisa, seria importante separar:
- Consumo durante a produção.
- Consumo em vazio.
- Consumo durante paradas.
- Consumo em partidas e transientes.
- Consumos auxiliares associados ao equipamento.

Também é importante considerar diferenças de mix de produtos, tempos de operação e condições de processo ao comparar equipamentos.

## 🎯 7. Conclusão

O projeto demonstra como a modelagem relacional e a integração de diferentes bases de dados podem ampliar a capacidade de análise de um processo industrial.

Ao relacionar consumo energético, produção, vendas, qualidade e manutenção, torna-se possível investigar fatores que influenciam o desempenho operacional e identificar oportunidades de melhoria.

O principal aprendizado é que **eficiência energética não deve ser avaliada somente pelo consumo total, mas também pela relação entre energia utilizada, produção realizada e condições operacionais do equipamento.**

## 👨‍💻 Competências Demonstradas

`Análise de Dados` | `Eficiência Energética` | `Gestão Industrial` | `Power Pivot` | `Excel` | `Modelagem Relacional` | `ETL` | `Tabelas Fato e Dimensão` | `PK/FK` | `Indicadores de Produção` | `Manutenção Industrial` | `Análise de Processos`

---

*Projeto acadêmico desenvolvido com dados sintéticos para demonstrar a aplicação de modelagem de dados e análise integrada em ambiente industrial.*
