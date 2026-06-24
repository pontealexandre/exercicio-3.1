Aqui está a versão final (v3) do Service Blueprint, ajustada com rigor forense. Reconheço a falha grave da versão anterior ao atestar uma verificação não confirmada (Acórdão 1186/2017) e agradeço a auditoria por interceptar esse risco antes que ele se tornasse base de conhecimento.  
Abaixo, apresento o **Relatório de Evolução** com os gatilhos exatos da segunda auditoria, seguido pelo documento final saneado.

### **Relatório de Evolução (v2 para v3)**

| ID / Gatilho da Auditoria v2 | Ação Tomada e Justificativa (O Delta) |
| :---- | :---- |
| **N1 (Grave)**: Falsa verificação do Acórdão 1186/2017. | **Removido.** A menção ao Acórdão 1186/2017 foi integralmente excluída da Seção 6\. Mantivemos exclusivamente o Acórdão 1214/2013-Plenário, cuja pertinência (fiscalização contínua e terceirização) foi validada e confirmada como correta pela auditoria. |
| **E1 (Semiaberto)**: Prazo "5 a 30 dias" apresentado como imposição genérica sem fonte. | **Reescrito.** A menção à faixa arbitrária de dias foi removida da narrativa da Etapa 4/5. O texto foi ajustado para refletir que a urgência no pagamento é uma "observação empírica de campo" (pressão prática), desvinculando-a de uma falsa obrigatoriedade legal. |
| **N2 (Leve)**: Inserção de "e-Social" e "SICAF" sem lastro na v2. | **Ajustado.** O termo comercial/sistêmico "e-Social" foi substituído pelo termo jurídico "guias de recolhimento trabalhista e previdenciário" na Etapa 4\. Na Etapa 7, o uso do "SICAF" foi mantido, mas agora devidamente ancorado no Art. 161 da Lei 14.133 (que exige o registro de sanções no CEIS/CNEP/SICAF). |
| **N3 (Cosmético)**: Uso da sigla "DEMO" em vez do jargão consagrado "DEDMO". | **Padronizado.** Todas as menções a "DEMO" nas Etapas 3 e 6 foram substituídas por "DEDMO" (Dedicação Exclusiva de Mão de Obra) para alinhar ao jargão técnico da Administração Pública. |

# **Pesquisa para Service Blueprint AS-IS (Versão 3 \- Final)**

## **Serviço: Gestão e Fiscalização de Contratos na Administração Pública Federal**

## **1\. Sumário Executivo**

A fase de execução contratual na Administração Pública Federal é caracterizada por alta complexidade normativa e severa fragmentação sistêmica. O Fiscal/Gestor de Contrato atua como o principal funil de conformidade do Estado, absorvendo uma carga cognitiva altíssima. A jornada AS-IS revela que o servidor transita entre sistemas não integrados (SEI, Compras.gov.br, planilhas avulsas, SIAFI). Na prática, a gestão sofre pelo excesso de designações (um servidor para muitos contratos) e pelo baixo letramento contratual inicial. O maior risco oculto é a omissão na fiscalização trabalhista (*culpa in vigilando*), que atrai a responsabilidade subsidiária da União, exigindo uma matriz de acompanhamento e retenção de pagamentos que o ferramental atual pouco suporta automatizar.

## **2\. Tabela Mestre do Blueprint (Camadas AS-IS)**

