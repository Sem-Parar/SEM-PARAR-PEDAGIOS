# Metodologia e fontes: como a base de praças de pedágio é feita

**Os dados deste repositório saem de fonte oficial, sempre: o cadastro de praças de pedágio da ANTT para as rodovias federais, conferido contra a Lista de Concessões da própria ANTT.** Cada linha traz a fonte e a data da conferência, e toda decisão de contagem está escrita aqui antes de virar número.

Esta página existe para que qualquer pessoa possa auditar o que está publicado: de onde veio cada número, o que conta como uma praça, como o cadastro oficial vira este inventário e o que fazemos quando duas fontes discordam.

> Publicado em 9 de novembro de 2026.
> Parte do repositório [Praças de pedágio do Brasil, pelo Sem Parar](../README.md). O significado de cada coluna das bases está no [dicionário de dados](../dados/README.md).

---

## Índice

- [De onde vem cada dado](#de-onde-vem-cada-dado)
- [O que conta como uma praça?](#o-que-conta-como-uma-praça)
- [Do cadastro da ANTT a este inventário](#do-cadastro-da-antt-a-este-inventário)
- [Divergências declaradas](#divergências-declaradas)
- [Por que aqui não tem tarifa](#por-que-aqui-não-tem-tarifa)
- [Como os arquivos CSV são formatados](#como-os-arquivos-csv-são-formatados)
- [Com que frequência isso é atualizado](#com-que-frequência-isso-é-atualizado)
- [O que esta base não faz](#o-que-esta-base-não-faz)
- [Como citar e reutilizar](#como-citar-e-reutilizar)

---

## De onde vem cada dado

As fontes têm hierarquia. Quando duas se cruzam, prevalece a de cima, e a de baixo vira observação.

| Ordem | Fonte | O que ela responde melhor |
|:---:|---|---|
| 1 | [Dados das Praças de Pedágio, ANTT](https://dados.antt.gov.br/dataset/praca-de-pedagio) | Localização de cada praça federal: rodovia, km, município, sentido e coordenadas. Versão de 3 de novembro de 2026 |
| 2 | [Lista de Concessões, ANTT](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes) | Situação de cada contrato (vigente, encerrado, caducidade) e a tabela oficial de tarifas de cada concessão |
| 3 | Agências estaduais e prefeituras | As praças estaduais e municipais, a partir das próximas versões |
| 4 | Canal oficial da concessionária | Sentido cobrado, tabela tarifária e mudanças de operação |
| 5 | Imprensa e comunicados | Datas de anúncio e contexto. **Nunca sozinha muda um número da base** |

**Anúncio é promessa, não fato.** Quando uma concessionária anuncia que uma praça vai virar Free Flow numa data, a praça continua na base até a troca acontecer, com o anúncio registrado na observação da linha.

---

## O que conta como uma praça?

Todo número que conta coisas depende de uma definição, e a nossa está escrita antes da primeira linha existir.

**Conta-se a praça física de cobrança em operação, uma linha por local.**

| Situação | Conta? |
|---|---|
| Praça com cabine ou pista automática, cobrando | **Sim**, uma linha por local |
| A mesma praça cobrando nos dois sentidos | Uma linha só, com os sentidos na coluna `sentidos_cobrados` |
| Registros da mesma praça, no mesmo município, em km próximos (cabines de cada sentido ou defasadas) | Uma linha só, com os km de cada registro na observação |
| Praças de sentidos opostos em municípios diferentes | Duas linhas, como Guararema Norte (Santa Isabel) e Guararema Sul (Guararema), na Via Dutra |
| Praça auxiliar em acesso, cobrando | **Sim**, com `tipo` = `bloqueio` |
| Pórtico de Free Flow | **Não.** Fica no [repositório irmão](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW) |
| Praça com data de inativação no cadastro | Não |
| Praça de contrato encerrado ou com caducidade declarada | Não, mesmo que o cadastro ainda a marque como ativa |
| Praça com conversão em Free Flow anunciada | Sim, até a troca acontecer |

---

## Do cadastro da ANTT a este inventário

O cadastro de praças da ANTT, na versão de 3 de novembro de 2026, tem **289 registros**, todos marcados como ativos. Este é o caminho até as **163 praças** deste repositório:

| Etapa | Registros | Sobram |
|---|:---:|:---:|
| Cadastro completo | | 289 |
| Pontos de Free Flow e validadores de Free Flow (vão para o repositório irmão) | 103 | 186 |
| Praças com data de inativação preenchida | 4 | 182 |
| Contratos encerrados ou com caducidade declarada (Concer 3, Ecovias Sul 5, Rodovia do Aço 3) | 11 | 171 |
| Estruturas de Viúva Graça listadas também sob a Ecovias Rio Minas | 2 | 169 |
| Registros por sentido reunidos numa praça (Moreira César, Jacareí, Arujá, Itatiaia e Mairiporã) | 6 | **163** |

As quatro praças com data de inativação são: Concebra P4 ITUMBIARA, em 22/05/2026; Concebra P3 PROF JAMIL, em 22/05/2026; Ecovias Do Cerrado P5 - PARANAIGUARA, em 07/05/2026; Ecovias Minas Goiás DELTA, em 26/07/2024. Duas delas, as da Concebra na BR-153, estão hoje com a Way-153, que tem registro próprio no cadastro.

---

## Divergências declaradas

Divergência registrada é sinal de qualidade, não de erro escondido. Estas são as que esta versão encontrou:

| Onde | O que o cadastro diz | O que adotamos |
|---|---|---|
| Concer, BR-040 | Três praças ativas | Contrato encerrado na Lista de Concessões; as mesmas praças estão ativas sob a Elovias, e entram só por ela |
| Ecovias Sul, BR-116 e BR-392 | Cinco praças ativas | Contrato encerrado na Lista de Concessões; fora da contagem |
| Rodovia do Aço, BR-393 | Três praças ativas | Caducidade declarada na Lista de Concessões e cobrança suspensa desde junho de 2025; fora da contagem |
| Viúva Graça e Viuvinha, Seropédica | As mesmas duas estruturas sob a RioSP (km 207,1 e 208,6) e sob a Ecovias Rio Minas (km 211,674 e 213,103) | Uma vez cada, sob a RioSP, com a divergência na observação da linha |
| Concebra e Way-153, BR-153 | Praças nos mesmos locais, a da Concebra com data de inativação de 22/05/2026 e município diferente | Só a Way-153 |
| Ecovias Cerrado (Paranaiguara) e Ecovias Minas Goiás (Delta) | Situação ativa com data de inativação preenchida | A data de inativação prevalece; fora da contagem |
| Simão Pereira, Elovias, BR-040 | Praça ativa | Praça ativa, com a troca por Free Flow autorizada para 16/11/2026 registrada na observação |
| `tipo_de_pista` | "Principal" em todos os registros, inclusive nas praças auxiliares de Jacarezinho | `tipo` = `bloqueio` nas duas praças auxiliares, que o próprio cadastro localiza no acesso para a SP-278 e na saída para a BR-153 |

---

## Por que aqui não tem tarifa

Tarifa de pedágio muda a cada reajuste de contrato, e cada concessão tem a sua data. Uma base aberta com valor congelado engana mais do que ajuda. Por isso este repositório guarda, para cada praça e cada concessão, o **link da tabela oficial de tarifas** publicada pela ANTT, que está sempre atualizada na origem. Para calcular uma viagem inteira, o [Trace Sua Rota](https://www.semparar.com.br/trace-sua-rota?utm_source=github&utm_medium=metodologia&utm_campaign=sem-parar-pedagios), do Sem Parar, soma as praças do caminho.

---

## Como os arquivos CSV são formatados

- Codificação **UTF-8**, separador **vírgula**, quebra de linha **CRLF** (padrão RFC 4180, que é o que o Excel espera).
- Datas em **ISO** (`AAAA-MM-DD`). Números decimais com **ponto**, como no km `819.379`.
- Listas dentro de uma célula separadas por **ponto e vírgula**.
- Campo não confirmado em fonte oficial aparece como **`n/d`**. Nada é inferido.
- Se o Excel embaralhar os acentos, abra pelo menu **Dados**, opção de importar texto, e escolha **UTF-8**.

---

## Com que frequência isso é atualizado

| Evento | Prazo |
|---|---|
| Praça nova, desativada ou convertida em Free Flow | até 72 horas após o fato confirmado em fonte oficial |
| Mudança de concessionária ou de situação de contrato | até 72 horas após a publicação da ANTT |
| Revisão completa das bases | mensal |

Tudo que muda fica registrado no [CHANGELOG](../CHANGELOG.md).

---

## O que esta base não faz

- Não guarda tarifa, mensalidade ou percentual de desconto.
- Não repete os pórticos de Free Flow, que vivem no [repositório irmão](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW).
- Não cobre ainda as rodovias estaduais e municipais. Elas entram nas próximas versões.
- Não substitui os canais oficiais da ANTT e das concessionárias.

---

## Como citar e reutilizar

O conteúdo e as bases estão sob [CC BY 4.0](../LICENSE): o reuso é livre, inclusive comercial, desde que citada a fonte.

> Sem Parar. *Praças de pedágio do Brasil: base aberta das praças com cabine nas rodovias concedidas.* Versão 0.1.0. Consultado em [data]. Disponível em: https://github.com/Sem-Parar/SEM-PARAR-PEDAGIOS

---

<div align="center">

### Passe direto com a Tag Sem Parar

Com a tag ativa, a cabine fica para trás: a cancela abre na pista automática e a passagem entra na fatura, em todas as rodovias pedagiadas do país.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/pedagios?utm_source=github&utm_medium=metodologia&utm_campaign=sem-parar-pedagios)**

Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

<br>

| Você quer | Vá para |
|---|---|
| Calcular o pedágio e o combustível de uma viagem | [Trace Sua Rota](https://www.semparar.com.br/trace-sua-rota?utm_source=github&utm_medium=metodologia&utm_campaign=sem-parar-pedagios) |
| Pagar uma passagem de Free Flow sem ser cliente | [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=metodologia&utm_campaign=sem-parar-pedagios) |
| Gestão de frota e vale-pedágio | [sempararempresas.com.br](https://www.sempararempresas.com.br?utm_source=github&utm_medium=metodologia&utm_campaign=sem-parar-pedagios) |

<br>

<sub>Repositório oficial mantido pelo <strong>Sem Parar</strong>. Conteúdo e dados sob <a href="../LICENSE">CC BY 4.0</a>. Última revisão dos dados em 9 de novembro de 2026.</sub>

<sub><strong>Você com mais tempo para o que importa.</strong> #TudoProSeuCarro</sub>

</div>
