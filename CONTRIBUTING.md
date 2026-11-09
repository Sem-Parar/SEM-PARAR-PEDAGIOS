# Como contribuir

Este repositório é mantido pelo Sem Parar e existe porque a informação sobre as praças de pedágio do Brasil está espalhada e muda com frequência. **Toda correção é bem-vinda**, inclusive as pequenas: um km errado, um link que quebrou, uma praça que virou Free Flow ontem.

## A regra que vale para tudo: fonte oficial

Toda contribuição precisa vir acompanhada de uma **fonte oficial**, seja a ANTT, uma agência reguladora estadual ou o site da própria concessionária. Notícia de imprensa serve como sinal para investigarmos, mas o dado só entra com confirmação oficial.

## O jeito mais rápido: abrir uma issue

Você não precisa saber Git. [Abra uma issue](../../issues/new) dizendo o que está errado ou o que mudou, e cole o link da fonte oficial. Serve para praça nova, praça desativada, mudança de concessionária, km errado ou link quebrado.

## Se preferir mandar um pull request

1. Faça um fork e crie um branch descritivo, por exemplo `dados/praca-br116-km87`.
2. Edite o CSV direto.
3. Atualize a coluna `atualizado_em` da linha que você mexeu, no formato `AAAA-MM-DD`, e preencha a coluna `fonte` com a URL oficial.
4. Some uma linha ao [CHANGELOG.md](CHANGELOG.md), na seção `[Não publicado]`.
5. Abra o PR explicando o que mudou e por quê.

## Convenções das bases

**Nada de valores.** Não registramos tarifa em reais. Registramos o link da tabela tarifária oficial, que fica sempre atualizada na origem.

**`n/d` em vez de chute.** Campo não confirmado é `n/d`. Nenhum dado deste repositório pode ser inferido, deduzido ou preenchido por analogia.

**Uma linha por praça física.** O critério completo está em [Metodologia e fontes](docs/metodologia-e-fontes.md#o-que-conta-como-uma-praça).

**Pórtico de Free Flow não entra aqui.** Ele vive no repositório [SEM-PARAR-FREE-FLOW](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW).

**Datas em ISO** (`AAAA-MM-DD`) e listas dentro de uma célula separadas por ponto e vírgula. O significado de cada coluna está em [`dados/README.md`](dados/README.md).

## Ritmo de atualização

| Evento | Prazo |
|---|---|
| Praça nova, desativada ou convertida em Free Flow | até 72 horas após o fato confirmado |
| Revisão completa das bases | mensal |

## O que não entra

- Valores de tarifa, mensalidade ou percentual de desconto.
- Dados sem fonte oficial verificável.
- Conteúdo promocional de terceiros.

**Nunca inclua dados pessoais**, como placa, CPF, número de cartão ou print de fatura. Este repositório é público.

## Código de conduta

Ao participar, você concorda com o [Código de Conduta](CODE_OF_CONDUCT.md).
