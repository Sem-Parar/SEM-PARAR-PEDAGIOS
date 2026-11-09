# Praças de pedágio por rodovia: km, sentido e concessionária de cada uma

**As 319 praças de pedágio com cabine desta base estão em 66 rodovias, e a BR-116 lidera com 28.** Abaixo, cada rodovia com as praças na ordem do quilômetro, o município, o sentido cobrado e a concessionária responsável, mais o link da tabela oficial de tarifas. As federais vêm primeiro, pela sigla BR, e as estaduais de São Paulo depois, pela sigla SP.

> Publicado em 9 de novembro de 2026. Gerado a partir de [`dados/pracas-de-pedagio.csv`](dados/pracas-de-pedagio.csv), com o cadastro da ANTT de 3 de novembro de 2026 e o cadastro de ativos da ARTESP de 30 de maio de 2025, conferido contra as passagens de 2026.
> Parte do repositório [Praças de pedágio do Brasil, pelo Sem Parar](README.md). Esta versão cobre as concessões federais e as estaduais de São Paulo; as estaduais dos demais estados e as municipais entram nas próximas.

Onde a rodovia também tem Free Flow, os pórticos ficam no repositório irmão, em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md). Para saber quanto custa uma viagem inteira, use o [Trace Sua Rota](https://www.semparar.com.br/trace-sua-rota?utm_source=github&utm_medium=rodovias&utm_campaign=sem-parar-pedagios).

**Como ler o sentido.** Nas federais, crescente e decrescente seguem a quilometragem da rodovia: crescente é o sentido em que o km aumenta. Nas paulistas, a ARTESP registra o sentido pelo ponto cardeal (norte, sul, leste, oeste) e, no Rodoanel, pela pista interna ou externa. "Ambos" quer dizer que a praça cobra nas duas mãos.

---

## Índice

| Rodovia | Nome popular do trecho | Praças | Estados |
|---|---|:---:|---|
| [BR-040](#br-040) | Rio-Juiz de Fora | 13 | RJ, MG |
| [BR-050](#br-050) |  | 5 | MG, GO |
| [BR-060](#br-060) |  | 2 | GO |
| [BR-080](#br-080) |  | 1 | GO |
| [BR-101](#br-101) | Ponte Rio-Niterói | 22 | RJ, ES, SC, RS |
| [BR-116](#br-116) | Régis Bittencourt, Via Dutra, Rio-Teresópolis, Rio-Bahia | 28 | SP, RJ, MG, PR, SC |
| [BR-153](#br-153) | Transbrasiliana | 15 | SP, MG, GO, TO |
| [BR-163](#br-163) |  | 16 | MS, MT, PA |
| [BR-262](#br-262) |  | 5 | MG |
| [BR-277](#br-277) |  | 10 | PR |
| [BR-290](#br-290) | Freeway | 2 | RS |
| [BR-364](#br-364) |  | 7 | MT, GO |
| [BR-365](#br-365) |  | 4 | MG |
| [BR-369](#br-369) |  | 5 | PR |
| [BR-373](#br-373) |  | 1 | PR |
| [BR-376](#br-376) | Rodovia do Café | 5 | PR |
| [BR-381](#br-381) | Fernão Dias | 8 | SP, MG |
| [BR-386](#br-386) |  | 4 | RS |
| [BR-414](#br-414) |  | 1 | GO |
| [BR-476](#br-476) |  | 1 | PR |
| [BR-493](#br-493) | Arco Metropolitano do Rio | 2 | RJ |
| [SP-021](#sp-021) | Rodoanel Mario Covas | 15 | SP |
| [SP-055](#sp-055) |  | 2 | SP |
| [SP-063](#sp-063) |  | 1 | SP |
| [SP-065](#sp-065) | Dom Pedro I | 3 | SP |
| [SP-070](#sp-070) | Ayrton Senna e Carvalho Pinto | 4 | SP |
| [SP-075](#sp-075) |  | 3 | SP |
| [PR-092](#pr-092) |  | 1 | PR |
| [SP-099](#sp-099) | Tamoios | 2 | SP |
| [SP-101](#sp-101) |  | 2 | SP |
| [SP-127](#sp-127) |  | 5 | SP |
| [SP-147](#sp-147) |  | 3 | SP |
| [SP-150](#sp-150) | Anchieta | 1 | SP |
| [PR-151](#pr-151) |  | 3 | PR |
| [SP-160](#sp-160) | Imigrantes | 4 | SP |
| [SP-191](#sp-191) |  | 2 | SP |
| [SP-215](#sp-215) |  | 2 | SP |
| [SP-225](#sp-225) |  | 5 | SP |
| [SP-255](#sp-255) |  | 7 | SP |
| [SP-258](#sp-258) |  | 2 | SP |
| [SP-270](#sp-270) | Raposo Tavares | 7 | SP |
| [SP-280](#sp-280) | Castello Branco | 9 | SP |
| [SP-284](#sp-284) |  | 2 | SP |
| [SP-293](#sp-293) |  | 1 | SP |
| [SP-294](#sp-294) |  | 7 | SP |
| [SP-300](#sp-300) | Marechal Rondon | 15 | SP |
| [SP-304](#sp-304) |  | 3 | SP |
| [SP-308](#sp-308) |  | 3 | SP |
| [SP-310](#sp-310) | Washington Luís | 5 | SP |
| [PR-317](#pr-317) |  | 1 | PR |
| [SP-318](#sp-318) |  | 1 | SP |
| [SP-322](#sp-322) |  | 2 | SP |
| [PR-323](#pr-323) |  | 1 | PR |
| [SP-326](#sp-326) |  | 1 | SP |
| [SP-327](#sp-327) |  | 1 | SP |
| [SP-330](#sp-330) | Anhanguera | 10 | SP |
| [SP-332](#sp-332) |  | 3 | SP |
| [SP-333](#sp-333) |  | 4 | SP |
| [SP-334](#sp-334) |  | 2 | SP |
| [SP-340](#sp-340) |  | 4 | SP |
| [SP-342](#sp-342) |  | 2 | SP |
| [SP-344](#sp-344) |  | 2 | SP |
| [SP-348](#sp-348) | Bandeirantes | 5 | SP |
| [SP-350](#sp-350) |  | 1 | SP |
| [SP-360](#sp-360) |  | 1 | SP |
| [SP-425](#sp-425) |  | 2 | SP |

---

## BR-040

**13 praças** em RJ, MG: Elovias, 3 praças (Rio-Juiz de Fora); Via Cristais, 7 praças; EPR Via Mineira, 3 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P2 | RJ | Petrópolis | 45,819 | ambos | Elovias |
| P1 | RJ | Duque de Caxias | 101,825 | ambos | Elovias |
| P1 - Paracatu | MG | Paracatu | 17,65 | ambos | Via Cristais |
| P2 - Lagoa Grande | MG | Lagoa Grande | 91,295 | ambos | Via Cristais |
| P3 - João Pinheiro | MG | João Pinheiro | 172,985 | ambos | Via Cristais |
| P4 - São Gonçalo do Abaeté | MG | São Gonçalo do Abaeté | 254,1 | ambos | Via Cristais |
| P5 - Felixlândia | MG | Felixlândia | 328,705 | ambos | Via Cristais |
| P6 - Curvelo | MG | Curvelo | 405,353 | ambos | Via Cristais |
| P7 - Capim Branco | MG | Capim Branco | 487,341 | ambos | Via Cristais |
| P1 - Itabirito | MG | Itabirito | 577,2 | ambos | EPR Via Mineira |
| P2 - Lafaiete | MG | Conselheiro Lafaiete | 642,85 | ambos | EPR Via Mineira |
| P3 - Barbacena | MG | Barbacena | 714,1 | ambos | EPR Via Mineira |
| P3 | MG | Simão Pereira | 819,379 | ambos | Elovias |

Tabela oficial de tarifas: [Elovias](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/elovias/tarifas-de-pedagio); [Via Cristais](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/via-cristais/revisoes-e-reajustes/tarifas-de-pedagio); [EPR Via Mineira](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/epr-via-mineira/tarifas-de-pedagios-via-mineira).

**Free Flow nas concessões desta rodovia:** Elovias, anunciado. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## BR-050

**5 praças** em MG, GO: Ecovias Minas Goiás, 5 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| ARAGUARI I | MG | Araguari | 13,94 | ambos | Ecovias Minas Goiás |
| ARAGUARI II | MG | Araguari | 51,5 | ambos | Ecovias Minas Goiás |
| UBERABA | MG | Uberaba | 104,98 | ambos | Ecovias Minas Goiás |
| IPAMERI | GO | Ipameri | 144 | ambos | Ecovias Minas Goiás |
| CAMPO ALEGRE | GO | Campo Alegre de Goiás | 226 | ambos | Ecovias Minas Goiás |

Tabela oficial de tarifas: [Ecovias Minas Goiás](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/eco050/tarifas-de-pedagio).

---

## BR-060

**2 praças** em GO: Concebra, 2 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P1 ALEXÂNIA | GO | Alexânia | 43,1 | ambos | Concebra |
| P2 GOIANÁPOLIS | GO | Goianápolis | 107,9 | ambos | Concebra |

Tabela oficial de tarifas: [Concebra](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/concebra/tarifas-de-pedagio).

---

## BR-080

**1 praça** em GO: Ecovias Araguaia, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P8 - Santa Rita do Novo Destino | GO | Santa Rita do Novo Destino | 155,5 | ambos | Ecovias Araguaia |

Tabela oficial de tarifas: [Ecovias Araguaia](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/ecovias-araguaia/tarifas-de-pedagio).

---

## BR-101

**22 praças** em RJ, ES, SC, RS: Autopista Fluminense, 5 praças; Ecovias Ponte, 1 praça (Ponte Rio-Niterói); Ecovias Capixaba, 7 praças; Autopista Litoral Sul, 4 praças; ViaCosteira, 4 praças; ViaSul, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Conselheiro Josino | RJ | Campos dos Goytacazes | 40,5 | ambos | Autopista Fluminense |
| Serrinha | RJ | Campos dos Goytacazes | 123,07 | ambos | Autopista Fluminense |
| Casimiro de Abreu | RJ | Casimiro de Abreu | 192,82 | ambos | Autopista Fluminense |
| Rio Bonito | RJ | Rio Bonito | 252,85 | ambos | Autopista Fluminense |
| São Gonçalo | RJ | São Gonçalo | 299,69 | só crescente | Autopista Fluminense |
| NITEROÍ-1 | RJ | Niterói | 322,23 | só decrescente | Ecovias Ponte |
| P1 - Pedro Canário | ES | Pedro Canário | 1 | ambos | Ecovias Capixaba |
| P2 - São Mateus | ES | São Mateus | 85,8 | ambos | Ecovias Capixaba |
| P3 - Aracruz | ES | Aracruz | 171,7 | ambos | Ecovias Capixaba |
| P4 - Serra | ES | Serra | 242 | ambos | Ecovias Capixaba |
| P5 - Guarapari | ES | Guarapari | 320,8 | ambos | Ecovias Capixaba |
| P6 - Itapemirim | ES | Itapemirim | 398,9 | ambos | Ecovias Capixaba |
| P7 - Mimoso do Sul | ES | Mimoso do Sul | 452 | ambos | Ecovias Capixaba |
| P2 | SC | Garuva | 1,35 | ambos | Autopista Litoral Sul |
| P3 | SC | Araquari | 79,3 | ambos | Autopista Litoral Sul |
| P4 | SC | Porto Belo | 157,4 | ambos | Autopista Litoral Sul |
| P5 | SC | Palhoça | 242,8 | ambos | Autopista Litoral Sul |
| P1-Laguna | SC | Laguna | 298,66 | ambos | ViaCosteira |
| P2-Tubarão | SC | Tubarão | 344,7 | ambos | ViaCosteira |
| P3-Araranguá | SC | Maracajá | 404,55 | ambos | ViaCosteira |
| P4-São João do Sul | SC | São João do Sul | 457,53 | ambos | ViaCosteira |
| P1-Três Cachoeiras | RS | Três Cachoeiras | 35,2 | ambos | ViaSul |

Tabela oficial de tarifas: [Autopista Fluminense](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/autopista-fluminense/tarifas-de-pedagio); [Ecovias Ponte](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/ecoponte/tarifas-de-pedagio); [Ecovias Capixaba](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/ecovias-capixaba/tarifas-de-pedagio); [Autopista Litoral Sul](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/autopista-litoral-sul/tarifas-de-pedagios); [ViaCosteira](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/ccr-viacosteira/tarifas-de-pedagio); [ViaSul](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/viasul/tarifas-de-pedagio).

**Free Flow nas concessões desta rodovia:** Autopista Fluminense, previsto; ViaSul, previsto. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## BR-116

**28 praças** em SP, RJ, MG, PR, SC: RioSP, 9 praças (Via Dutra); Autopista Régis Bittencourt, 6 praças (Régis Bittencourt); Ecovias Rio Minas, 8 praças (Rio-Teresópolis, Rio-Bahia); Autopista Planalto Sul, 5 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Moreira César | SP | Pindamonhangaba | 87 | ambos | RioSP |
| Jacareí | SP | Jacareí | 165,1 | ambos | RioSP |
| Guararema Sul | SP | Guararema | 180,7 | só crescente | RioSP |
| Guararema Norte | SP | Santa Isabel | 182,4 | só decrescente | RioSP |
| Arujá | SP | Arujá | 204,3 | ambos | RioSP |
| Arujá Rodoanel | SP | Arujá | 204,8 | só decrescente | RioSP |
| São Lourenço da Serra | SP | São Lourenço da Serra | 298,8 | ambos | Autopista Régis Bittencourt |
| Miracatu | SP | Miracatu | 370,4 | ambos | Autopista Régis Bittencourt |
| Juquiá | SP | Juquiá | 426,6 | ambos | Autopista Régis Bittencourt |
| Cajati | SP | Cajati | 485,7 | ambos | Autopista Régis Bittencourt |
| Barra do Turvo | SP | Barra do Turvo | 542,9 | ambos | Autopista Régis Bittencourt |
| P07 Magé | RJ | Magé | 118,2 | ambos | Ecovias Rio Minas |
| Viúva Graça Norte | RJ | Seropédica | 207,1 | só decrescente | RioSP |
| Viuvinha Norte | RJ | Seropédica | 208,6 | só decrescente | RioSP |
| Itatiaia | RJ | Itatiaia | 324,8 | ambos | RioSP |
| P15 Engenheiro Caldas | MG | Engenheiro Caldas | 433,6 | ambos | Ecovias Rio Minas |
| P14 Inhapim | MG | Inhapim | 488,7 | ambos | Ecovias Rio Minas |
| P13 Santa Bárbara do Leste | MG | Santa Bárbara do Leste | 551,88 | ambos | Ecovias Rio Minas |
| P12 São João do Manhuaçu | MG | São João do Manhuaçu | 610,94 | ambos | Ecovias Rio Minas |
| P11 São Francisco do Glória | MG | São Francisco do Glória | 664 | ambos | Ecovias Rio Minas |
| P10 Laranjal | MG | Laranjal | 724,02 | ambos | Ecovias Rio Minas |
| P09 Leopoldina | MG | Leopoldina | 784,32 | ambos | Ecovias Rio Minas |
| Campina Grande do Sul | PR | Campina Grande do Sul | 57,1 | ambos | Autopista Régis Bittencourt |
| FAZENDA RIO GRANDE | PR | Fazenda Rio Grande | 134,4 | ambos | Autopista Planalto Sul |
| RIO NEGRO | PR | Rio Negro | 204,1 | ambos | Autopista Planalto Sul |
| MONTE CASTELO | SC | Monte Castelo | 81,6 | ambos | Autopista Planalto Sul |
| SANTA CECÍLIA | SC | Santa Cecília | 152 | ambos | Autopista Planalto Sul |
| CORREIA PINTO | SC | Correia Pinto | 233,16 | ambos | Autopista Planalto Sul |

Tabela oficial de tarifas: [RioSP](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/ccr-rio-sp/tarifas-de-pedagio); [Autopista Régis Bittencourt](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/autopista-regis-bittencourt/tarifas-de-pedagio); [Ecovias Rio Minas](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/ecoriominas/revisoes-e-reajustes/tarifas-de-pedagios); [Autopista Planalto Sul](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/autopista-planalto-sul/tarifas-de-pedagio-autopista-planalto-sul).

**Free Flow nas concessões desta rodovia:** RioSP, sim; Ecovias Rio Minas, previsto. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## BR-153

**15 praças** em SP, MG, GO, TO: Transbrasiliana, 4 praças (Transbrasiliana); Way-153, 4 praças; Ecovias Araguaia, 7 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P 01 | SP | Onda Verde | 35,8 | ambos | Transbrasiliana |
| P 02 | SP | José Bonifácio | 98,9 | ambos | Transbrasiliana |
| P 03 | SP | Lins | 183,8 | ambos | Transbrasiliana |
| P 04 | SP | Vera Cruz | 268,1 | ambos | Transbrasiliana |
| Praça 03 - Prata | MG | Prata | 128,49 | ambos | Way-153 |
| Praça 04 - Fronteira | MG | Fronteira | 225,83 | ambos | Way-153 |
| P3 - Porangatu | GO | Porangatu | 12,5 | ambos | Ecovias Araguaia |
| P4 - Estrela do Norte | GO | Estrela do Norte | 116,12 | ambos | Ecovias Araguaia |
| P5 - Campinorte | GO | Campinorte | 182,04 | ambos | Ecovias Araguaia |
| P6 - Hidrolina | GO | Hidrolina | 233,4 | ambos | Ecovias Araguaia |
| P7 - Jaraguá | GO | Jaraguá | 367,5 | ambos | Ecovias Araguaia |
| Praça 01 - Piracanjuba | GO | Professor Jamil | 553,265 | ambos | Way-153 |
| Praça 02 - Itumbiara | GO | Itumbiara | 685,39 | ambos | Way-153 |
| P1 - Aliança do Tocantins | TO | Aliança do Tocantins | 640 | ambos | Ecovias Araguaia |
| P2 - Alvorada | TO | Alvorada | 744,91 | ambos | Ecovias Araguaia |

Tabela oficial de tarifas: [Transbrasiliana](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/Transbrasiliana/tarifas-de-pedagio); [Way-153](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/rota-sertaneja/tarifas-de-pedagio); [Ecovias Araguaia](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/ecovias-araguaia/tarifas-de-pedagio).

---

## BR-163

**16 praças** em MS, MT, PA: Motiva Pantanal, 9 praças; Nova Rota do Oeste, 4 praças; Via Brasil BR-163, 3 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P1-Mundo Novo | MS | Mundo Novo | 28,2 | ambos | Motiva Pantanal |
| P2-Itaquirai | MS | Itaquiraí | 113 | ambos | Motiva Pantanal |
| P3-Caarapó | MS | Caarapó | 228,2 | ambos | Motiva Pantanal |
| P4-Rio Brilhante | MS | Rio Brilhante | 313,5 | ambos | Motiva Pantanal |
| P5-Campo Grande | MS | Campo Grande | 431,8 | ambos | Motiva Pantanal |
| P6-Jaraguari | MS | Jaraguari | 533,8 | ambos | Motiva Pantanal |
| P7-São Gabriel | MS | São Gabriel do Oeste | 605 | ambos | Motiva Pantanal |
| P8-Rio Verde | MS | Rio Verde de Mato Grosso | 704,3 | ambos | Motiva Pantanal |
| P9-Sonora | MS | Sonora | 819,2 | ambos | Motiva Pantanal |
| P1 | MT | Itiquira | 33,6 | ambos | Nova Rota do Oeste |
| P7 | MT | Nova Mutum | 586,9 | ambos | Nova Rota do Oeste |
| P8 | MT | Lucas do Rio Verde | 664,45 | ambos | Nova Rota do Oeste |
| P9 | MT | Sorriso | 766,7 | ambos | Nova Rota do Oeste |
| P1 - Claúdia | MT | Cláudia | 897 | ambos | Via Brasil BR-163 |
| P2 - Guarantã do Norte | MT | Terra Nova do Norte | 1089,45 | ambos | Via Brasil BR-163 |
| P3 - Trairão | PA | Trairão | 636,015 | ambos | Via Brasil BR-163 |

Tabela oficial de tarifas: [Motiva Pantanal](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/motiva-pantanal/tarifas-de-pedagio); [Nova Rota do Oeste](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/rota-do-oeste/tarifas-de-pedagio); [Via Brasil BR-163](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/via-brasil/tarifas-de-pedagio).

---

## BR-262

**5 praças** em MG: Way-262, 4 praças; Way-153, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Praça 01 - Florestal | MG | Florestal | 384,78 | ambos | Way-262 |
| Praça 03 - Luz | MG | Luz | 505,4 | ambos | Way-262 |
| Praça 04 - Campos Altos | MG | Campos Altos | 591,8 | ambos | Way-262 |
| Praça 06 - Perdizes | MG | Perdizes | 721,63 | ambos | Way-262 |
| Praça 05 - Campo Florido | MG | Conceição das Alagoas | 853,19 | ambos | Way-153 |

Tabela oficial de tarifas: [Way-262](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/way-262/tarifas-de-pedagio); [Way-153](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/rota-sertaneja/tarifas-de-pedagio).

**Free Flow nas concessões desta rodovia:** Way-262, sim. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## BR-277

**10 praças** em PR: EPR Litoral Pioneiro, 1 praça; Via Araucária, 3 praças; EPR Iguaçu, 6 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P01 SÃO JOSÉ DOS PINHAIS | PR | São José dos Pinhais | 60,25 | ambos | EPR Litoral Pioneiro |
| P01 São Luiz do Purunã | PR | Balsa Nova | 140 | ambos | Via Araucária |
| P02 Porto Amazonas | PR | Porto Amazonas | 165,7 | ambos | Via Araucária |
| P03 Irati | PR | Irati | 256,1 | ambos | Via Araucária |
| P02 PRUDENTROPOLIS | PR | Prudentópolis | 308,29 | ambos | EPR Iguaçu |
| P03 CANDOI | PR | Candói | 393,04 | ambos | EPR Iguaçu |
| P04 LARANJEIRAS DO SUL | PR | Laranjeiras do Sul | 468,11 | ambos | EPR Iguaçu |
| P05 CASCAVEL | PR | Cascavel | 571,34 | ambos | EPR Iguaçu |
| P06 CÉU AZUL | PR | Céu Azul | 615,34 | ambos | EPR Iguaçu |
| P07 SÃO MIQUEL DO IGUAÇU | PR | São Miguel do Iguaçu | 706,07 | ambos | EPR Iguaçu |

Tabela oficial de tarifas: [EPR Litoral Pioneiro](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/epr-litoral-pioneiro/tarifas-de-pedagio); [Via Araucária](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/via-araucaria/tarifas-de-pedagio); [EPR Iguaçu](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/epr-iguacu/tarifas-de-pedagio).

**Free Flow nas concessões desta rodovia:** EPR Litoral Pioneiro, previsto; EPR Iguaçu, sim. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## BR-290

**2 praças** em RS: ViaSul, 2 praças (Freeway).

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P2-Santo Antônio da Patrulha | RS | Santo Antônio da Patrulha | 19,4 | ambos | ViaSul |
| P3-Gravatai | RS | Gravataí | 60 | ambos | ViaSul |

Tabela oficial de tarifas: [ViaSul](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/viasul/tarifas-de-pedagio).

**Free Flow nas concessões desta rodovia:** ViaSul, previsto. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## BR-364

**7 praças** em MT, GO: Nova Rota do Oeste, 5 praças; Ecovias Cerrado, 2 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P2 | MT | Rondonópolis | 214,4 | ambos | Nova Rota do Oeste |
| P3 | MT | Campo Verde | 316,55 | ambos | Nova Rota do Oeste |
| P4 | MT | Santo Antônio de Leverger | 383,1 | ambos | Nova Rota do Oeste |
| P5 | MT | Jangada | 479,1 | ambos | Nova Rota do Oeste |
| P6 | MT | Nobres | 579,1 | ambos | Nova Rota do Oeste |
| P6 - CACHOEIRA ALTA | GO | Cachoeira Alta | 92,85 | ambos | Ecovias Cerrado |
| P7 - JATAÍ | GO | Jataí | 156,18 | ambos | Ecovias Cerrado |

Tabela oficial de tarifas: [Nova Rota do Oeste](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/rota-do-oeste/tarifas-de-pedagio); [Ecovias Cerrado](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/ecovias-do-cerrado/tarifas-de-pedagio).

---

## BR-365

**4 praças** em MG: Ecovias Cerrado, 4 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P1 - UBERLÂNDIA | MG | Uberlândia | 646 | ambos | Ecovias Cerrado |
| P2 - MONTE ALEGRE | MG | Monte Alegre de Minas | 704,12 | ambos | Ecovias Cerrado |
| P3 - ITUIUTABA | MG | Ituiutaba | 765,37 | ambos | Ecovias Cerrado |
| P4 - SANTA VITÓRIA | MG | Santa Vitória | 834,45 | ambos | Ecovias Cerrado |

Tabela oficial de tarifas: [Ecovias Cerrado](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/ecovias-do-cerrado/tarifas-de-pedagio).

---

## BR-369

**5 praças** em PR: EPR Litoral Pioneiro, 3 praças; Via Campo, 2 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P03 JACAREZINHO | PR | Jacarezinho | 1,4 | ambos | EPR Litoral Pioneiro |
| P08 JACAREZINHO AUX I | PR | Jacarezinho | 1,653 | ambos | EPR Litoral Pioneiro |
| P09 JACAREZINHO AUX II | PR | Jacarezinho | 1,698 | ambos | EPR Litoral Pioneiro |
| P02 - Mamborê | PR | Campo Mourão | 363 | ambos | Via Campo |
| P03 - Corbélia | PR | Corbélia | 479 | ambos | Via Campo |

Tabela oficial de tarifas: [EPR Litoral Pioneiro](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/epr-litoral-pioneiro/tarifas-de-pedagio); [Via Campo](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/via-campos/tarifa-de-pedagio/tarifas-de-pedagio).

**Free Flow nas concessões desta rodovia:** EPR Litoral Pioneiro, previsto; Via Campo, adiado. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## BR-373

**1 praça** em PR: Via Araucária, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P04 Imbituva | PR | Imbituva | 216 | ambos | Via Araucária |

Tabela oficial de tarifas: [Via Araucária](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/via-araucaria/tarifas-de-pedagio).

---

## BR-376

**5 praças** em PR: Motiva Paraná, 4 praças (Rodovia do Café); Autopista Litoral Sul, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P03 ORTIGUEIRA | PR | Ortigueira | 316,35 | ambos | Motiva Paraná |
| P04 IMBAÚ | PR | Ortigueira | 370,95 | ambos | Motiva Paraná |
| P05 TIBAGI | PR | Tibagi | 448,55 | ambos | Motiva Paraná |
| P06 WITMARSUM | PR | Palmeira | 529,85 | ambos | Motiva Paraná |
| P1 | PR | São José dos Pinhais | 635,3 | ambos | Autopista Litoral Sul |

Tabela oficial de tarifas: [Motiva Paraná](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/pr-vias/tarifas-de-pedagio); [Autopista Litoral Sul](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/autopista-litoral-sul/tarifas-de-pedagios).

**Free Flow nas concessões desta rodovia:** Motiva Paraná, sim. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## BR-381

**8 praças** em SP, MG: Motiva Minas SP, 8 praças (Fernão Dias).

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| 2 (Vargem) | SP | Vargem | 7,3 | ambos | Motiva Minas SP |
| 1 (Mairiporã) | SP | Mairiporã | 65,7 | ambos | Motiva Minas SP |
| 8 (Itatiaiuçu) | MG | Itatiaiuçu | 545,9 | ambos | Motiva Minas SP |
| 7 (Carmópolis de Minas) | MG | Carmópolis de Minas | 597,7 | ambos | Motiva Minas SP |
| 6 (Santo Antônio do Amparo) | MG | Santo Antônio do Amparo | 658,3 | ambos | Motiva Minas SP |
| 5 (Carmo da Cachoeira) | MG | Carmo da Cachoeira | 735,5 | ambos | Motiva Minas SP |
| 4 (São Gonçalo) | MG | São Gonçalo do Sapucaí | 805,2 | ambos | Motiva Minas SP |
| 3 (Cambuí) | MG | Cambuí | 900,9 | ambos | Motiva Minas SP |

Tabela oficial de tarifas: [Motiva Minas SP](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/motiva-minas-sp/tarifas-de-pedagio).

---

## BR-386

**4 praças** em RS: ViaSul, 4 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P7-Victor Graeff | RS | Victor Graeff | 204,4 | ambos | ViaSul |
| P6-Fontoura Xavier | RS | Fontoura Xavier | 262,7 | ambos | ViaSul |
| P5-Paverama | RS | Paverama | 375,8 | ambos | ViaSul |
| P4-Montenegro | RS | Montenegro | 426 | ambos | ViaSul |

Tabela oficial de tarifas: [ViaSul](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/viasul/tarifas-de-pedagio).

**Free Flow nas concessões desta rodovia:** ViaSul, previsto. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## BR-414

**1 praça** em GO: Ecovias Araguaia, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P9 - Corumbá de Goiás | GO | Corumbá de Goiás | 404,08 | ambos | Ecovias Araguaia |

Tabela oficial de tarifas: [Ecovias Araguaia](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/ecovias-araguaia/tarifas-de-pedagio).

---

## BR-476

**1 praça** em PR: Via Araucária, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P05 Lapa | PR | Lapa | 191,42 | ambos | Via Araucária |

Tabela oficial de tarifas: [Via Araucária](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/via-araucaria/tarifas-de-pedagio).

---

## BR-493

**2 praças** em RJ: Ecovias Rio Minas, 2 praças (Arco Metropolitano do Rio).

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P08 Guapimirim | RJ | Guapimirim | 13,86 | ambos | Ecovias Rio Minas |
| P06 Itaguaí | RJ | Itaguaí | 112,7 | ambos | Ecovias Rio Minas |

Tabela oficial de tarifas: [Ecovias Rio Minas](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/ecoriominas/revisoes-e-reajustes/tarifas-de-pedagios).

**Free Flow nas concessões desta rodovia:** Ecovias Rio Minas, previsto. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## SP-021

**15 praças** em SP: RodoAnel Oeste, 8 praças (Rodoanel Mario Covas); SPMar, 7 praças (Rodoanel Mario Covas).

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Raimundo Pereira de Magalhães | SP | São Paulo | 0,36 | só pista interna | RodoAnel Oeste |
| Bandeirantes | SP | São Paulo | 3,63 | ambos | RodoAnel Oeste |
| Anhanguera | SP | São Paulo | 7 | ambos | RodoAnel Oeste |
| Castello Branco, pista externa | SP | Barueri | 14,29 | só pista externa | RodoAnel Oeste |
| Castello Branco, pista interna | SP | Carapicuíba | 15,61 | só pista interna | RodoAnel Oeste |
| Padroeira | SP | Carapicuíba | 20,87 | ambos | RodoAnel Oeste |
| Raposo Tavares | SP | Osasco | 24,7 | ambos | RodoAnel Oeste |
| Régis Bittencourt | SP | Osasco | 25,36 | só pista externa | RodoAnel Oeste |
| Parelheiros | SP | São Paulo | 50 | só pista interna | SPMar |
| Imigrantes | SP | São Bernardo do Campo | 70 | ambos | SPMar |
| Anchieta | SP | São Bernardo do Campo | 75 | só pista interna | SPMar |
| Interligação Sul-Leste | SP | Ribeirão Pires | 86 | ambos | SPMar |
| Ribeirão Pires | SP | Ribeirão Pires | 87 | ambos | SPMar |
| Ayrton Senna | SP | Itaquaquecetuba | 123 | ambos | SPMar |
| Dutra | SP | Itaquaquecetuba | 127 | só pista externa | SPMar |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-055

**2 praças** em SP: Ecovias dos Imigrantes, 2 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Santos | SP | Santos | 250,464 | só oeste | Ecovias dos Imigrantes |
| São Vicente | SP | São Vicente | 279,95 | só leste | Ecovias dos Imigrantes |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

**Free Flow nas concessões desta rodovia:** Ecovias dos Imigrantes, adiado. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## SP-063

**1 praça** em SP: Rota das Bandeiras, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Louveira | SP | Itatiba | 10,4 | ambos | Rota das Bandeiras |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-065

**3 praças** em SP: Rota das Bandeiras, 3 praças (Dom Pedro I).

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Igaratá | SP | Igaratá | 22,3 | ambos | Rota das Bandeiras |
| Atibaia | SP | Atibaia | 79,9 | ambos | Rota das Bandeiras |
| Itatiba | SP | Itatiba | 110,1 | ambos | Rota das Bandeiras |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-070

**4 praças** em SP: Ecovias Leste Paulista, 4 praças (Ayrton Senna e Carvalho Pinto).

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Itaquaquecetuba | SP | Itaquaquecetuba | 32,9 | ambos | Ecovias Leste Paulista |
| Guararema | SP | Guararema | 57,8 | ambos | Ecovias Leste Paulista |
| São José dos Campos | SP | São José dos Campos | 92,5 | ambos | Ecovias Leste Paulista |
| Caçapava | SP | Caçapava | 114 | ambos | Ecovias Leste Paulista |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-075

**3 praças** em SP: Motiva Sorocabana, 1 praça; Via Colinas, 2 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Sorocaba | SP | Itu | 12,5 | só sul | Motiva Sorocabana |
| Indaiatuba | SP | Indaiatuba | 60,8 | ambos | Via Colinas |
| Indaiatuba (bloqueio) | SP | Indaiatuba | 62 | ambos | Via Colinas |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

**Free Flow nas concessões desta rodovia:** Motiva Sorocabana, sim. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## PR-092

**1 praça** em PR: EPR Litoral Pioneiro, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P07 QUATIGUÁ | PR | Siqueira Campos | 286,74 | ambos | EPR Litoral Pioneiro |

Tabela oficial de tarifas: [EPR Litoral Pioneiro](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/epr-litoral-pioneiro/tarifas-de-pedagio).

**Free Flow nas concessões desta rodovia:** EPR Litoral Pioneiro, previsto. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## SP-099

**2 praças** em SP: Tamoios, 2 praças (Tamoios).

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Jambeiro | SP | Jambeiro | 16,1 | ambos | Tamoios |
| Paraibuna | SP | Paraibuna | 59,3 | ambos | Tamoios |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

**Free Flow nas concessões desta rodovia:** Tamoios, sim. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## SP-101

**2 praças** em SP: Rodovias do Tietê, 2 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Monte Mor | SP | Monte Mor | 29,72 | ambos | Rodovias do Tietê |
| Rafard | SP | Rafard | 55,8 | ambos | Rodovias do Tietê |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-127

**5 praças** em SP: Via Colinas, 2 praças; SPVias, 3 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Rio Claro | SP | Piracicaba | 12,63 | ambos | Via Colinas |
| Rio das Pedras | SP | Rio das Pedras | 58,6 | ambos | Via Colinas |
| Morro do Alto Norte | SP | Tatuí | 128,9 | só norte | SPVias |
| Morro do Alto Sul | SP | Itapetininga | 133,9 | só sul | SPVias |
| Gramadão | SP | Capão Bonito | 196,725 | ambos | SPVias |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-147

**3 praças** em SP: Arteris Intervias, 3 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Mogi Mirim | SP | Mogi Mirim | 52 | ambos | Arteris Intervias |
| Engenheiro Coelho | SP | Limeira | 91,3 | ambos | Arteris Intervias |
| Iracemápolis | SP | Iracemápolis | 127,2 | ambos | Arteris Intervias |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-150

**1 praça** em SP: Ecovias dos Imigrantes, 1 praça (Anchieta).

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Riacho Grande | SP | São Bernardo do Campo | 31,106 | só sul | Ecovias dos Imigrantes |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

**Free Flow nas concessões desta rodovia:** Ecovias dos Imigrantes, adiado. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## PR-151

**3 praças** em PR: EPR Litoral Pioneiro, 3 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P02 SENGES | PR | Sengés | 187,7 | ambos | EPR Litoral Pioneiro |
| P06 JAGUARIAÍVA | PR | Jaguariaíva | 223,1 | ambos | EPR Litoral Pioneiro |
| P05 CARAMBEÍ | PR | Carambeí | 304,25 | ambos | EPR Litoral Pioneiro |

Tabela oficial de tarifas: [EPR Litoral Pioneiro](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/epr-litoral-pioneiro/tarifas-de-pedagio).

**Free Flow nas concessões desta rodovia:** EPR Litoral Pioneiro, previsto. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## SP-160

**4 praças** em SP: Ecovias dos Imigrantes, 4 praças (Imigrantes).

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Diadema (bloqueio) | SP | Diadema | 15,917 | só sul | Ecovias dos Imigrantes |
| Eldorado (bloqueio) | SP | Diadema | 20,1 | só sul | Ecovias dos Imigrantes |
| Batistini (bloqueio) | SP | São Bernardo do Campo | 24,255 | só sul | Ecovias dos Imigrantes |
| Piratininga | SP | São Bernardo do Campo | 32,381 | só sul | Ecovias dos Imigrantes |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

**Free Flow nas concessões desta rodovia:** Ecovias dos Imigrantes, adiado. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## SP-191

**2 praças** em SP: Arteris Intervias, 2 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Araras | SP | Araras | 27,5 | ambos | Arteris Intervias |
| Rio Claro | SP | Rio Claro | 59 | ambos | Arteris Intervias |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-215

**2 praças** em SP: Arteris Intervias, 2 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Santa Cruz das Palmeiras | SP | Santa Cruz das Palmeiras | 65,55 | ambos | Arteris Intervias |
| Descalvado | SP | Descalvado | 104,4 | ambos | Arteris Intervias |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-225

**5 praças** em SP: Eixo SP, 3 praças; CART, 2 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Brotas | SP | Itirapina | 106,9 | ambos | Eixo SP |
| Dois Córregos | SP | Brotas | 143,8 | ambos | Eixo SP |
| Jaú | SP | Jaú | 199,4 | ambos | Eixo SP |
| Piratininga | SP | Piratininga | 251,9 | ambos | CART |
| Santa Cruz do Rio Pardo | SP | Santa Cruz do Rio Pardo | 300,93 | ambos | CART |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-255

**7 praças** em SP: Arteris ViaPaulista, 6 praças; SPVias, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Guatapará | SP | Guatapará | 45,5 | ambos | Arteris ViaPaulista |
| Boa Esperança do Sul | SP | Boa Esperança do Sul | 117,22 | ambos | Arteris ViaPaulista |
| Jaú | SP | Jaú | 165,6 | ambos | Arteris ViaPaulista |
| Botucatu | SP | Botucatu | 229,04 | ambos | Arteris ViaPaulista |
| Avaré | SP | Avaré | 240,3 | ambos | SPVias |
| Itaí | SP | Itaí | 306 | ambos | Arteris ViaPaulista |
| Coronel Macedo | SP | Coronel Macedo | 331,5 | ambos | Arteris ViaPaulista |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-258

**2 praças** em SP: SPVias, 2 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Buri | SP | Taquarivaí | 250,145 | ambos | SPVias |
| Itararé | SP | Itararé | 326,637 | ambos | SPVias |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-270

**7 praças** em SP: SPVias, 1 praça (Raposo Tavares); CART, 6 praças (Raposo Tavares).

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Alambari | SP | Sarapuí | 135,3 | ambos | SPVias |
| Palmital | SP | Palmital | 413,49 | ambos | CART |
| Assis | SP | Assis | 453,59 | ambos | CART |
| Rancharia | SP | Rancharia | 512,3 | ambos | CART |
| Regente Feijó | SP | Regente Feijó | 541,54 | ambos | CART |
| Presidente Bernardes | SP | Presidente Bernardes | 590,4 | ambos | CART |
| Caiuá | SP | Caiuá | 639 | ambos | CART |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-280

**9 praças** em SP: Ecovias Raposo Castello, 3 praças (Castello Branco); Motiva Sorocabana, 1 praça (Castello Branco); Via Colinas, 2 praças (Castello Branco); SPVias, 3 praças (Castello Branco).

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Osasco | SP | Osasco | 18,92 | só oeste | Ecovias Raposo Castello |
| Barueri | SP | Barueri | 20,454 | só leste | Ecovias Raposo Castello |
| Itapevi | SP | Itapevi | 33,42 | só oeste | Ecovias Raposo Castello |
| Itu | SP | Itu | 74 | só leste | Motiva Sorocabana |
| Boituva (bloqueio) | SP | Boituva | 110,8 | ambos | Via Colinas |
| Boituva | SP | Boituva | 111,6 | ambos | Via Colinas |
| Quadra | SP | Quadra | 158,3 | ambos | SPVias |
| Itatinga | SP | Itatinga | 208,4 | ambos | SPVias |
| Iaras | SP | Iaras | 278 | ambos | SPVias |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

**Free Flow nas concessões desta rodovia:** Ecovias Raposo Castello, previsto; Motiva Sorocabana, sim. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## SP-284

**2 praças** em SP: Eixo SP, 2 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Paraguaçu Paulista | SP | Paraguaçu Paulista | 458,3 | ambos | Eixo SP |
| Rancharia | SP | Rancharia | 531,2 | ambos | Eixo SP |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-293

**1 praça** em SP: Eixo SP, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Cabrália Paulista | SP | Cabrália Paulista | 2 | ambos | Eixo SP |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-294

**7 praças** em SP: Eixo SP, 7 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Piratininga | SP | Bauru | 370 | ambos | Eixo SP |
| Garça | SP | Garça | 425,7 | ambos | Eixo SP |
| Oriente | SP | Oriente | 474,8 | ambos | Eixo SP |
| Parapuã | SP | Parapuã | 551,5 | ambos | Eixo SP |
| Inúbia Paulista | SP | Inúbia Paulista | 581,7 | ambos | Eixo SP |
| Pacaembu | SP | Pacaembu | 623,1 | ambos | Eixo SP |
| Santa Mercedes | SP | Santa Mercedes | 670,8 | ambos | Eixo SP |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-300

**15 praças** em SP: Via Colinas, 2 praças (Marechal Rondon); Rodovias do Tietê, 5 praças (Marechal Rondon); ViaRondon, 8 praças (Marechal Rondon).

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Itupeva | SP | Itupeva | 76,68 | ambos | Via Colinas |
| Porto Feliz | SP | Porto Feliz | 136,722 | ambos | Via Colinas |
| Conchas | SP | Conchas | 192,1 | ambos | Rodovias do Tietê |
| Anhembi | SP | Anhembi | 228,2 | ambos | Rodovias do Tietê |
| Botucatu | SP | Botucatu | 259,3 | ambos | Rodovias do Tietê |
| Areiópolis | SP | Areiópolis | 285 | ambos | Rodovias do Tietê |
| Agudos | SP | Lençóis Paulista | 314 | ambos | Rodovias do Tietê |
| Avaí | SP | Avaí | 367,767 | ambos | ViaRondon |
| Pirajuí | SP | Pirajuí | 400,833 | ambos | ViaRondon |
| Promissão | SP | Promissão | 455,715 | ambos | ViaRondon |
| Glicério | SP | Glicério | 497,912 | ambos | ViaRondon |
| Rubiácea | SP | Rubiácea | 562,008 | ambos | ViaRondon |
| Lavínia | SP | Lavínia | 590,482 | ambos | ViaRondon |
| Guaraçaí | SP | Guaraçaí | 621,27 | ambos | ViaRondon |
| Castilho | SP | Castilho | 655,485 | ambos | ViaRondon |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-304

**3 praças** em SP: Eixo SP, 3 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| São Pedro I | SP | São Pedro | 183,4 | ambos | Eixo SP |
| São Pedro II | SP | São Pedro | 215,1 | ambos | Eixo SP |
| Torrinha | SP | Torrinha | 255,8 | ambos | Eixo SP |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-308

**3 praças** em SP: Rodovias do Tietê, 2 praças; Eixo SP, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Salto | SP | Elias Fausto | 109,3 | ambos | Rodovias do Tietê |
| Rio das Pedras | SP | Rio das Pedras | 147,3 | ambos | Rodovias do Tietê |
| Piracicaba | SP | Piracicaba | 182,25 | ambos | Eixo SP |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-310

**5 praças** em SP: Eixo SP, 2 praças (Washington Luís); Ecovias Noroeste Paulista, 3 praças (Washington Luís).

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Rio Claro | SP | Rio Claro | 181,3 | ambos | Eixo SP |
| Itirapina | SP | São Carlos | 217 | ambos | Eixo SP |
| Araraquara | SP | Araraquara | 282,4 | ambos | Ecovias Noroeste Paulista |
| Agulha | SP | Fernando Prestes | 346,404 | ambos | Ecovias Noroeste Paulista |
| Catiguá | SP | Catiguá | 398,5 | ambos | Ecovias Noroeste Paulista |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

**Free Flow nas concessões desta rodovia:** Ecovias Noroeste Paulista, sim. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## PR-317

**1 praça** em PR: Via Campo, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P01 - Floresta | PR | Floresta | 129,6 | ambos | Via Campo |

Tabela oficial de tarifas: [Via Campo](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/via-campos/tarifa-de-pedagio/tarifas-de-pedagio).

**Free Flow nas concessões desta rodovia:** Via Campo, adiado. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## SP-318

**1 praça** em SP: Arteris ViaPaulista, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| São Carlos | SP | São Carlos | 254,374 | ambos | Arteris ViaPaulista |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-322

**2 praças** em SP: Entrevias, 2 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Sertãozinho | SP | Sertãozinho | 327,5 | ambos | Entrevias |
| Pitangueiras | SP | Pitangueiras | 361,5 | ambos | Entrevias |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## PR-323

**1 praça** em PR: Motiva Paraná, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| P01 SERTANEJA | PR | Sertaneja | 2,97 | ambos | Motiva Paraná |

Tabela oficial de tarifas: [Motiva Paraná](https://www.gov.br/antt/pt-br/assuntos/rodovias/concessionarias/lista-de-concessoes/pr-vias/tarifas-de-pedagio).

**Free Flow nas concessões desta rodovia:** Motiva Paraná, sim. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## SP-326

**1 praça** em SP: Ecovias Noroeste Paulista, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Colina | SP | Colina | 407,479 | ambos | Ecovias Noroeste Paulista |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

**Free Flow nas concessões desta rodovia:** Ecovias Noroeste Paulista, sim. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## SP-327

**1 praça** em SP: CART, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Ourinhos | SP | Santa Cruz do Rio Pardo | 14,5 | ambos | CART |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-330

**10 praças** em SP: AutoBAn, 4 praças (Anhanguera); Arteris Intervias, 2 praças (Anhanguera); Arteris ViaPaulista, 2 praças (Anhanguera); Entrevias, 2 praças (Anhanguera).

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Perus | SP | São Paulo | 26,495 | ambos | AutoBAn |
| Valinhos | SP | Valinhos | 81 | ambos | AutoBAn |
| Nova Odessa | SP | Nova Odessa | 117,71 | ambos | AutoBAn |
| Limeira (Anhanguera) | SP | Cordeirópolis | 152,46 | ambos | AutoBAn |
| Leme | SP | Leme | 181,76 | ambos | Arteris Intervias |
| Pirassununga | SP | Pirassununga | 215 | ambos | Arteris Intervias |
| Santa Rita do Passa Quatro | SP | Santa Rita do Passa Quatro | 253 | ambos | Arteris ViaPaulista |
| São Simão | SP | São Simão | 281 | ambos | Arteris ViaPaulista |
| Sales Oliveira | SP | Sales Oliveira | 350 | ambos | Entrevias |
| Ituverava | SP | Ituverava | 405 | ambos | Entrevias |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-332

**3 praças** em SP: Rota das Bandeiras, 3 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Paulínia B | SP | Paulínia | 132,5 | só norte | Rota das Bandeiras |
| Paulínia A | SP | Cosmópolis | 135,5 | ambos | Rota das Bandeiras |
| Engenheiro Coelho | SP | Engenheiro Coelho | 159,7 | ambos | Rota das Bandeiras |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-333

**4 praças** em SP: Entrevias, 4 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Pongaí | SP | Pongaí | 234,276 | ambos | Entrevias |
| Marília | SP | Marília | 315,13 | ambos | Entrevias |
| Echaporã | SP | Marília | 354,374 | ambos | Entrevias |
| Florínea | SP | n/d | 449,76 | ambos | Entrevias |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-334

**2 praças** em SP: Arteris ViaPaulista, 2 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Batatais | SP | Batatais | 344 | ambos | Arteris ViaPaulista |
| Restinga | SP | Restinga | 374,5 | ambos | Arteris ViaPaulista |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-340

**4 praças** em SP: Rota Mogiana, 4 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Jaguariúna | SP | Campinas | 123,5 | ambos | Rota Mogiana |
| Estiva Gerbi | SP | Mogi Guaçu | 192,84 | ambos | Rota Mogiana |
| Casa Branca | SP | Casa Branca | 221,292 | ambos | Rota Mogiana |
| Mococa | SP | Casa Branca | 254,69 | ambos | Rota Mogiana |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

**Free Flow nas concessões desta rodovia:** Rota Mogiana, previsto. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## SP-342

**2 praças** em SP: Rota Mogiana, 2 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Pinhal | SP | Espírito Santo do Pinhal | 191,89 | ambos | Rota Mogiana |
| Águas da Prata | SP | Águas da Prata | 240 | ambos | Rota Mogiana |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

**Free Flow nas concessões desta rodovia:** Rota Mogiana, previsto. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## SP-344

**2 praças** em SP: Rota Mogiana, 2 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Aguaí | SP | São João da Boa Vista | 219 | ambos | Rota Mogiana |
| São João da Boa Vista | SP | São João da Boa Vista | 230,44 | só leste | Rota Mogiana |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

**Free Flow nas concessões desta rodovia:** Rota Mogiana, previsto. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## SP-348

**5 praças** em SP: AutoBAn, 5 praças (Bandeirantes).

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Caieiras | SP | Caieiras | 36,2 | só sul | AutoBAn |
| Campo Limpo | SP | Franco da Rocha | 39 | só norte | AutoBAn |
| Itupeva | SP | Itupeva | 77,43 | ambos | AutoBAn |
| Sumaré | SP | Sumaré | 115,52 | ambos | AutoBAn |
| Limeira (Bandeirantes) | SP | Limeira | 159,55 | ambos | AutoBAn |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-350

**1 praça** em SP: Rota Mogiana, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Itobi | SP | Itobi | 252,14 | só norte | Rota Mogiana |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

**Free Flow nas concessões desta rodovia:** Rota Mogiana, previsto. Os pórticos estão em [Rodovias com Free Flow no Brasil](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/RODOVIAS-COM-FREE-FLOW.md).

---

## SP-360

**1 praça** em SP: Rota das Bandeiras, 1 praça.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Jundiaí | SP | Itatiba | 77,1 | ambos | Rota das Bandeiras |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## SP-425

**2 praças** em SP: Eixo SP, 2 praças.

| Praça (cadastro oficial) | UF | Município | km | Sentido cobrado | Concessão |
|---|:---:|---|:---:|---|---|
| Martinópolis | SP | Martinópolis | 400,1 | ambos | Eixo SP |
| Indiana | SP | Indiana | 436 | ambos | Eixo SP |

Tabela oficial de tarifas: [ARTESP](https://www.artesp.sp.gov.br/artesp/setor-regulado/rodovia/pedagios).

---

## Perguntas frequentes

<details>
<summary><strong>Quantas praças de pedágio tem a Via Dutra?</strong></summary>

Nas pistas da BR-116 operadas pela RioSP, entre São Paulo e Rio de Janeiro, são **9 praças com cabine** nesta base, contadas uma vez por local. No trecho metropolitano de São Paulo, a cobrança das pistas expressas é por Free Flow, com 21 pontos de cobrança, que estão no [repositório irmão](https://github.com/Sem-Parar/SEM-PARAR-FREE-FLOW/blob/main/rodovias/free-flow-dutra.md).
</details>

<details>
<summary><strong>O km da praça é o mesmo da placa na estrada?</strong></summary>

É o km do cadastro oficial, da ANTT nas federais e da ARTESP nas paulistas, que segue a quilometragem oficial da rodovia. Na BR-116, por exemplo, a contagem recomeça na divisa, então dois estados podem ter praças com km parecidos. No Rodoanel, cada praça fica num ramo de acesso, e o km é o do ramo.
</details>

<details>
<summary><strong>Por que algumas praças têm nome de código, como P1 ou P3?</strong></summary>

Porque é assim que a concessionária registra a praça no cadastro oficial. A coluna de município, ao lado, diz onde ela fica, e as coordenadas estão em [`dados/pracas-de-pedagio.csv`](dados/pracas-de-pedagio.csv). Nem sempre o nome da praça é o do município: a praça Rio Claro da Via Colinas, na SP-127, fica em Piracicaba, segundo a ARTESP.</details>

<details>
<summary><strong>Quantas praças de pedágio tem a Bandeirantes?</strong></summary>

Na SP-348, operada pela AutoBAn, são **5 praças com cabine** nesta base: Caieiras, Campo Limpo, Itupeva, Sumaré, Limeira (Bandeirantes), na ordem do km. A Anhanguera, a SP-330, tem 10 praças, divididas entre 4 concessões.
</details>

---

<div align="center">

### Passe direto com a Tag Sem Parar

Com a tag ativa, a cabine fica para trás: a cancela abre na pista automática e a passagem entra na fatura, em todas as rodovias pedagiadas do país.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/pedagios?utm_source=github&utm_medium=rodovias&utm_campaign=sem-parar-pedagios)**

Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

<br>

| Você quer | Vá para |
|---|---|
| Calcular o pedágio e o combustível de uma viagem | [Trace Sua Rota](https://www.semparar.com.br/trace-sua-rota?utm_source=github&utm_medium=rodovias&utm_campaign=sem-parar-pedagios) |
| Pagar uma passagem de Free Flow sem ser cliente | [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=rodovias&utm_campaign=sem-parar-pedagios) |
| Gestão de frota e vale-pedágio | [sempararempresas.com.br](https://www.sempararempresas.com.br?utm_source=github&utm_medium=rodovias&utm_campaign=sem-parar-pedagios) |

<br>

<sub>Repositório oficial mantido pelo <strong>Sem Parar</strong>. Conteúdo e dados sob <a href="LICENSE">CC BY 4.0</a>. Última revisão dos dados em 9 de novembro de 2026.</sub>

<sub><strong>Você com mais tempo para o que importa.</strong> #TudoProSeuCarro</sub>

</div>
