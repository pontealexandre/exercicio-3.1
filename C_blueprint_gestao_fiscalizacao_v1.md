# Service Blueprint AS-IS — Versão 1

## Serviço: Gestão e Fiscalização de Contratos na Administração Pública Federal

---

## 1. Sumário Executivo

A fase de execução contratual na Administração Pública Federal é um serviço de alta complexidade normativa prestado internamente pelo Estado a si mesmo: o **Fiscal/Gestor de Contrato** é o agente que sustenta a conformidade e a legalidade do dispêndio público. A jornada AS-IS revela um servidor que transita entre sistemas não integrados (SEI, Compras.gov.br, planilhas avulsas, SIAFI), absorve uma carga cognitiva desproporcional ao ferramental disponível e responde pessoalmente pelas falhas de omissão.

O presente blueprint aplica a metodologia de **G. Lynn Shostack (1984)** a esse serviço, mapeando explicitamente as cinco camadas (Evidências Físicas, Ações do Fiscal, Frontstage, Backstage, Processos de Suporte) e as três linhas divisórias (Interação, Visibilidade, Interação Interna). O artefato identifica os pontos em que o design atual do serviço falha antes que a falha se torne um processo de responsabilização.

**Tensão central:** O servidor é simultaneamente cliente da burocracia estatal (depende de sistemas e setores de apoio que não controla) e provedor de conformidade para o Estado (responde pelas omissões desses mesmos sistemas). Essa posição estruturalmente ambígua é a raiz da maioria dos fail points identificados.

---

## 2. Nota Metodológica — Shostack Aplicado ao Contexto

Em Shostack (1984), o Service Blueprint organiza o serviço em camadas horizontais separadas por linhas divisórias que explicitam o que é visível ou não para o cliente. Neste blueprint, os papéis foram mapeados da seguinte forma:

| Camada Shostack | Correspondência neste serviço |
| :--- | :--- |
| **Evidências Físicas** | Documentos, portarias, sistemas, formulários e registros tangíveis (físicos ou digitais) encontrados pelo Fiscal em cada etapa |
| **Ações do Fiscal/Gestor** | O ator principal da jornada — o servidor público designado como fiscal técnico, administrativo e/ou gestor |
| `— LINHA DE INTERAÇÃO —` | Separa o Fiscal das partes com quem interage diretamente: preposto, contratada, setores de apoio |
| **Ações Frontstage** | Ações visíveis ao Fiscal: respostas do preposto, entregas da contratada, despachos e feedbacks dos setores internos |
| `— LINHA DE VISIBILIDADE —` | Separa o que o Fiscal vê do que ocorre nos bastidores sem seu acompanhamento |
| **Ações Backstage** | Ações invisíveis ao Fiscal: análises financeiras, processamentos jurídicos, conferências sistêmicas, registros no SIAFI |
| `— LINHA DE INTERAÇÃO INTERNA —` | Separa as equipes de backstage dos sistemas tecnológicos e de suporte que as sustentam |
| **Processos de Suporte** | Infraestrutura tecnológica e normativa: SEI, SIAFI, Compras.gov.br, SICAF, CEIS, CNEP, bancos de dados trabalhistas |

> **Nota de adaptação:** No blueprint original de Shostack, o "cliente" é o beneficiário externo do serviço. Aqui, o **Fiscal/Gestor** assume esse papel porque é o ator que vive a jornada, toma decisões e responde por elas. A contratada e seu preposto atuam na camada frontstage — são a "face visível do serviço" que o Fiscal enfrenta diariamente.

---

## 3. Visão Panorâmica — Tabela de Referência Rápida