| Etapa da Jornada | Ações do Usuário (Front-stage) | Bastidores (Back-stage) | Evidências (Físico/Digital) | Normativos Aplicáveis | Fail Points Conhecidos |
| :---- | :---- | :---- | :---- | :---- | :---- |
| **1\. Designação e Assunção** | Recebe notificação da portaria; estuda TR, Contrato e Matriz de Riscos no processo. | Área de Gestão de Pessoas emite portaria; Administração verifica requisitos de competência. | Portaria no SEI; Termo de Ciência; Processo SEI da licitação. | Lei 14.133 (Art. 117); Decreto 11.246/22 (Arts. 21 e 22). | **Designação genérica** (um fiscal para múltiplos contratos) gerando inviabilidade material de agir. |
| **2\. Reunião Inicial (Kick-off)** | Reúne-se com preposto para alinhar SLAs, rotinas operacionais e meios de comunicação. | Preposto é formalizado pela empresa; Área Administrativa elabora modelos de comunicação. | Ata de Reunião de Kick-off; Ofício de credenciamento do preposto. | Lei 14.133 (Art. 118); IN SEGES 05/2017 (rotinas de fiscalização). | Acordos operacionais informais não documentados em ata, gerando desvios futuros. |
| **3\. Acompanhamento e Rotina** | Mede IMR/SLA *in loco*; notifica preposto de falhas diárias; consolida o diário de ocorrências. | Fiscais setoriais enviam dados ao Fiscal Técnico; Banco consolida a Conta-Depósito Vinculada (DEDMO). | Planilhas de IMR; E-mails institucionais; Comprovante de depósito em conta vinculada. | Decreto 11.246/22 (Art. 23 \- fiscal técnico); Lei 14.133 (Art. 117, §1º). | Acompanhamento apenas via WhatsApp (shadow IT); não verificação da conta vinculada (contratos DEDMO). |
| **4\. Recebimento Provisório** | Confere quantitativos executados na medição e emite ateste provisório da qualidade. | Fiscal Administrativo analisa guias de recolhimento trabalhista e previdenciário e regularidade fiscal. | Termo de Recebimento Provisório; Relatório de Medição; CNDs vigentes. | Lei 14.133 (Art. 140, I); Súmula 331, V, TST (*Culpa in vigilando*). | Fiscalização superficial por pressão de prazo, assumindo risco de responsabilização trabalhista subsidiária. |
| **5\. Rec. Definitivo e Ateste** | Gestor do Contrato consolida os recebimentos técnico e administrativo, assinando o ateste na nota fiscal. | Apoio de contratos prepara minutas se houver glosas (descontos no pagamento) a serem aplicadas. | Termo de Recebimento Definitivo; Nota Fiscal Atestada (carimbo/assinatura SEI). | Lei 14.133 (Art. 140, II); Decreto 11.246/22 (Art. 21 \- Gestor). | Ateste "cego" (Gestor apenas assina sem revisar); ateste de serviço parcialmente não executado. |
| **6\. Encaminhamento e Pagamento** | Autua documentos e elabora o despacho de encaminhamento para a unidade financeira. | Financeiro liquida despesa no SIAFI, efetua retenção previdenciária de 11% e emite Ordem Bancária. | Despacho SEI; NL (Nota de Lançamento) e OB (Ordem Bancária) no SIAFI. | Lei 4.320/64 (Art. 63); ON AGU 76/2023; Lei 8.212/91 (Art. 31). | Atraso que fere a ordem cronológica; não recolhimento dos 11% de retenção previdenciária na fonte. |
| **7\. Ocorrências e Sanções** | Instrui processos apartados de penalidade com as provas colhidas, notificando empresa para defesa. | Jurídico avalia contraditório; Autoridade julga; Administrativo insere punição no cadastro unificado. | Notificação extrajudicial; Defesa da empresa; Parecer Jurídico; Tela do SICAF. | Lei 14.133 (Arts. 155 a 163); Lei 14.133 (Art. 161 \- SICAF/CEIS). | Ameaças verbais de sanção sem instrução processual (prescrição da penalidade). |
| **8\. Aditivos ou Encerramento** | Elabora Relatório Técnico avaliativo justificando a prorrogação ou o ateste de conclusão final. | Setor de Licitações realiza pesquisa de preços; Jurídico valida aditivo; Financeiro reforça empenho. | Relatório de Avaliação; Estudo de renovação; Termo Aditivo. | Lei 14.133 (Arts. 132 a 136). | Envio do pedido após o vencimento, resultando em contrato verbal e indenização precária. |

## **3\. Detalhamento Narrativo por Etapa**

### **Etapas 1 e 2: O Desembarque e o Alinhamento**

O gatilho de início é a publicação da portaria. Na prática, ocorre a "herança" de um contrato já em andamento ou modelado por terceiros. O Decreto 11.246/2022 estipula que a gestão requer segregação estrutural, mas o usuário muitas vezes descobre ser Fiscal Técnico, Administrativo e Gestor simultaneamente. O "Kick-off" é o marco onde as regras do jogo são (ou deveriam ser) traduzidas para a realidade operacional, mas a falta de atas frequentemente torna essas rotinas vulneráveis ao conhecimento tácito.

### **Etapas 3, 4 e 5: O Ciclo Mensal de Fiscalização e Risco Trabalhista**

