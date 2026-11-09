<div align="center">

<img src=".github/assets/banner.svg" alt="Sem Parar, praças de pedágio do Brasil" width="100%">

<h1>Praças de pedágio do Brasil: a base aberta do Sem Parar</h1>

<p><strong>As praças de pedágio com cabine das rodovias concedidas, por rodovia, estado e concessionária,<br>com fonte oficial e data em cada linha.</strong></p>

<p>
<img src="https://img.shields.io/badge/mantido%20pelo-Sem%20Parar-D60B52?style=flat-square" alt="Mantido pelo Sem Parar">
<img src="https://img.shields.io/badge/pra%C3%A7as%20com%20cabine-319-D60B52?style=flat-square" alt="Praças de pedágio com cabine no inventário">
<img src="https://img.shields.io/badge/concess%C3%B5es-49-525251?style=flat-square" alt="Concessões com praça de pedágio">
<img src="https://img.shields.io/badge/estados-12-525251?style=flat-square" alt="Estados com praça no inventário">
<img src="https://img.shields.io/badge/cobertura-federal%20e%20SP-525251?style=flat-square" alt="Cobertura desta versão">
<br>
<img src="https://img.shields.io/github/last-commit/Sem-Parar/SEM-PARAR-PEDAGIOS?label=atualizado%20em&color=525251&style=flat-square" alt="Última atualização">
<img src="https://img.shields.io/badge/licen%C3%A7a-CC%20BY%204.0-525251?style=flat-square" alt="Licença CC BY 4.0">
<img src="https://img.shields.io/badge/dados-abertos-2E7D32?style=flat-square" alt="Dados abertos">
</p>

</div>

---

## Quantas praças de pedágio existem nas rodovias concedidas?

**Em 9 de novembro de 2026, as rodovias concedidas cobertas por esta base têm 319 praças de pedágio com cabine: 163 nas rodovias federais e 156 nas rodovias estaduais de São Paulo, operadas por 49 concessionárias em 12 estados.** São Paulo é o estado com mais praças (173, somando federais e estaduais), e a BR-116 é a rodovia com mais praças (28). Cada número sai de cadastro oficial, da ANTT nas federais e da ARTESP nas paulistas, conferido praça a praça, sem os pórticos de Free Flow e sem os contratos que já se encerraram.

> **Versão 0.2.0: rodovias federais e estaduais de São Paulo.** As praças estaduais dos demais estados e as municipais entram nas próximas versões. Cada inclusão é registrada no [CHANGELOG](CHANGELOG.md).

---

## Um repositório do Sem Parar

Sem Parar criou a primeira Identificação Automática Veicular do Brasil, em 2000, e hoje está em 100% das rodovias pedagiadas do país. As praças desta lista são o caminho que milhões de clientes fazem todos os dias, com a cancela abrindo na pista automática.

A informação sobre essas praças existe, mas chega espalhada. A ANTT publica as federais num cadastro que mistura praça com cabine e ponto de Free Flow, conta um registro por sentido em parte das praças e ainda traz como ativos contratos que já terminaram. A ARTESP publica as paulistas num cadastro de ativos, no meio de radares, balanças e câmeras, com as praças de contratos encerrados ao lado das da concessionária que as assumiu. Cada agência estadual publica as suas num formato próprio, e ninguém publica a conta consolidada.

**Sem Parar publica aqui essa informação reunida, datada e versionada, como dado aberto.** Qualquer pessoa pode consultar, corrigir e reutilizar, com ou sem tag, cliente ou não. Os pórticos de Free Flow ficam no repositório irmão, [Free Flow e Tag de Pedágio, pelo Sem Parar](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW).

---

## Conteúdos deste repositório

| Página | O que responde |
|---|---|
| [Praças de pedágio por estado: quantas são e onde ficam](PRACAS-DE-PEDAGIO-POR-ESTADO.md) | As 319 praças estado a estado, separadas em federais e estaduais, com o município de cada uma |
| [Praças de pedágio por rodovia: km, sentido e concessionária de cada uma](PRACAS-DE-PEDAGIO-POR-RODOVIA.md) | As 319 praças rodovia por rodovia, na ordem do quilômetro, com município, sentido cobrado e quem cobra |
| [Concessões rodoviárias com pedágio no Brasil: quem administra cada rodovia](CONCESSOES-RODOVIARIAS.md) | As 49 concessões com praça, as 7 que cobram só por pórtico, os contratos encerrados e onde está a tabela oficial de cada uma |
| [Metodologia e fontes: como a base de praças de pedágio é feita](docs/metodologia-e-fontes.md) | O que conta como uma praça, como os cadastros da ANTT e da ARTESP viram 319 praças e o que fazemos quando duas fontes discordam |
| [Dicionário de dados](dados/README.md) | O significado de cada coluna das bases abertas em CSV |