| Etapa | Evidência Central | Ação-Chave do Fiscal | Principal Frontstage | Principal Backstage | Sistema de Suporte | ⚠ Fail Point Crítico |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1. Designação e Assunção | Portaria + Processo SEI | Ler TR, contrato e assinar Termo de Ciência | RH emite portaria; Administração entrega processo | Verificação de competências e conflito de interesses | SEI / SIAPE | Designação genérica (múltiplos contratos por fiscal) |
| 2. Reunião Inicial (Kick-off) | Ata de Reunião + Ofício do preposto | Alinhar SLAs e rotinas com preposto | Preposto formalizado participa e alinha operação | Elaboração de modelos e check-lists de acompanhamento | SEI (arquivo de ata) | Acordos verbais não registrados em ata |
| 3. Acompanhamento e Rotina | Planilhas IMR + e-mails institucionais | Medir IMR in loco; notificar preposto; manter diário | Preposto recebe notificações; contratada executa | Fiscais setoriais consolidam dados; banco verifica conta vinculada | Compras.gov.br / DEDMO | WhatsApp como canal oficial (shadow IT) |
| 4. Recebimento Provisório | Termo Provisório + CNDs + guias trabalhistas | Conferir medição e emitir ateste provisório | Contratada entrega NF e documentação previdenciária | Fiscal Adm. analisa guias e regularidade fiscal | Portais CND / planilhas | Ateste sem conferência trabalhista real (culpa in vigilando) |
| 5. Recebimento Definitivo e Ateste | Termo Definitivo + NF atestada no SEI | Consolidar recebimentos e assinar ateste final | Empresa confirma execução; preposto co-assina medição | Apoio de contratos prepara minutas de glosas | SEI (tramitação da NF) | Ateste "cego" do Gestor sem revisão substancial |
| 6. Encaminhamento e Pagamento | Despacho SEI + NL + OB no SIAFI | Autuar docs e despachar para Financeiro | Financeiro acusa recebimento do processo | Liquidação no SIAFI; retenção 11% INSS; emissão da OB | SIAFI / e-Social | Quebra da ordem cronológica; não retenção previdenciária |
| 7. Ocorrências e Sanções | Notificação + Defesa + Parecer Jurídico | Instruir processo de penalidade com provas | Empresa recebe notificação e apresenta defesa | Jurídico avalia; Autoridade julga; Adm. registra sanção | SICAF / CEIS / CNEP | Ameaça verbal sem instrução → prescrição da penalidade |
| 8. Aditivos ou Encerramento | Relatório de Avaliação + Termo Aditivo | Elaborar Relatório Técnico; justificar prorrogação | Empresa manifesta interesse; Licitações pesquisam preço | Jurídico valida aditivo; Financeiro reforça empenho | Compras.gov.br / SIAFI | Pedido enviado após vencimento → contrato verbal |

---

## 4. Blueprint Detalhado por Etapa — Camadas AS-IS (Shostack)

---

### Etapa 1 — Designação e Assunção

**Evidências Físicas**
- Portaria de designação publicada no SEI
- Processo SEI da licitação (TR, Edital, Contrato, Matriz de Riscos)
- Termo de Ciência e Responsabilidade (assinado pelo fiscal)

**Ações do Fiscal/Gestor**
- Recebe notificação da portaria
- Abre e estuda o processo: TR, contrato, matriz de riscos e histórico de ocorrências (se houver)
- Assina o Termo de Ciência e passa a responder formalmente pelo contrato

`— LINHA DE INTERAÇÃO —`

**Ações Frontstage** *(visíveis ao Fiscal)*
- Área de Gestão de Pessoas publica a portaria e comunica o fiscal
- Administração do Contrato (área demandante) entrega o processo e faz briefing informal
- Fiscal anterior (se houver substituição) realiza passagem de bastão — ou não

`— LINHA DE VISIBILIDADE —`

**Ações Backstage** *(invisíveis ao Fiscal)*
- Verificação se o servidor possui competências técnicas para o tipo de contrato
- Análise de possível conflito de interesses (relação prévia com a contratada)
- Levantamento do volume total de contratos já atribuídos ao servidor (carga acumulada)

`— LINHA DE INTERAÇÃO INTERNA —`

**Processos de Suporte**
- SEI: publicação e tramitação da portaria
- SIAPE/sistema de RH: dados funcionais do servidor designado
- Banco de dados de designações (quando existente na unidade)

**Normativos:** Lei 14.133/2021, Art. 117; Decreto 11.246/2022, Arts. 21-22

**⚠ Fail Points**
- **[CRÍTICO]** Designação genérica: um servidor para múltiplos contratos simultâneos, gerando inviabilidade material de fiscalizar qualquer um com profundidade
- **[OPERACIONAL]** Herança de contrato sem passagem de bastão estruturada: conhecimento tácito perdido no e-mail ou WhatsApp do fiscal anterior
- **[OPERACIONAL]** Fiscal sem qualificação técnica para o objeto do contrato (ex.: servidor administrativo designado para fiscal técnico de TI ou engenharia)