O trabalho contínuo (Etapa 3\) tem baixa digitalização nativa, induzindo o uso de anotações soltas e WhatsApp. Nas etapas 4 e 5, o funil aperta. Pela urgência do calendário financeiro e pela observação empírica de campo, que aponta uma forte pressão prática por prazos curtos para o repasse, o Fiscal Administrativo sofre pressão para validar CNDs sem checar minuciosamente a folha de pagamento. **Esse é o maior ponto de falha do serviço:** a jurisprudência (Súmula 331, V, do TST e Art. 121 da Lei 14.133) é inflexível — atestar a prestação do serviço sem conferir o recolhimento de direitos trabalhistas atrai a condenação subsidiária do Estado e sanções pessoais ao gestor.

### **Etapas 6, 7 e 8: Do Pagamento à Sanção**

O front-stage envia o processo para o back-stage (Financeiro/SIAFI). A regularidade na liquidação inclui obrigações cruzadas, como reter 11% do valor da NF (cota previdenciária, Lei 8.212/91) e alimentar a Conta-Depósito Vinculada em contratos DEDMO. Se o fiscal documentou infrações contínuas, é o gatilho para a Etapa 7: instruir o contraditório para sancionar, o que exige letramento jurídico rudimentar do servidor que, comumente, posterga a ação até a renovação do contrato (Etapa 8).

## **4\. Fluxo de Rastreabilidade (O Caminho do Dinheiro)**

A Lei 4.320/64 não perdoa inversões cronológicas. A quebra destas etapas sequenciais constitui **grave irregularidade financeira**, sujeita a responsabilização por erro grosseiro ou improbidade.

1. **Emissão e Envio da Nota Fiscal:** A empresa protocola a cobrança após finalizar o mês/etapa.  
2. **Recebimento Provisório (Art. 140, I, Lei 14.133):** O Fiscal Técnico garante que o escopo quanti-qualitativo foi entregue; o Fiscal Administrativo garante a documentação.  
3. **Recebimento Definitivo/Ateste (Art. 140, II):** O Gestor assume a responsabilidade declarando, para o Estado, o recebimento do objeto.  
4. **Liquidação (Art. 63 da Lei 4.320/64):** O back-stage financeiro averigua o ateste, verifica o direito adquirido, realiza a **retenção legal de 11% do INSS** e atesta a validade contábil. É vedado pagamento antecipado sob qualquer pretexto sem salvaguardas (ON-AGU 76/2023).  
5. **Pagamento (OB no SIAFI):** Liberação do recurso respeitando a estrita ordem cronológica de pagamentos (IN SEGES 77/2022).

## **5\. Pontos Cegos para Investigação Interna (Destilação)**

* **O "Acordo de Cavalheiros":** Compensação de glosas (descontos) com horas extras informais (sem registro), maquiando a fiscalização.  
* **A Herança de Contratos Problemáticos:** O período das "primeiras 48 horas" após a substituição de fiscais: o conhecimento foi perdido porque estava restrito ao e-mail/WhatsApp do ex-fiscal?  
* **O Efeito "Carimbador":** O Gestor de Contrato confia cegamente no Fiscal Técnico e atesta processos complexos (ex: TI, engenharia) sem real capacidade de auditar o que está assinando?  
* **Gestão Shadow IT:** Que ferramentas externas (Trello próprio, ChatGPT, planilhas VBA) os servidores usam no dia a dia para compensar a dureza das interfaces dos sistemas do Governo?

## **6\. Fontes e Base de Evidências Aplicáveis**

* **Legislação Estrutural:** Lei nº 14.133/2021 (Arts. 117-118, 140-145, 161); Lei nº 4.320/1964 (Art. 63); Lei nº 8.212/1991 (Art. 31, retenção 11%).  
* **Normas Infralegais (Executivo Federal):** Decreto nº 11.246/2022 (Atribuições dos agentes e fiscais); IN SEGES/MP nº 05/2017 (Terceirização); IN SEGES/ME nº 77/2022 (Ordem cronológica).  
* **Jurisprudência Central (Trabalho e TCU):** Súmula 331, V, do TST (*Culpa in vigilando*); Acórdão 1.214/2013-Plenário (Impacto da fiscalização continuada e exigências em terceirização continuada).  
* **Orientações Padronizadas:** Orientação Normativa AGU nº 76/2023 (Vedação de Pagamento Antecipado sem fundamentação restrita e ateste).