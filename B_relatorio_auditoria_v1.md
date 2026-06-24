# Relatório de Auditoria — Pesquisa para Service Blueprint AS-IS
## Objeto auditado: pesquisa estruturada sobre Gestão e Fiscalização de Contratos na Administração Pública Federal (ótica do Fiscal/Gestor)

> **Escopo da auditoria:** verificação de erros factuais, omissões de bastidor, normativos/evidências ausentes, fail points não identificados e inferências mal-suportadas. Questões cosméticas (formatação, estilo, ordem) foram deliberadamente ignoradas. Afirmações normativas verificadas por busca web; fontes indicadas ao final.

---

## Parecer-síntese

Estruturalmente o blueprint é sólido: a jornada do fiscal está bem reconstruída, os fail points são realistas e os pontos cegos (acordo de cavalheiros, herança de contratos, shadow IT, efeito carimbador) são genuinamente úteis para a destilação. O problema concentra-se nas **fontes normativas** — a parte que não pode conter erro, porque o blueprint vira base de conhecimento para entregáveis seguintes.

Há **duas trocas de objeto normativo graves** (Súmula 261/TCU e IN SEGES 81/2022) que se propagariam para qualquer artefato posterior, mais uma alocação de norma à etapa errada (Lei 4.320/64). Em segundo nível, faltam um fail point central (responsabilização subsidiária trabalhista) e uma obrigação de bastidor recorrente (retenção previdenciária de 11%).

---

## A. Erros factuais (com trecho citado)

### A1 — Súmula 261/TCU descrita com conteúdo errado [GRAVE]
**Trecho auditado:** *"Súmula 261/TCU (Vedação de pagamento antecipado sem ateste)"* (seção 6).

A atribuição está incorreta. A Súmula TCU 261 trata de **projeto básico** em licitações de obras — da exigência de projeto básico adequado, preciso e atualizado, sendo aplicada contra editais com planilhas e quantitativos arbitrários. Não tem relação com pagamento antecipado nem com ateste.

A vedação ao pagamento antecipado tem outra base: em regra, o pagamento só pode ocorrer após o recebimento do objeto e a emissão da nota fiscal, com fundamento na Lei 14.133/2021 (arts. 141 a 145) e na **Orientação Normativa AGU 76/2023**.

**Correção:** substituir a referência da Súmula 261 pela ON-AGU 76/2023 e pelos arts. 141–145 da Lei 14.133/2021.

### A2 — IN SEGES 81/2022 descrita com objeto errado [GRAVE]
**Trecho auditado:** *"IN SEGES/ME nº 81/2022 (Terceirização e Serviços)"* (seção 6).

Errado. A IN SEGES/ME 81/2022 dispõe sobre a **elaboração do Termo de Referência (TR) e o Sistema TR Digital** — norma da fase preparatória, não de terceirização. A norma de serviços terceirizados/continuados com dedicação de mão de obra é a **IN SEGES 05/2017**, que a própria pesquisa cita corretamente em outro ponto.

**Correção:** reclassificar a IN 81/2022 como norma de TR (fase preparatória, fora do recorte AS-IS), ou substituí-la pela IN 05/2017 se a intenção era citar a norma de terceirização.

### A3 — "Lei 4.320/64 (Art. 63)" alocada à etapa errada [MODERADO]
**Trecho auditado:** Etapa 5 (Rec. Definitivo e Ateste) → normativo *"Lei 4.320/64 (Art. 63)"*.

O art. 63 da Lei 4.320/64 trata da **liquidação da despesa** (verificação do direito adquirido pelo credor), que é ato do setor financeiro — **etapa 6** no blueprint, não o ateste do gestor na etapa 5. A pesquisa funde o ateste (ato do fiscal/gestor, fundado no art. 140 da Lei 14.133) com a liquidação (ato contábil-financeiro, fundado na 4.320/64). A norma existe e é pertinente, mas está na etapa errada.

**Correção:** mover a Lei 4.320/64, art. 63, para a etapa 6 (Encaminhamento e Pagamento) e deixar a etapa 5 ancorada no art. 140, II, da Lei 14.133.

---

## B. Pontos verificados que estão corretos (não rechecar)

- **Art. 117 e parágrafos** — bem aplicados: o fiscal detém a atribuição indelegável de atestar a conformidade da execução; todas as ocorrências devem ser anotadas no histórico de gerenciamento do contrato, incluindo a substituição do fiscal titular.
- **Art. 140** (recebimento provisório/definitivo), **Art. 118** (preposto), **Arts. 155–163** (sanções) e **Arts. 132–136** (alterações) — corretamente atribuídos.
- **Decreto 11.246/2022** — corretamente descrito como a norma que regulamenta a atuação de gestores e fiscais de contratos (mas ver C2: não está amarrado às etapas).
- **Acórdãos 1.214/2013-Plenário e 1.186/2017-Plenário** — **NÃO verificados** nesta auditoria. Não confirmados nem refutados; exigem checagem direta no portal do TCU antes de publicar.

---

## C. Omissões de bastidor / normativos relevantes

### C1 — Retenção previdenciária de 11% ausente
O blueprint trata a conferência fiscal (CNDs, FGTS, INSS) na etapa 4, mas omite uma obrigação concreta de back-stage: a Administração deve reter 11% do valor bruto da nota fiscal de prestação de serviços e recolher ao órgão previdenciário em nome da empresa (art. 121, §5º, da Lei 14.133 c/c art. 31 da Lei 8.212/91). É ação financeira recorrente, com fail point próprio (retenção indevida ou não efetuada).