---

### Etapa 2 — Reunião Inicial (Kick-off)

**Evidências Físicas**
- Ata de Reunião de Kick-off (lavrada em SEI ou papel)
- Ofício de credenciamento do preposto (enviado pela empresa)
- Check-list de alinhamento operacional (quando existe)

**Ações do Fiscal/Gestor**
- Convoca e preside a reunião com o preposto da contratada
- Alinha: SLAs contratuais, rotinas de medição, canais oficiais de comunicação, prazos de entrega de documentação
- Registra os acordos em ata e trata da formalização do preposto

`— LINHA DE INTERAÇÃO —`

**Ações Frontstage** *(visíveis ao Fiscal)*
- Preposto credenciado pela empresa participa e representa a contratada
- Empresa apresenta equipe, cronograma e proposta operacional
- Área Administrativa da contratante entrega modelos de documentação exigida

`— LINHA DE VISIBILIDADE —`

**Ações Backstage** *(invisíveis ao Fiscal)*
- Área Administrativa elabora modelos de comunicação, formulários de medição e check-lists
- Setor de Contratos verifica se o preposto indicado tem poderes suficientes (procuração)
- Juridico verifica cláusulas de subcontratação e obrigações acessórias que devem ser reforçadas

`— LINHA DE INTERAÇÃO INTERNA —`

**Processos de Suporte**
- SEI: arquivamento da ata e do ofício de credenciamento
- Modelos padronizados de atas e formulários (quando existentes na unidade)

**Normativos:** Lei 14.133/2021, Art. 118; IN SEGES/MP nº 05/2017 (rotinas de fiscalização)

**⚠ Fail Points**
- **[CRÍTICO]** Acordos operacionais firmados verbalmente sem registro em ata: desvios futuros ficam sem base probatória para notificação
- **[OPERACIONAL]** Preposto sem formalização documental ou sem poderes para representar a empresa em decisões
- **[COSMÉTICO]** Kick-off tratado como formalidade burocrática, sem alinhamento real de SLAs e expectativas

---

### Etapa 3 — Acompanhamento e Rotina

**Evidências Físicas**
- Planilhas de controle de IMR (Instrumento de Medição de Resultado)
- E-mails institucionais de notificação ao preposto
- Comprovante de depósito na Conta-Depósito Vinculada (contratos DEDMO)
- Diário de ocorrências (quando mantido)

**Ações do Fiscal/Gestor**
- Realiza visitas de acompanhamento e mede IMR/SLA in loco
- Notifica o preposto formalmente sobre falhas e inconformidades identificadas
- Consolida o diário de ocorrências mensalmente para subsidiar o recebimento provisório

`— LINHA DE INTERAÇÃO —`

**Ações Frontstage** *(visíveis ao Fiscal)*
- Preposto recebe notificações, acusa ciência e apresenta justificativas ou planos de ação
- Equipe da contratada executa os serviços e interage com fiscais setoriais no local
- Fiscais setoriais (quando existentes) alimentam o Fiscal Técnico com dados consolidados

`— LINHA DE VISIBILIDADE —`

**Ações Backstage** *(invisíveis ao Fiscal)*
- Banco gestor (Banco do Brasil ou Caixa) verifica os saldos e movimentações da Conta-Depósito Vinculada (DEDMO)
- Setor de contratos monitora vencimentos, saldos de empenho e obrigações acessórias
- Financeiro acompanha a posição de crédito orçamentário disponível para pagamento

`— LINHA DE INTERAÇÃO INTERNA —`

**Processos de Suporte**
- Compras.gov.br: consulta de informações contratuais
- Sistema bancário de conta vinculada (DEDMO)
- Planilhas avulsas de IMR (frequentemente locais, sem integração sistêmica)
- **Shadow IT:** WhatsApp, e-mails pessoais, Google Sheets não corporativos

**Normativos:** Decreto 11.246/2022, Art. 23 (fiscal técnico); Lei 14.133/2021, Art. 117, §1º

