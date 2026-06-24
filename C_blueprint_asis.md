# Service Blueprint AS-IS — Gestão e Fiscalização de Contratos na APF

**Metodologia:** Shostack (1984) — 5 camadas, 3 linhas divisórias  
**Perspectiva:** Fiscal/Gestor de Contrato (o "cliente" / "cidadão" da jornada)  

**Posicionamento das camadas — leitura obrigatória:**

| Camada Shostack | Quem opera | Posição relativa às linhas |
|---|---|---|
| **Evidências Físicas** | Artefatos encontrados pelo Fiscal | acima de tudo |
| **Ações do Cidadão (Fiscal/Gestor)** | Fiscal Técnico · Fiscal Adm. · Gestor | **ACIMA** da Linha de Interação |
| *— Linha de Interação —* | | |
| **Frontstage** | Preposto · Contratada · RH/Adm (quando visível) | **ABAIXO** da Linha de Interação |
| *— Linha de Visibilidade —* | | |
| **Backstage** | Financeiro · Jurídico · Apoio de Contratos | abaixo da Linha de Visibilidade |
| *— Linha de Interação Interna —* | | |
| **Processos de Suporte** | SEI · SIAFI · e-Social · SICAF · Compras.gov.br | abaixo da Linha de Interação Interna |

> ⚠ **O Fiscal/Gestor opera EXCLUSIVAMENTE na camada "Ações do Cidadão", ACIMA da Linha de Interação. O Fiscal NUNCA opera no Frontstage.** O Frontstage é a camada da contratada e do preposto. Esta distinção foi o principal eixo de correção nas 6 rodadas do grill (ver `C_grill_transcript.md`).
>
> **Consistência com o transcript:** O blueprint usa "Ações do Cidadão (Fiscal/Gestor)" consistente com a posição correta do **examinador** no transcript. O transcript registra que o **aluno** errou essa classificação 4 vezes — mas o examinador corrigiu em cada caso. O blueprint reflete a posição **correta do examinador**, não os erros do aluno.

**Rubrica cruzada:** Cada etapa e ator desta tabela aparece em `C_grill_transcript.md` (Rodadas 1–6).

---

## Tabela Mestre

| Camada \ Etapa | 1. Designação e Assunção | 2. Reunião Inicial (Kick-off) | 3. Acompanhamento e Rotina | 4. Recebimento Provisório | 5. Recebimento Definitivo e Ateste | 6. Encaminhamento e Pagamento | 7. Ocorrências e Sanções | 8. Aditivos ou Encerramento |
|:---|:---|:---|:---|:---|:---|:---|:---|:---|
| **Evidências Físicas** | Portaria SEI; processo licitatório (TR, contrato, Matriz de Riscos); Termo de Ciência | Ata de reunião; ofício de credenciamento do preposto | Planilhas de IMR; e-mails institucionais; extrato conta vinculada (DEDMO) | Termo Provisório; Relatório de Medição; CNDs; guias de recolhimento trabalhista | Termo Definitivo; NF com ateste (SEI) | Despacho SEI; Nota de Lançamento (NL); Ordem Bancária (OB) | Notificação extrajudicial; defesa da empresa; parecer jurídico; tela SICAF | Relatório de avaliação; pesquisa de preços; Termo Aditivo |
| **Ações do Cidadão (Fiscal / Gestor)** | Recebe portaria; lê TR/contrato; assina Termo de Ciência | Convoca e preside reunião; alinha SLAs e canais oficiais; registra em ata | Mede IMR in loco; notifica preposto de falhas; mantém diário de ocorrências | Confere quantitativos da medição; verifica CNDs e guias; emite ateste provisório | Consolida pareceres técnico e administrativo; assina ateste final na NF | Autua documentação; elabora despacho para Financeiro | Instrui processo de penalidade; coleta provas; notifica empresa para defesa | Elabora Relatório Técnico avaliativo; justifica prorrogação ou encerramento |
| *— Linha de Interação —* | | | | | | | | |
| **Frontstage** (visível ao Fiscal) | RH publica portaria e comunica o fiscal; Adm. entrega processo e faz briefing | Preposto formalizado participa da reunião; empresa apresenta equipe e proposta | Preposto recebe notificações e responde; contratada executa serviços no local | Contratada entrega medição, CNDs e guias trabalhistas | Empresa apresenta Nota Fiscal; preposto confirma execução integral | Financeiro acusa recebimento do processo no SEI | Empresa recebe notificação formal e protocola defesa | Empresa manifesta interesse na renovação; Licitações comunica pesquisa de preços |
| *— Linha de Visibilidade —* | | | | | | | | |
| **Backstage** (invisível ao Fiscal) | Verificação de competências técnicas do servidor; análise de conflito de interesses; levantamento de carga de contratos já atribuídos | Adm. elabora modelos e check-lists; Jurídico verifica poderes do preposto | Fiscais setoriais consolidam dados e reportam ao Fiscal Técnico; banco verifica saldo e movimentação DEDMO | Fiscal Adm. analisa guias de recolhimento trabalhista e previdenciário; confere folha de pagamento e regularidade fiscal | Apoio de contratos prepara minutas de glosas; revisa pendências de notificações anteriores | Financeiro liquida despesa no SIAFI; retém 11% INSS; emite OB em ordem cronológica | Jurídico avalia contraditório e emite parecer; Autoridade Competente julga; Adm. registra sanção | Licitações realiza pesquisa de mercado; Jurídico valida minuta do aditivo; Financeiro verifica disponibilidade orçamentária |
| *— Linha de Interação Interna —* | | | | | | | | |
| **Processos de Suporte** | SEI (publicação da portaria); SIAPE (dados funcionais do servidor) | SEI (arquivo da ata e do ofício) | Compras.gov.br; sistema bancário DEDMO; planilhas avulsas; **shadow IT** (WhatsApp, Google Sheets) | Portais de CND: Receita Federal, PGFN, FGTS, Trabalhista | SEI (tramitação da NF e dos termos de recebimento) | SIAFI (liquidação, NL e OB); e-Social (cruzamento trabalhista); sistema bancário | SICAF; CEIS; CNEP; SEI (instrução processual) | Compras.gov.br (pesquisa de preços e publicação); SIAFI (reforço de empenho) |
| **⚠ Fail Points** | **[C]** Designação genérica: um fiscal para múltiplos contratos — inviabilidade material de fiscalizar | **[O]** Acordos verbais não registrados em ata; preposto sem formalização de poderes | **[C]** Shadow IT como canal oficial; **[C]** não verificação da conta DEDMO; ausência de diário de ocorrências | **[C]** CND como véu (PC-5): certidão válida ≠ trabalhadores pagos → *culpa in vigilando*; fiscalização superficial por pressão de prazo | **[C]** Ateste cego — Efeito Carimbador (PC-3): Gestor assina sem revisar; ateste de serviço não executado | **[C]** Quebra da ordem cronológica de pagamentos (IN 77/2022); **[C]** omissão da retenção de 11% INSS (Lei 8.212/91, Art. 31) | **[C]** Ameaça verbal sem instrução processual → prescrição da penalidade (PC-6); **[O]** fiscal sem letramento jurídico para instruir o contraditório | **[C]** Pedido de prorrogação enviado após vencimento → contrato verbal (Lei 4.320/64, Art. 60); **[O]** prorrogação de contrato deficitário por omissão |

