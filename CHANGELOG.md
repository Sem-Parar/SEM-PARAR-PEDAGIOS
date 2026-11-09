# Changelog

Todas as mudanças relevantes deste repositório são registradas aqui. O formato é baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/) e as datas seguem o padrão ISO (`AAAA-MM-DD`).

**Por que um changelog num repositório de dados:** praça de pedágio muda de dono, vira Free Flow ou deixa de cobrar quando um contrato termina. O changelog é o que permite a qualquer pessoa saber o que mudou e quando, e é o registro de frescor da base.

## [Não publicado]

- **Praças das rodovias estaduais dos demais estados e das municipais**, em levantamento concessão por concessão.

---

## [0.2.0], 2026-11-09

As rodovias estaduais de São Paulo entram na base. São **156 praças** de **20 concessões** reguladas pela ARTESP, e o total vai de 163 para **319 praças**, em **66 rodovias** e **49 concessões**. São Paulo passa a ser o estado com mais praças, 173 somando federais e estaduais.

### Adicionado

- **156 praças estaduais de São Paulo** em [`dados/pracas-de-pedagio.csv`](dados/pracas-de-pedagio.csv), com identificador `S`, a partir do cadastro de ativos da ARTESP de 30 de maio de 2025 e conferidas contra as passagens por praça de 2026.
- **20 concessões estaduais** em [`dados/concessoes-rodoviarias.csv`](dados/concessoes-rodoviarias.csv) e as linhas correspondentes em [`dados/rodovias-pedagiadas.csv`](dados/rodovias-pedagiadas.csv), que vai a 112 linhas.
- **[Praças de pedágio por estado](PRACAS-DE-PEDAGIO-POR-ESTADO.md)**, página nova, com cada estado separado em federais e estaduais e as praças por município.
- **A seção paulista** em [Concessões rodoviárias](CONCESSOES-RODOVIARIAS.md) e em [Metodologia e fontes](docs/metodologia-e-fontes.md), com o caminho dos 239 registros de pedágio da ARTESP às 156 praças.

### Alterado

- **README, praças por rodovia e dicionário de dados** passaram a cobrir as duas esferas, com as colunas de federais e estaduais na tabela por estado e os sentidos da ARTESP (ponto cardeal e pista do Rodoanel).

### Corrigido

- **A data da autorização da ANTT para o Free Flow de Simão Pereira, na BR-040**, aparecia como 6 de novembro. A Deliberação ANTT nº 310 é de 4 de novembro de 2026, publicada no dia 5.

### Notas de dado

- **Pirangi e Monte Alto**, da Ecovias Noroeste Paulista, viraram pórtico em 1º de novembro de 2026 e não entram. **Colina** segue na base, com o pórtico anunciado para 1º de dezembro de 2026 na observação.
- **As nove praças da Renovias** entram sob a **Rota Mogiana**, que assumiu o trecho em 1º de novembro de 2026.
- **Tebe e ViaOeste**, contratos encerrados, ainda aparecem no cadastro de ativos da ARTESP. Ficaram fora, porque as mesmas praças estão registradas sob as concessionárias atuais.

---

## [0.1.0], 2026-11-09

Primeira versão pública. A base aberta das praças de pedágio com cabine das rodovias federais concedidas: **163 praças**, em **25 rodovias**, **29 concessões** e **12 estados**, conferidas contra o cadastro da ANTT de 3 de novembro de 2026.

### Adicionado

- **[`dados/pracas-de-pedagio.csv`](dados/pracas-de-pedagio.csv)**, com as 163 praças, uma linha por local, com rodovia, km, município, sentido cobrado, concessão, coordenadas e o link da tabela oficial de tarifas.
- **[`dados/concessoes-rodoviarias.csv`](dados/concessoes-rodoviarias.csv)**, com as 29 concessões e a situação do Free Flow em cada uma.
- **[`dados/rodovias-pedagiadas.csv`](dados/rodovias-pedagiadas.csv)**, com 55 linhas de rodovia, concessão e estado e o nome popular de cada trecho.
- **[Praças de pedágio por rodovia](PRACAS-DE-PEDAGIO-POR-RODOVIA.md)** e **[Concessões rodoviárias com pedágio no Brasil](CONCESSOES-RODOVIARIAS.md)**, geradas a partir das bases.
- **[Metodologia e fontes](docs/metodologia-e-fontes.md)**, com o critério de contagem e o caminho dos 289 registros da ANTT às 163 praças, e o **[dicionário de dados](dados/README.md)**.

### Notas de dado

- **Três contratos encerrados ainda aparecem como ativos no cadastro de praças da ANTT** (Concer, Ecovias Sul e Rodovia do Aço). Ficaram fora da contagem, com a divergência declarada.
- **A praça de Simão Pereira (MG), na BR-040**, segue na base com a troca por Free Flow autorizada pela ANTT para 16/11/2026 registrada na observação. Sai quando o pórtico começar a cobrar.