**⚠ Fail Points**
- **[CRÍTICO]** Acompanhamento exclusivo via WhatsApp: comunicações sem validade probatória formal e sujeitas a perda com troca de aparelho/número
- **[CRÍTICO]** Não verificação da Conta-Depósito Vinculada (DEDMO): recolhimentos trabalhistas "fantasmas" declarados mas não depositados
- **[OPERACIONAL]** Ausência de diário de ocorrências: falhas não documentadas impossibilitam instrução futura de processos de sanção
- **[OPERACIONAL]** Fragmentação entre fiscais setoriais sem protocolo de consolidação: dados chegam ao Fiscal Técnico incompletos ou com atraso

---

### Etapa 4 — Recebimento Provisório

**Evidências Físicas**
- Termo de Recebimento Provisório
- Relatório de Medição (apresentado pela contratada)
- CNDs vigentes (Receita Federal, FGTS, Trabalhista, Municipal)
- Guias de recolhimento trabalhista e previdenciário

**Ações do Fiscal/Gestor**
- Confere os quantitativos executados declarados na medição
- Verifica a regularidade fiscal e trabalhista da contratada (CNDs e guias)
- Emite o ateste provisório confirmando a qualidade da execução do período

`— LINHA DE INTERAÇÃO —`

**Ações Frontstage** *(visíveis ao Fiscal)*
- Contratada entrega o Relatório de Medição, as guias de recolhimento e as CNDs
- Preposto confirma a execução do escopo e solicita anuência formal do fiscal

`— LINHA DE VISIBILIDADE —`

**Ações Backstage** *(invisíveis ao Fiscal)*
- Fiscal Administrativo analisa individualmente as guias de recolhimento trabalhista e previdenciário
- Verifica folha de pagamento, FGTS, férias, 13º e demais direitos dos trabalhadores alocados
- Confere regularidade fiscal junto aos portais de CND (Receita, PGFN, FGTS)

`— LINHA DE INTERAÇÃO INTERNA —`

**Processos de Suporte**
- Portal da Receita Federal e PGFN (CND tributária)
- Portal do FGTS / Caixa (CND trabalhista)
- Portais Estaduais e Municipais (quando exigidos)
- Planilhas de conferência de folha de pagamento

**Normativos:** Lei 14.133/2021, Art. 140, I; Súmula 331, V, do TST *(culpa in vigilando)*; Art. 121 da Lei 14.133/2021

**⚠ Fail Points**
- **[CRÍTICO]** Fiscalização superficial por pressão de prazo: CNDs checadas superficialmente sem conferência real da folha de pagamento → risco de responsabilidade trabalhista subsidiária da União
- **[CRÍTICO]** Empresa com CND válida mas com débitos em parcelamento: a regularidade formal mascara a irregularidade material
- **[OPERACIONAL]** Confusão entre CND geral da empresa e CND específica para o lote/unidade do contrato (especialmente em empresas com múltiplas filiais)
- **[OPERACIONAL]** Guias de recolhimento apresentadas sem cruzamento com a relação nominal dos trabalhadores alocados no contrato

---

### Etapa 5 — Recebimento Definitivo e Ateste

**Evidências Físicas**
- Termo de Recebimento Definitivo (assinado pelo Gestor)
- Nota Fiscal com ateste (carimbo físico ou assinatura digital no SEI)
- Eventuais minutas de glosa (desconto) devidamente instruídas

**Ações do Fiscal/Gestor**
- Consolida os pareceres do Fiscal Técnico e do Fiscal Administrativo
- Revisa a documentação completa do ciclo
- Assina o ateste final na Nota Fiscal, declarando ao Estado que o objeto foi recebido

`— LINHA DE INTERAÇÃO —`

**Ações Frontstage** *(visíveis ao Fiscal)*
- Empresa apresenta a Nota Fiscal para ateste
- Preposto confirma formalmente a execução integral do escopo contratado

`— LINHA DE VISIBILIDADE —`

**Ações Backstage** *(invisíveis ao Fiscal)*
- Apoio de contratos (quando existente) prepara minutas de glosas para desconto em caso de falhas documentadas
- Setor revisa se há pendências de notificações anteriores que devem ser convertidas em glosa antes do pagamento

`— LINHA DE INTERAÇÃO INTERNA —`

**Processos de Suporte**
- SEI: digitalização da NF, tramitação do processo e registro do ateste
- Modelos de Termo de Recebimento Definitivo (padronizados ou ad hoc)

**Normativos:** Lei 14.133/2021, Art. 140, II; Decreto 11.246/2022, Art. 21 (atribuições do Gestor)