### C2 — Decreto 11.246/2022 não amarrado às etapas
O decreto é a espinha regulamentar das atribuições de fiscal técnico, administrativo, setorial e gestor, mas aparece apenas na lista de fontes. Cada etapa da tabela deveria referenciá-lo na coluna de normativos — p. ex., o recebimento definitivo mediante termo detalhado e a coordenação da rotina de fiscalização com histórico de gerenciamento são atribuições que o decreto detalha por tipo de fiscal.

### C3 — Conta-depósito vinculada / garantia
Para contratos com dedicação exclusiva de mão de obra existe o mecanismo de depósito de valores em conta vinculada e bloqueada, como salvaguarda trabalhista. É um bastidor administrativo-financeiro relevante e um fail point clássico (não constituição da conta vinculada), ausente do blueprint.

---

## D. Fail points não identificados

### D1 — Responsabilização subsidiária trabalhista por falha de fiscalização [CENTRAL]
Talvez o maior risco pessoal/institucional da fiscalização administrativa, e está ausente. A ausência de fiscalização adequada caracteriza culpa in vigilando e justifica a responsabilidade subsidiária do ente público pelos créditos trabalhistas, exigindo que a Administração comprove documentalmente que fiscalizou o cumprimento das obrigações trabalhistas (Súmula 331, V, TST; art. 121 da Lei 14.133). O fail point existente "conferência de FGTS/INSS por pressão de prazo" toca no tema, mas subdimensiona a consequência (condenação judicial do órgão).

### D2 — Designação genérica de fiscal
A pesquisa cita "fiscal com excesso de contratos", mas falta o fail point específico já apontado por tribunais de contas: a designação de um único servidor por secretaria para acompanhar todos os contratos não garante o acompanhamento efetivo e pode gerar inobservância da lei.

---

## E. Inferências mal-suportadas / fontes fracas

### E1 — Pagamento "até o 5º dia útil"
A etapa 4/5 apresenta como regra a pressão de que "o pagamento precisa sair até o 5º dia útil". É plausível como prática de campo, mas não há base normativa geral para esse prazo específico — o que existe é a ordem cronológica de pagamentos (IN SEGES 77/2022) e os prazos contratuais. Marcar como hipótese de campo, não como regra.

### E2 — "Crime de responsabilidade" por pagar antes de liquidar
A seção 4 afirma que pagar antes de liquidar "constitui crime de responsabilidade". A sequência empenho→liquidação→pagamento é obrigatória, mas a tipificação como "crime de responsabilidade" é imprecisa — a irregularidade configura, conforme o caso, ato de improbidade, infração financeira sancionável pelo TCU e, na jurisprudência sob a 8.666, erro grosseiro. Recomenda-se suavizar para "grave irregularidade financeira, sujeita a responsabilização".

---

## F. Tabela de severidade (priorização de correção)

| ID | Falha | Tipo | Severidade | Ação |
|----|-------|------|------------|------|
| A1 | Súmula 261/TCU com conteúdo errado | Erro factual | Grave | Substituir por ON-AGU 76/2023 + arts. 141–145 |
| A2 | IN 81/2022 descrita como terceirização | Erro factual | Grave | Reclassificar como norma de TR ou trocar por IN 05/2017 |
| D1 | Responsabilização subsidiária trabalhista | Fail point omitido | Central | Adicionar às etapas 4 e 6 |
| A3 | Lei 4.320/64 na etapa errada | Alocação incorreta | Moderado | Mover para etapa 6 |
| C1 | Retenção previdenciária 11% | Bastidor omitido | Moderado | Adicionar à etapa 6 |
| C2 | Decreto 11.246/2022 não amarrado | Normativo solto | Moderado | Referenciar por etapa |
| C3 | Conta vinculada / garantia | Bastidor omitido | Moderado | Adicionar como fail point |
| D2 | Designação genérica de fiscal | Fail point omitido | Baixo | Refinar etapa 1 |
| E2 | "Crime de responsabilidade" | Inferência imprecisa | Baixo | Suavizar redação |
| E1 | Prazo "5º dia útil" | Inferência fraca | Baixo | Marcar como hipótese |
| — | Acórdãos 1.214/2013 e 1.186/2017 | Não verificado | — | Checar no portal TCU |

---

## G. Fontes consultadas na verificação

- Lei 14.133/2021, arts. 117, 118, 140, 141–145, 121 §5º — TCU (licitacoesecontratos.tcu.gov.br); TCE-SP (legislação comentada).
- Súmula TCU 261 — TCE-MG, Informativo de Jurisprudência n. 321; jurisprudência TCU.
- IN SEGES/ME 81/2022 — Portal de Compras do Governo Federal; gov.br/governodigital.
- IN SEGES 05/2017 e IN SEGES 77/2022 (ordem cronológica) — IFB; gov.br/compras.
- Decreto 11.246/2022 — gov.br/governodigital; AGU/SAPIENS.
- ON-AGU 76/2023 (vedação a pagamento antecipado) — TCU, Licitações e Contratos.
- Responsabilização subsidiária / culpa in vigilando — Súmula 331 TST; jurisprudência citada (Jusbrasil; Barbieri Advogados).
- Lei 8.212/91, art. 31 (retenção 11%) — TCU, Licitações e Contratos.

> **Observação:** os acórdãos 1.214/2013-Plenário e 1.186/2017-Plenário, citados na pesquisa original, não foram confirmados nesta sessão e devem ser verificados diretamente em pesquisa.apps.tcu.gov.br antes da publicação.
