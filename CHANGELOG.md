# Changelog

Todas as mudanças relevantes deste repositório são registradas aqui. O formato é baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/) e as datas seguem o padrão ISO (`AAAA-MM-DD`).

**Por que um changelog num repositório de dados:** praça de pedágio muda de dono, vira Free Flow ou deixa de cobrar quando um contrato termina. O changelog é o que permite a qualquer pessoa saber o que mudou e quando, e é o registro de frescor da base.

## [Não publicado]

- **Praças das rodovias estaduais e municipais**, começando por São Paulo, em levantamento concessão por concessão.

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