**⚠ Fail Points**
- **[CRÍTICO]** Ateste "cego": Gestor assina a NF sem revisar os pareceres dos fiscais, fiando-se apenas na confiança interpessoal → Efeito Carimbador
- **[CRÍTICO]** Ateste de serviço parcialmente não executado: ocorre quando o diário de ocorrências da Etapa 3 não foi mantido e não há provas de falhas
- **[OPERACIONAL]** Glosas não aplicadas por ausência de instrução prévia: infrações documentadas mas não formalizadas em notificação perdem o fundamento para desconto
- **[OPERACIONAL]** NF com valores divergentes do contrato (erros ou reajustes não formalizados) atestada sem ressalva

---

### Etapa 6 — Encaminhamento e Pagamento

**Evidências Físicas**
- Despacho de encaminhamento no SEI
- Nota de Lançamento (NL) no SIAFI
- Ordem Bancária (OB) emitida pelo SIAFI
- Comprovante de retenção previdenciária (11%)

**Ações do Fiscal/Gestor**
- Autua os documentos do ciclo (NF atestada, termos de recebimento, guias) no processo SEI
- Elabora despacho de encaminhamento para a unidade financeira
- Aguarda liquidação e pagamento (etapa de baixo controle do fiscal)

`— LINHA DE INTERAÇÃO —`

**Ações Frontstage** *(visíveis ao Fiscal)*
- Unidade Financeira acusa recebimento do processo pelo SEI
- Financeiro comunica eventuais pendências ou inconsistências documentais que bloqueiam a liquidação

`— LINHA DE VISIBILIDADE —`

**Ações Backstage** *(invisíveis ao Fiscal)*
- Financeiro liquida a despesa no SIAFI (verificação do ateste, crédito orçamentário e regularidade fiscal)
- Realiza a **retenção legal de 11% do INSS** sobre o valor da Nota Fiscal (Lei 8.212/91, Art. 31)
- Posiciona o processo na fila respeitando a **ordem cronológica de pagamentos** (IN SEGES 77/2022)
- Emite a Ordem Bancária (OB) e credita o valor na conta da contratada

`— LINHA DE INTERAÇÃO INTERNA —`

**Processos de Suporte**
- **SIAFI:** liquidação da despesa, emissão de NL e OB
- **e-Social / eSocial:** cruzamento de informações trabalhistas para suporte à retenção
- **Compras.gov.br:** consulta de dados contratuais e saldo de empenho
- **Sistema Bancário (Banco do Brasil):** processamento da transferência financeira

**Normativos:** Lei 4.320/1964, Art. 63 (liquidação); ON AGU nº 76/2023 (vedação de pagamento antecipado); Lei 8.212/1991, Art. 31 (retenção 11%); IN SEGES/ME nº 77/2022 (ordem cronológica)

**⚠ Fail Points**
- **[CRÍTICO]** Quebra da ordem cronológica de pagamentos: pagamento fora da fila constitui irregularidade financeira grave (Lei 4.320/64)
- **[CRÍTICO]** Não recolhimento da retenção previdenciária de 11% na fonte: gera responsabilidade solidária da União
- **[OPERACIONAL]** Processo devolvido por pendência documental sem comunicação clara ao fiscal: retrabalho e atraso que configura ilegalidade se ultrapassar prazos
- **[OPERACIONAL]** Empenho insuficiente no final do exercício: contratada executou o serviço sem crédito orçamentário disponível para pagamento (contrato verbal de fato)

---

### Etapa 7 — Ocorrências e Sanções

**Evidências Físicas**
- Notificação extrajudicial (enviada formalmente ao preposto)
- Defesa escrita da empresa
- Parecer Jurídico sobre a sanção proposta
- Tela de registro no SICAF / CEIS / CNEP

**Ações do Fiscal/Gestor**
- Instrui processo apartado de penalidade com as provas colhidas no diário de ocorrências
- Elabora notificação formal concedendo prazo para defesa e contraditório
- Encaminha ao Jurídico para análise e à Autoridade Competente para julgamento

`— LINHA DE INTERAÇÃO —`

**Ações Frontstage** *(visíveis ao Fiscal)*
- Empresa recebe a notificação e protocola defesa dentro do prazo concedido
- Preposto comunica ao fiscal o status da empresa e eventuais medidas saneadoras

