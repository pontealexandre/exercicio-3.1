# Segunda Auditoria — Pesquisa para Service Blueprint AS-IS (v2)
## Objeto: verificação do tratamento dado ao audit_v1, detecção de falhas novas e pontos abertos

> **Escopo:** (a) confirmar se cada falha do audit_v1 foi de fato endereçada no corpo da v2 — não apenas declarada na tabela de tratamento; (b) detectar falhas introduzidas pela v2; (c) listar pontos que permanecem abertos. Verificação por busca web; fontes ao final. Questões cosméticas não contam como falha.

---

## Veredito

A v2 endereçou **9 das 10 falhas** do audit_v1 de forma limpa e deixou a décima (E1) em estado aceitável, porém não totalmente saneado. O ganho sobre a v1 é real e substancial.

Contudo, a v2 introduziu **um problema novo e grave (N1)**: afirmou ter verificado o Acórdão 1186/2017 nas bases do TCU e atribuiu-lhe um conteúdo que não se confirma. Uma alegação de checagem sem respaldo é, em auditoria, mais perigosa que uma omissão — carrega uma falsa garantia de fidedignidade. **Antes de promover a v2 a base de conhecimento, o Acórdão 1186/2017 precisa ser removido ou corrigido.** Resolvido isso, o documento está pronto para a destilação.

---

## (a) As falhas do audit_v1 foram endereçadas?

Cada item verificado contra o corpo da v2 (a tabela de tratamento só vale se o texto confirmar).

### Corrigidas e confirmadas — 9 de 10

| ID | Falha original | Status na v2 | Confirmação |
| :-- | :-- | :-- | :-- |
| A1 | Súmula 261/TCU errada | ✔ Resolvida | Súmula removida; seção 6 traz ON-AGU 76/2023 e arts. 141–145; fluxo de rastreabilidade cita ON-AGU para vedação de antecipação. |
| A2 | IN 81/2022 objeto errado | ✔ Resolvida | IN 81 removida; IN 05/2017 figura como norma de terceirização. |
| A3 | Lei 4.320/64 na etapa errada | ✔ Resolvida | Etapa 5 ficou só com art. 140, II; art. 63 da 4.320/64 movido para a etapa 6. |
| C1 | Retenção 11% omitida | ✔ Resolvida | Etapa 6, como bastidor e fail point. Base confirmada (art. 121 §5º Lei 14.133 c/c art. 31 Lei 8.212/91). |
| C2 | Decreto 11.246/2022 solto | ✔ Resolvida | Distribuído por etapa (arts. 21, 22, 23 nas etapas 1, 3, 5). |
| C3 | Conta vinculada omitida | ✔ Resolvida | Etapas 3 e 6, com fail point de não constituição. Mecanismo confirmado. |
| D1 | Responsabilização subsidiária | ✔ Resolvida | Promovida a risco central; Súmula 331, V, TST e culpa in vigilando nas etapas 4 e 5 e no sumário. |
| D2 | Designação genérica | ✔ Resolvida | Fail point da etapa 1. |
| E2 | "Crime de responsabilidade" | ✔ Resolvida | Reescrito como "grave irregularidade financeira, sujeita a responsabilização (improbidade, sanção do TCU ou erro grosseiro)". |

### Parcialmente resolvida — 1

**E1 — prazo "5º dia útil".** O detalhamento suaviza ("pressão prática", inclui IN SEGES 77/2022 da ordem cronológica), mas ainda apresenta a faixa "5 a 30 dias" como imposição contratual genérica, sem fonte. Melhor que a v1, porém não totalmente saneado. **Ação:** remover a faixa de prazos ou marcá-la explicitamente como observação de campo.

---

## (b) Falhas introduzidas pela v2

### N1 — Defesa não-sustentada do Acórdão 1186/2017 [GRAVE — nova]
A v2 alega: *"Realizei consulta às bases do TCU. O Acórdão 1186/2017-Plenário trata de FOC em aquisições, apontando pagamentos indevidos por falha de governança."*

A verificação não sustenta essa descrição. A única referência concreta localizada liga o Acórdão 1186/2017-Plenário a **repactuação e formação de preços** (contexto de reajuste de contrato de TI — apostilamento do FNDE/CTIS, DOU 01/10/2018), não a "FOC" (fraude/conluio) nem a "pagamentos indevidos por falha de governança". Ou houve confusão de acórdão, ou descrição de memória apresentada como verificada. Em qualquer hipótese, é uma **afirmação de verificação sem respaldo** — o tipo de inferência mal-suportada que esta auditoria existe para pegar.

**Ação:** remover o Acórdão 1186/2017 da seção 6 ou substituí-lo por acórdão cujo teor seja confirmável.

> Contraponto: a defesa do **Acórdão 1214/2013 está correta**. Ele trata efetivamente de gestão/fiscalização de contratos de serviços continuados e novas exigências de habilitação, originado de representação sobre melhorias na contratação e execução de terceirização de serviços continuados (Relator Min. Aroldo Cedraz, TC 006.156/2011-8, Sessão 22/5/2013). Mantê-lo está justificado.

### N2 — e-Social e SICAF afirmados sem lastro [menor — nova]
A v2 acrescentou "e-Social" (etapa 4) e "inserção da punição no SICAF" (etapa 7). Ambos são plausíveis e provavelmente corretos na prática, mas entraram sem que o audit_v1 os pedisse e sem fonte. Não são erros confirmados — são afirmações novas que merecem checagem antes de virarem base de conhecimento. Registrado por consistência metodológica.

### N3 — Sigla "DEMO" [cosmético — não conta como falha]
A v2 usa "DEMO" para Dedicação Exclusiva de Mão de Obra. O jargão consagrado é "DEDMO" ou "dedicação exclusiva". Apenas padronização.

---

## (c) Pontos que permanecem abertos

| Ponto | Estado | Ação |
| :-- | :-- | :-- |
| Acórdão 1186/2017 (N1) | **Aberto — prioritário** | Verificar no portal do TCU ou remover. Não usar como fonte enquanto não confirmar o teor. |
| E1 (faixa "5 a 30 dias") | Semiaberto | Remover faixa de prazos ou marcar como observação de campo. |
| N2 (e-Social / SICAF) | Aberto (leve) | Confirmar antes de consolidar. |
| Acórdão 1214/2013 | **Fechado** | Verificado e correto. |

---

## Fontes consultadas na verificação

- Acórdão 1214/2013-TCU-Plenário (TC 006.156/2011-8, Rel. Min. Aroldo Cedraz, Sessão 22/5/2013) — Revista do TCU n. 148; Portal Investidura; comprasnet.gov.br; Jus Navigandi.
- Acórdão 1186/2017-TCU-Plenário — única referência localizada: apostilamento FNDE/CTIS (DOU 01/10/2018), contexto de repactuação/formação de preços. Teor "FOC / pagamentos indevidos" NÃO confirmado.
- Conta-depósito vinculada e culpa in vigilando — material doutrinário sobre terceirização à luz do TCU; IN 02/2008/SLTI anexo VII.
- Retenção previdenciária 11% — TCU, Licitações e Contratos (art. 121 §5º Lei 14.133 c/c art. 31 Lei 8.212/91).

> **Nota metodológica:** o Acórdão 1186/2017 deve ser confirmado diretamente em pesquisa.apps.tcu.gov.br antes de qualquer uso. A ausência de confirmação aqui não prova que o acórdão não exista — prova apenas que o conteúdo a ele atribuído pela v2 não foi corroborado por nenhuma fonte localizada.