**Legenda:** [C] Crítico · [O] Operacional · PC-n = Ponto Cego correspondente em `C_blueprint_gestao_fiscalizacao_v1.md`

---

## Notas de Rubrica — Cruzamento com C_grill_transcript.md

| Elemento do Blueprint | Aparece no Transcript |
|:---|:---|
| Cidadão / Fiscal/Gestor (Ações do Cidadão) | Rodadas 1–6 (eixo central de todas as perguntas) |
| Preposto (Frontstage) | R1-Q1; R2-Q3; R3-Q1; R5-Q5 |
| Contratada (Frontstage) | R2-Q7; R4-Q1; R5-Q1, Q5 |
| Fiscal Técnico / Fiscal Administrativo | R1-Q4; R2-Q5; R4-Q7; R5-Q1 a Q6 |
| Financeiro / Ordenador de Despesa | R2-Q3; R4-Q3, Q5 |
| Jurídico (Backstage) | R2-Q4; R4-Q4 |
| SEI (Processos de Suporte) | R4-Q5; R5-Q3; R6-Q5 |
| SIAFI (Processos de Suporte) | R1-Q6; R2-Q3; R4-Q5, Q6; R6-Q6 |
| e-Social (Processos de Suporte) | R2-Q8; R4-Q6; R6-Q6 |
| SICAF / CEIS / CNEP | R2-Q8 (indireto); mencionados em R2 |
| Shadow IT (PC-4) | R2-Q8 (LGPD); R3-Q4; R6-Q4 |
| CNDs / Evidências Físicas | R1-Q7; R2-Q3; R3-Q5 |
| Etapa 1 — Designação | R2-Q4; R4-Q7; R5 (papéis segregados) |
| Etapa 2 — Kick-off | R2-Q2; R4-Q7 |
| Etapa 3 — Acompanhamento | R1-Q5; R2-Q5; R3-Q1, Q4, Q8; R4 |
| Etapa 4 — Rec. Provisório | R1-Q1; R2-Q1, Q5; R3-Q5; R4-Q4 |
| Etapa 5 — Ateste Definitivo | R1-Q3, Q5; R3-Q3; R4-Q2; R5-Q3; R6-Q5 |
| Etapa 6 — Pagamento | R2-Q2, Q3; R4-Q1 a Q5 |
| Etapa 7 — Sanções | R2-Q8; R3-Q6; R4-Q4 |
| Etapa 8 — Encerramento/Aditivo | R4-Q7; R6 (redesign) |
| Linha de Interação | R1-Q3; R3-Q1; R5-Q1 |
| Linha de Visibilidade | R1-Q4; R3-Q2; R5-Q2 |
| Linha de Interação Interna | R1-Q6; R3-Q4; R4-Q6; R6-Q6 |