`— LINHA DE VISIBILIDADE —`

**Ações Backstage** *(invisíveis ao Fiscal)*
- Jurídico analisa a defesa da empresa, verifica proporcionalidade da sanção e emite parecer
- Autoridade Competente julga o processo e decide pela aplicação ou não da penalidade
- Área Administrativa registra a sanção nos cadastros unificados (SICAF, CEIS, CNEP)

`— LINHA DE INTERAÇÃO INTERNA —`

**Processos de Suporte**
- **SICAF** (Sistema de Cadastramento Unificado de Fornecedores)
- **CEIS** (Cadastro Nacional de Empresas Inidôneas e Suspensas)
- **CNEP** (Cadastro Nacional de Empresas Punidas)
- **SEI:** instrução do processo sancionatório
- Sistemas de jurisprudência e normativos internos

**Normativos:** Lei 14.133/2021, Arts. 155-163 (sanções); Art. 161 (registro no SICAF/CEIS); Lei 14.133/2021, Art. 156 (gradação das sanções)

**⚠ Fail Points**
- **[CRÍTICO]** Ameaças verbais de sanção sem abertura de processo formal: a penalidade prescreve sem instrução → infrator impune e precedente negativo para o contrato
- **[CRÍTICO]** Fiscal sem letramento jurídico mínimo para instruir processo sancionatório: peças deficientes são derrubadas no contraditório
- **[OPERACIONAL]** Prazo de defesa concedido na notificação incompatível com os prazos legais (Lei 14.133, Art. 157) → nulidade processual
- **[OPERACIONAL]** Sanção aplicada mas não registrada nos cadastros (SICAF/CEIS): empresa punida continua habilitada em outros certames

---

### Etapa 8 — Aditivos ou Encerramento

**Evidências Físicas**
- Relatório Técnico de Avaliação do contrato
- Pesquisa de preços atualizada
- Termo Aditivo (prorrogação ou alteração de escopo)
- Ateste de Conclusão Final (encerramento)

**Ações do Fiscal/Gestor**
- Elabora Relatório Técnico avaliativo do contrato: qualidade, ocorrências, riscos e recomendação
- Para prorrogação: justifica a conveniência e oportunidade
- Para encerramento: emite ateste de conclusão e verifica pendências trabalhistas residuais

`— LINHA DE INTERAÇÃO —`

**Ações Frontstage** *(visíveis ao Fiscal)*
- Empresa manifesta formalmente interesse (ou não) na renovação
- Setor de Licitações comunica o resultado da pesquisa de mercado
- Jurídico retorna com o parecer sobre a viabilidade do aditivo

`— LINHA DE VISIBILIDADE —`

**Ações Backstage** *(invisíveis ao Fiscal)*
- Setor de Licitações realiza pesquisa de preços para verificar economicidade da renovação
- Jurídico elabora e valida a minuta do Termo Aditivo
- Financeiro verifica disponibilidade orçamentária e reforça o empenho para o novo período

`— LINHA DE INTERAÇÃO INTERNA —`

**Processos de Suporte**
- **Compras.gov.br:** pesquisa de preços e publicação do aditivo
- **SIAFI:** reforço de empenho para a prorrogação
- **SEI:** instrução e tramitação do processo de aditamento ou encerramento

**Normativos:** Lei 14.133/2021, Arts. 132-136 (aditivos e prorrogações)

**⚠ Fail Points**
- **[CRÍTICO]** Pedido de prorrogação enviado após o vencimento contratual: configura contrato verbal, sem amparo legal → indenização precária e responsabilização do gestor
- **[CRÍTICO]** Prorrogação de contrato deficitário por omissão: relatório favorável emitido para evitar o esforço de nova licitação, mesmo com histórico de infrações
- **[OPERACIONAL]** Encerramento sem verificação de pendências trabalhistas residuais: trabalhadores substituídos sem baixa correta no e-Social
- **[OPERACIONAL]** Pesquisa de preços desatualizada utilizada como base do aditivo: risco de sobrepreço e questionamento pelo TCU

---

## 5. Fluxo de Rastreabilidade — O Caminho do Dinheiro

A Lei 4.320/1964 estabelece uma sequência obrigatória e inviolável. A quebra de qualquer etapa constitui **grave irregularidade financeira**, sujeita a responsabilização por erro grosseiro ou improbidade administrativa.