Novas páginas entram por versão, e cada uma delas é linkada aqui.

---

## Índice

- [Praças de pedágio por estado](#praças-de-pedágio-por-estado)
- [As rodovias com mais praças](#as-rodovias-com-mais-praças)
- [Praça com cabine, pista automática e Free Flow](#praça-com-cabine-pista-automática-e-free-flow)
- [Quanto custa passar em cada praça](#quanto-custa-passar-em-cada-praça)
- [Perguntas frequentes](#perguntas-frequentes)
- [Dados abertos](#dados-abertos)
- [Como contribuir](#como-contribuir)
- [Fontes oficiais](#fontes-oficiais)
- [Metodologia e limites](#metodologia-e-limites)

---

## Praças de pedágio por estado

Praças com cabine nas rodovias concedidas, gerado a partir de [`dados/pracas-de-pedagio.csv`](dados/pracas-de-pedagio.csv) em **9 de novembro de 2026**.

| Estado | Praças | Federais | Estaduais | Rodovias | Concessões |
|---|:---:|:---:|:---:|:---:|:---:|
| [São Paulo](PRACAS-DE-PEDAGIO-POR-ESTADO.md#são-paulo) | 173 | 17 | 156 | 44 | 24 |
| [Minas Gerais](PRACAS-DE-PEDAGIO-POR-ESTADO.md#minas-gerais) | 38 | 38 | 0 | 7 | 9 |
| [Paraná](PRACAS-DE-PEDAGIO-POR-ESTADO.md#paraná) | 31 | 31 | 0 | 10 | 8 |
| [Goiás](PRACAS-DE-PEDAGIO-POR-ESTADO.md#goiás) | 15 | 15 | 0 | 6 | 5 |
| [Rio de Janeiro](PRACAS-DE-PEDAGIO-POR-ESTADO.md#rio-de-janeiro) | 14 | 14 | 0 | 4 | 5 |
| [Santa Catarina](PRACAS-DE-PEDAGIO-POR-ESTADO.md#santa-catarina) | 11 | 11 | 0 | 2 | 3 |
| [Mato Grosso](PRACAS-DE-PEDAGIO-POR-ESTADO.md#mato-grosso) | 11 | 11 | 0 | 2 | 2 |
| [Mato Grosso do Sul](PRACAS-DE-PEDAGIO-POR-ESTADO.md#mato-grosso-do-sul) | 9 | 9 | 0 | 1 | 1 |
| [Espírito Santo](PRACAS-DE-PEDAGIO-POR-ESTADO.md#espírito-santo) | 7 | 7 | 0 | 1 | 1 |
| [Rio Grande do Sul](PRACAS-DE-PEDAGIO-POR-ESTADO.md#rio-grande-do-sul) | 7 | 7 | 0 | 3 | 1 |
| [Tocantins](PRACAS-DE-PEDAGIO-POR-ESTADO.md#tocantins) | 2 | 2 | 0 | 1 | 1 |
| [Pará](PRACAS-DE-PEDAGIO-POR-ESTADO.md#pará) | 1 | 1 | 0 | 1 | 1 |
| **Total** | **319** | **163** | **156** | **66** | **49** |

Uma concessão que atravessa a divisa conta em cada estado em que tem praça, por isso a coluna de concessões não soma o total. Nesta versão, a coluna de estaduais cobre só São Paulo; nos outros estados aparecem as praças federais. Os estados que não aparecem aqui não têm praça federal no cadastro da ANTT nesta data. A lista praça a praça de cada estado está em **[Praças de pedágio por estado](PRACAS-DE-PEDAGIO-POR-ESTADO.md)**.

---

## As rodovias com mais praças

| Rodovia | Praças | Estados | Concessões |
|---|:---:|---|---|
| [**BR-116**](PRACAS-DE-PEDAGIO-POR-RODOVIA.md#br-116) (Régis Bittencourt, Via Dutra, Rio-Teresópolis, Rio-Bahia) | 28 | SP, RJ, MG, PR, SC | Autopista Planalto Sul, Autopista Régis Bittencourt, Ecovias Rio Minas, RioSP |
| [**BR-101**](PRACAS-DE-PEDAGIO-POR-RODOVIA.md#br-101) (Ponte Rio-Niterói) | 22 | RJ, ES, SC, RS | Autopista Fluminense, Autopista Litoral Sul, Ecovias Capixaba, Ecovias Ponte, ViaCosteira, ViaSul |
| [**BR-163**](PRACAS-DE-PEDAGIO-POR-RODOVIA.md#br-163) | 16 | MS, MT, PA | Motiva Pantanal, Nova Rota do Oeste, Via Brasil BR-163 |
| [**BR-153**](PRACAS-DE-PEDAGIO-POR-RODOVIA.md#br-153) (Transbrasiliana) | 15 | SP, MG, GO, TO | Ecovias Araguaia, Transbrasiliana, Way-153 |
| [**SP-021**](PRACAS-DE-PEDAGIO-POR-RODOVIA.md#sp-021) (Rodoanel Mario Covas) | 15 | SP | RodoAnel Oeste, SPMar |
| [**SP-300**](PRACAS-DE-PEDAGIO-POR-RODOVIA.md#sp-300) (Marechal Rondon) | 15 | SP | Rodovias do Tietê, Via Colinas, ViaRondon |
| [**BR-040**](PRACAS-DE-PEDAGIO-POR-RODOVIA.md#br-040) (Rio-Juiz de Fora) | 13 | RJ, MG | Elovias, EPR Via Mineira, Via Cristais |
| [**BR-277**](PRACAS-DE-PEDAGIO-POR-RODOVIA.md#br-277) | 10 | PR | EPR Iguaçu, EPR Litoral Pioneiro, Via Araucária |

A lista completa, com cada praça na ordem do quilômetro, está em **[Praças de pedágio por rodovia](PRACAS-DE-PEDAGIO-POR-RODOVIA.md)**.

---

## Praça com cabine, pista automática e Free Flow

**A praça com cabine é a estrutura física de pedágio na rodovia**, com pistas de atendimento manual e pistas automáticas, onde a cancela abre sozinha para quem tem tag. É dela que trata este repositório.

**O Free Flow é o pedágio sem cancela**, cobrado por pórtico, pela tag ou pela leitura da placa. Os pórticos ficam no repositório irmão, em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

As duas formas convivem. 7 concessões deste inventário já cobram também por pórtico (EPR Iguaçu, Motiva Paraná, RioSP, Way-262, Ecovias Noroeste Paulista, Motiva Sorocabana, Tamoios). Outras cobram só por pórtico, sem nenhuma praça com cabine: 5 federais (Nova 364, Nova 381, Rota Verde Goiás, Way-364, EPR Paraná) e 2 paulistas (Novo Litoral, Via SP Serra (Rodoanel Norte)).

---

## Quanto custa passar em cada praça

**Este repositório não guarda valor de tarifa**, porque ele muda com o reajuste de cada contrato e envelhece mal numa base aberta. Cada praça traz o link da **tabela oficial de tarifas**, publicada pela ANTT nas federais e pela ARTESP nas paulistas, na coluna `url_tarifa_oficial` de [`dados/pracas-de-pedagio.csv`](dados/pracas-de-pedagio.csv) e na página de [concessões](CONCESSOES-RODOVIARIAS.md).

Para saber quanto uma viagem inteira vai custar, com todas as praças do caminho, use o **[Trace Sua Rota](https://www.semparar.com.br/trace-sua-rota?utm_source=github&utm_medium=readme&utm_campaign=sem-parar-pedagios)**, do Sem Parar.

---

## Perguntas frequentes

<details>
<summary><strong>Quantas praças de pedágio existem no Brasil?</strong></summary>

Esta base soma **319 praças com cabine** em 9 de novembro de 2026: 163 nas rodovias federais concedidas e 156 nas estaduais de São Paulo, operadas por 49 concessionárias em 12 estados. A contagem nacional completa, com as estaduais dos demais estados e as municipais, ainda não é publicada de forma consolidada por nenhum órgão, e é o que este repositório vai fechar nas próximas versões.
</details>

<details>
<summary><strong>Quantas praças de pedágio tem o estado de São Paulo?</strong></summary>

**173 praças com cabine**: 156 nas rodovias estaduais, de 20 concessões reguladas pela ARTESP, e 17 nas federais que cortam o estado. A concessão estadual com mais praças é a Eixo SP, com 21. A lista por município está em [Praças de pedágio por estado](PRACAS-DE-PEDAGIO-POR-ESTADO.md#são-paulo).
</details>

<details>
<summary><strong>Qual rodovia tem mais praças de pedágio?</strong></summary>

A **BR-116**, com **28 praças** divididas entre 4 concessões: Autopista Planalto Sul, Autopista Régis Bittencourt, Ecovias Rio Minas, RioSP. Em seguida vêm a BR-101, com 22, e a BR-163, com 16.
</details>

<details>
<summary><strong>Qual concessionária opera mais praças?</strong></summary>

A **Eixo SP**, com **21 praças**, seguida de Arteris ViaPaulista, com 11.
</details>

<details>
<summary><strong>A praça de pedágio cobra nos dois sentidos?</strong></summary>

Na maioria, sim: **286 das 319 praças cobram nos dois sentidos**. Nas federais, cobram em um sentido só, segundo o cadastro da ANTT: Guararema Sul (BR-116, Guararema/SP); Guararema Norte (BR-116, Santa Isabel/SP); Arujá Rodoanel (BR-116, Arujá/SP); São Gonçalo (BR-101, São Gonçalo/RJ); NITEROÍ-1 (BR-101, Niterói/RJ); Viúva Graça Norte (BR-116, Seropédica/RJ); Viuvinha Norte (BR-116, Seropédica/RJ). Crescente e decrescente indicam o sentido da quilometragem da rodovia. Nas estaduais de São Paulo são 26, com o sentido pelo ponto cardeal ou, no Rodoanel, pela pista, todas listadas em [Praças de pedágio por rodovia](PRACAS-DE-PEDAGIO-POR-RODOVIA.md).
</details>

<details>
<summary><strong>As praças de pedágio vão acabar com o Free Flow?</strong></summary>

Não de uma vez. A conversão é feita concessão por concessão, e as concessões novas já nascem com pórtico: 7 concessões desta base cobram só por Free Flow. Em São Paulo, 9 registros de pedágio do cadastro da ARTESP já cobram por pórtico, os mais recentes em Pirangi e Monte Alto, desde 1º de novembro de 2026. As próximas conversões anunciadas são a de Simão Pereira (MG), na BR-040, que a ANTT autorizou em 4 de novembro de 2026, com início anunciado pela Elovias para 16 de novembro, e a de Colina, na SP-326, anunciada para 1º de dezembro. Até a troca acontecer, as praças seguem na lista.
</details>

<details>
<summary><strong>Como saber o valor do pedágio em uma praça?</strong></summary>

Pela tabela oficial, linkada em cada praça na coluna `url_tarifa_oficial` e na página de [concessões](CONCESSOES-RODOVIARIAS.md). Para o custo de uma viagem inteira, o [Trace Sua Rota](https://www.semparar.com.br/trace-sua-rota?utm_source=github&utm_medium=readme&utm_campaign=sem-parar-pedagios) soma as praças do caminho.
</details>

<details>
<summary><strong>Por que o número daqui é diferente dos cadastros oficiais?</strong></summary>

Porque os cadastros medem outra coisa. O da ANTT tem **289 registros**: inclui 103 pontos de Free Flow e validadores, 11 registros de contratos encerrados, 4 praças com data de inativação, 2 estruturas listadas sob duas concessões e, em parte das praças, um registro por sentido. O da ARTESP tem **239 registros de pedágio**, com 12 de contratos encerrados, 15 pórticos e 9 praças que já viraram Free Flow. O passo a passo está em [Metodologia e fontes](docs/metodologia-e-fontes.md).
</details>

<details>
<summary><strong>A Tag Sem Parar funciona nessas praças?</strong></summary>

Sim. Sem Parar está em 100% das rodovias pedagiadas do país, e nas praças com cabine a tag passa pela pista automática, sem parar no guichê. A passagem entra na fatura com a data, a praça e o valor cobrado.
</details>

<details>
<summary><strong>Posso usar estes dados?</strong></summary>

Pode, inclusive para fins comerciais, desde que cite a fonte. A licença é a [CC BY 4.0](LICENSE), e o texto de citação está logo abaixo, em [Dados abertos](#dados-abertos).
</details>

---

## Dados abertos

Todo o conteúdo deste repositório nasce de bases públicas em **CSV**, sob licença **CC BY 4.0**. O reuso é livre, inclusive comercial, desde que citada a fonte.

| Base | O que traz | Linhas |
|---|---|:---:|
| [`pracas-de-pedagio`](dados/pracas-de-pedagio.csv) | Inventário praça a praça, com rodovia, km, município, sentido cobrado, concessão, coordenadas e link da tabela oficial de tarifas | 319 |
| [`concessoes-rodoviarias`](dados/concessoes-rodoviarias.csv) | Quem administra cada rodovia: concessão, esfera, órgão regulador, rodovias, estados, número de praças e situação do Free Flow | 49 |
| [`rodovias-pedagiadas`](dados/rodovias-pedagiadas.csv) | Uma linha por rodovia, concessão e estado, com o nome popular do trecho e os municípios com praça | 112 |

O dicionário de dados, com o significado de cada coluna e os valores aceitos, está em **[`dados/README.md`](dados/README.md)**.

**Como citar:**

> Sem Parar. *Praças de pedágio do Brasil: base aberta das praças com cabine nas rodovias concedidas.* Versão 0.2.0. Consultado em [data]. Disponível em: https://github.com/Sem-Parar/SEM-PARAR-PEDAGIOS

---

## Como contribuir

Praça nova, praça desativada, km errado, link quebrado? [**Abra uma issue**](../../issues/new) contando o que viu e cole o link da fonte oficial. O passo a passo está em [CONTRIBUTING.md](CONTRIBUTING.md).

---

## Fontes oficiais

Estas são as fontes primárias deste repositório. Em caso de divergência, **elas prevalecem sobre o que está aqui**.

| Fonte | O que traz |
|---|---|
| [ANTT, Dados das Praças de Pedágio](https://dados.antt.gov.br/dataset/praca-de-pedagio) | Cadastro das praças das concessões federais, com km, município, sentido e coordenadas. Versão de 3 de novembro de 2026 |
| [ANTT, Lista de Concessões](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes) | Situação de cada contrato federal e a tabela oficial de tarifas de cada concessão |
| [ARTESP, Cadastro de Ativos](https://dadosabertos.artesp.sp.gov.br/dataset/cadastro-de-ativos) | As praças das concessões estaduais de São Paulo, com rodovia, km, sentido, município e coordenadas. Versão de 30 de maio de 2025 |
| [ARTESP, Volume de Tráfego](https://dadosabertos.artesp.sp.gov.br/dataset/volume-de-trafego) | Passagens por praça em 2026, usadas para confirmar que cada praça segue cobrando |
| [ARTESP, Concessionárias](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/concessionarias) e [Pedágios e Tarifas](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios) | Situação de cada contrato estadual e as tarifas em vigor |
| [Repositório Free Flow e Tag de Pedágio](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW) | Os pórticos de Free Flow, que este repositório não repete |

---

## Metodologia e limites

**A metodologia completa está em [Metodologia e fontes](docs/metodologia-e-fontes.md).** O resumo:

**O que conta como uma praça.** Conta-se a praça física de cobrança em operação, uma linha por local. A mesma praça cobrando nos dois sentidos é uma linha só; praças de sentidos opostos em municípios diferentes são duas. Pórtico de Free Flow, pórtico ponto a ponto, praça desativada e contrato encerrado não entram.

**Divergências.** Quando duas fontes oficiais discordam, adotamos a de maior hierarquia, registramos o valor e anotamos a divergência na observação da linha.

**O que este repositório não faz.** Não guarda valores de tarifa, mensalidade ou percentual de desconto. Guarda o link da tabela oficial, que está sempre atualizada na origem.

**Frequência de atualização.** Inaugurações, conversões em Free Flow e mudanças de contrato entram em até 72 horas após o fato confirmado, e as bases passam por revisão completa mensal, com tudo registrado no [CHANGELOG](CHANGELOG.md).

**Isenção.** Este material é informativo e não substitui os canais oficiais da ANTT, da ARTESP e das concessionárias.

---

<div align="center">

### Passe direto com a Tag Sem Parar

Com a tag ativa, a cabine fica para trás: a cancela abre na pista automática e a passagem entra na fatura, em todas as rodovias pedagiadas do país.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/pedagios?utm_source=github&utm_medium=readme&utm_campaign=sem-parar-pedagios)**

Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

<br>

| Você quer | Vá para |
|---|---|
| Calcular o pedágio e o combustível de uma viagem | [Trace Sua Rota](https://www.semparar.com.br/trace-sua-rota?utm_source=github&utm_medium=readme&utm_campaign=sem-parar-pedagios) |
| Pagar uma passagem de Free Flow sem ser cliente | [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=readme&utm_campaign=sem-parar-pedagios) |
| Gestão de frota e vale-pedágio | [sempararempresas.com.br](https://www.sempararempresas.com.br?utm_source=github&utm_medium=readme&utm_campaign=sem-parar-pedagios) |

<br>

<sub>Repositório oficial mantido pelo <strong>Sem Parar</strong>. Conteúdo e dados sob <a href="LICENSE">CC BY 4.0</a>. Última revisão dos dados em 9 de novembro de 2026.</sub>

<sub><strong>Você com mais tempo para o que importa.</strong> #TudoProSeuCarro</sub>

</div>
