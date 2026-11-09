# Dicionário de dados da base de praças de pedágio

Esta pasta guarda as bases públicas do repositório, em **CSV**, publicadas pelo Sem Parar sob licença **[CC BY 4.0](../LICENSE)**. O reuso é livre, inclusive comercial, desde que citada a fonte.

| Base | O que traz | Linhas |
|---|---|:---:|
| [pracas-de-pedagio](pracas-de-pedagio.csv) | Inventário praça a praça, com rodovia, km, município, sentido cobrado, concessão, coordenadas e link da tabela oficial de tarifas | 163 |
| [concessoes-rodoviarias](concessoes-rodoviarias.csv) | Quem administra cada rodovia: concessão, esfera, órgão regulador, rodovias, estados, número de praças e situação do Free Flow | 29 |
| [rodovias-pedagiadas](rodovias-pedagiadas.csv) | Uma linha por rodovia, concessão e estado, com o nome popular do trecho e os municípios com praça | 55 |

Codificação **UTF-8**, separador **vírgula**, quebra de linha **CRLF** (padrão RFC 4180), datas em **ISO** (`AAAA-MM-DD`), decimais com **ponto**. Listas dentro de uma célula usam **ponto e vírgula**. Se o Excel embaralhar os acentos, abra pelo menu **Dados**, opção de importar texto, e escolha **UTF-8**.

---

## Três regras que valem para todas as bases

**1. Nenhum valor monetário é armazenado.** Não há tarifa em reais em lugar nenhum. Cada praça e cada concessão traz o link da tabela oficial de tarifas da ANTT.

**2. `n/d` em vez de chute.** Campo não confirmado em fonte oficial aparece como `n/d`. Nenhum dado aqui foi inferido, deduzido ou preenchido por analogia.

**3. Divergência se registra.** Quando duas fontes oficiais discordam, adotamos a de maior hierarquia e anotamos a divergência na coluna de observação. As divergências desta versão estão tabuladas em [Metodologia e fontes](../docs/metodologia-e-fontes.md#divergências-declaradas).

O critério do que conta como uma praça também está em [Metodologia e fontes](../docs/metodologia-e-fontes.md#o-que-conta-como-uma-praça).

---

## `pracas-de-pedagio.csv`

Uma linha por **praça física de cobrança em operação**.

| Coluna | Tipo | Descrição |
|---|---|---|
| `id_praca` | texto | Identificador estável da linha. A letra indica a esfera (`F` federal); o número nunca é reaproveitado |
| `praca` | texto | Nome da praça como registrado no cadastro da ANTT, como `Moreira César` ou `P3`. Onde registros por sentido foram reunidos, o nome comum a eles |
| `tipo` | texto | `principal` ou `bloqueio` (praça auxiliar em acesso) |
| `rodovia` | texto | Sigla oficial: `BR-116`, `PR-151` |
| `uf` | texto | Sigla do estado onde a praça fica |
| `municipio` | texto | Município registrado no cadastro da ANTT |
| `km` | número | Quilômetro do cadastro da ANTT. Onde registros foram reunidos, o menor deles, e os demais na observação |
| `sentidos_cobrados` | texto | `ambos`, `crescente` ou `decrescente`. Crescente é o sentido em que a quilometragem aumenta |
| `concessao` | texto | Concessão responsável, com o nome da Lista de Concessões da ANTT |
| `esfera` | texto | `federal`, `estadual` ou `municipal` |
| `orgao_regulador` | texto | Quem regula o contrato, como `ANTT` |
| `situacao` | texto | `ativa` nesta versão. Praça desativada sai da base e é registrada no CHANGELOG |
| `url_tarifa_oficial` | URL | Página da tabela oficial de tarifas da concessão |
| `latitude`, `longitude` | número | Coordenadas do cadastro da ANTT |
| `fonte` | URL | Fonte oficial da linha |
| `atualizado_em` | data | Data da última conferência da linha |
| `observacao` | texto | Divergências, registros reunidos e anúncios ainda não cumpridos |

---

## `concessoes-rodoviarias.csv`

Uma linha por **concessão com praça de pedágio**.

| Coluna | Tipo | Descrição |
|---|---|---|
| `concessao` | texto | Nome da concessão na Lista de Concessões da ANTT |
| `esfera` | texto | `federal`, `estadual` ou `municipal` |
| `orgao_regulador` | texto | Quem regula o contrato |
| `rodovias` | lista | Rodovias com praça da concessão, separadas por ponto e vírgula |
| `ufs` | lista | Estados com praça da concessão |
| `n_pracas` | número | Praças da concessão nesta base. Total derivado, conferido por soma contra `pracas-de-pedagio.csv` em toda versão |
| `free_flow` | texto | `sim` (já cobra também por pórtico), `previsto`, `adiado`, `anunciado` (data oficial ainda não cumprida) ou `não`, conforme o repositório [SEM-PARAR-FREE-FLOW](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW) e a ANTT |
| `url_concessao` | URL | Página da concessão na ANTT |
| `url_tarifa_oficial` | URL | Página da tabela oficial de tarifas |
| `fonte`, `atualizado_em` | URL, data | Procedência e data da conferência |
| `observacao` | texto | Transições de contrato e divergências |

---

## `rodovias-pedagiadas.csv`

Uma linha por **rodovia, concessão e estado**. Uma rodovia longa como a BR-116 ocupa várias linhas.

| Coluna | Tipo | Descrição |
|---|---|---|
| `rodovia` | texto | Sigla oficial |
| `nome_popular` | texto | Nome pelo qual o trecho é conhecido, como `Via Dutra` ou `Fernão Dias`. `n/d` quando não há nome consagrado |
| `uf` | texto | Estado |
| `concessao` | texto | Concessão responsável pelo trecho |
| `esfera` | texto | `federal`, `estadual` ou `municipal` |
| `n_pracas` | número | Praças da concessão nessa rodovia e nesse estado. Total derivado, conferido por soma |
| `municipios_com_praca` | lista | Municípios com praça, na ordem do km |
| `free_flow_na_concessao` | texto | A mesma classificação da coluna `free_flow` da base de concessões |
| `fonte`, `atualizado_em` | URL, data | Procedência e data da conferência |