```
 Execução do Serviço (contratada)
        ↓
 Emissão e Protocolo da Nota Fiscal
        ↓
 Recebimento Provisório — Art. 140, I, Lei 14.133
 (Fiscal Técnico: escopo quanti-qualitativo)
 (Fiscal Administrativo: documentação trabalhista)
        ↓
 Recebimento Definitivo / Ateste — Art. 140, II, Lei 14.133
 (Gestor: declaração formal ao Estado do recebimento do objeto)
        ↓
 Liquidação — Art. 63, Lei 4.320/64
 (Financeiro: averiguação do ateste, retenção de 11% INSS, validação contábil)
        ↓
 Pagamento — Ordem Bancária no SIAFI
 (Ordem cronológica obrigatória — IN SEGES 77/2022)
```

> Qualquer pagamento realizado antes do ateste formal constitui **pagamento antecipado vedado** (ON AGU 76/2023), salvo hipóteses excepcionais fundamentadas.

---

## 6. Pontos Cegos para Investigação Interna

| # | Ponto Cego | Risco Oculto |
| :--- | :--- | :--- |
| **PC-1** | **O "Acordo de Cavalheiros":** fiscal e preposto combinam compensar glosas com horas extras informais, sem registro | Maquiagem da fiscalização; supressão de prova de infrações; responsabilidade pessoal do fiscal por omissão |
| **PC-2** | **A Herança Problemática:** fiscal substituto recebe contrato com histórico de falhas não documentadas | Primeiras 48h de responsabilidade sem base de conhecimento; risco de atestar irregularidades desconhecidas |
| **PC-3** | **O Efeito Carimbador:** Gestor atesta processos complexos (TI, engenharia, saúde) sem capacidade real de auditar | Responsabilidade solidária por ato de gestão sem o devido cuidado objetivo |
| **PC-4** | **Gestão Shadow IT:** servidores usam Trello pessoal, ChatGPT, WhatsApp e planilhas VBA para compensar a dureza dos sistemas do governo | Rastreabilidade zero; perda de evidências em auditoria; decisões baseadas em dados não oficiais |
| **PC-5** | **A CND como Véu:** empresa apresenta CND válida obtida via parcelamento enquanto acumula dívidas com trabalhadores do contrato | Responsabilidade trabalhista subsidiária da União materializada somente após ação judicial |
| **PC-6** | **O Prazo Silencioso da Sanção:** fiscal documenta infração, mas não abre processo de penalidade; infração prescreve no prazo do contrato | Contratada infratora não punida + precedente que estimula reincidência |

---

## 7. Fontes e Base de Evidências Aplicáveis

**Legislação Estrutural**
- Lei nº 14.133/2021 — Lei de Licitações e Contratos Administrativos (Arts. 117-118, 140-145, 155-163)
- Lei nº 4.320/1964 — Normas Gerais de Direito Financeiro (Art. 63 — liquidação)
- Lei nº 8.212/1991 — Custeio da Previdência Social (Art. 31 — retenção de 11%)

**Normas Infralegais**
- Decreto nº 11.246/2022 — Atribuições dos agentes de fiscalização e gestão
- IN SEGES/MP nº 05/2017 — Regras de fiscalização de contratos de terceirização
- IN SEGES/ME nº 77/2022 — Ordem cronológica obrigatória de pagamentos

**Orientações Normativas**
- Orientação Normativa AGU nº 76/2023 — Vedação de pagamento antecipado sem ateste e fundamentação restrita

**Jurisprudência e Controle Externo**
- Súmula 331, V, do TST — *Culpa in vigilando*: responsabilidade subsidiária da Administração por omissão na fiscalização trabalhista
- Acórdão 1.214/2013-Plenário/TCU — Exigências de fiscalização continuada e impactos em contratos de terceirização (DEDMO)

**Sistemas Referenciados**
- SEI (Sistema Eletrônico de Informações) — tramitação processual
- SIAFI (Sistema Integrado de Administração Financeira) — liquidação e pagamento
- Compras.gov.br — dados contratuais e pesquisa de preços
- SICAF / CEIS / CNEP — cadastros de sanções
- e-Social (eventos S-1200, S-2299) — obrigações trabalhistas e previdenciárias
