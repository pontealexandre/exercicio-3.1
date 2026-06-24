Aqui está a pesquisa estruturada para o Service Blueprint AS-IS da Gestão e Fiscalização de Contratos, elaborada sob a dupla ótica de auditoria de conformidade e design de serviços, mapeando a realidade viva da linha de frente da Administração Pública Federal.

## **1\. Sumário Executivo**

A fase de execução contratual na Administração Pública Federal é caracterizada por alta complexidade normativa e severa fragmentação sistêmica. O Fiscal/Gestor de Contrato atua como o principal funil de conformidade do Estado, absorvendo uma carga cognitiva altíssima. A jornada AS-IS revela um serviço onde o usuário precisa transitar constantemente entre sistemas não integrados (SEI, Compras.gov.br, planilhas avulsas) e onde o design das ferramentas não acompanha o rigor da responsabilidade imputada pela Lei 14.133/2021. Observa-se que a gestão ocorre, na prática, de forma reativa: o fiscal é frequentemente sobrecarregado, atua com baixo letramento contratual no início da designação e supre as lacunas sistêmicas através de controles paralelos (e-mails, WhatsApp, pastas no drive local), o que gera altos riscos de auditoria e falhas na rastreabilidade dos atestes.

## **2\. Tabela Mestre do Blueprint (Camadas AS-IS)**

A tabela abaixo sintetiza as cinco raias de visibilidade e suporte para cada etapa da jornada pós-assinatura.

| Etapa da Jornada | Ações do Usuário (Front-stage) | Bastidores (Back-stage) | Evidências (Físico/Digital) | Normativos Aplicáveis | Fail Points Conhecidos |
| :---- | :---- | :---- | :---- | :---- | :---- |
| **1\. Designação e Assunção** | Recebe notificação da portaria e acessa o processo para ler TR, Contrato e Matriz de Riscos. | Setor de Gestão de Pessoas ou Contratos emite portaria e publica em boletim. | Portaria no SEI; Termo de Ciência; TR; Contrato assinado. | Lei 14.133 (Art. 117); Manuais internos de delegação. | Fiscal designado sem ciência prévia, sem capacitação ou com excesso de contratos. |
| **2\. Reunião Inicial (Kick-off)** | Reúne-se com preposto da contratada para alinhar rotinas, entregas e formato de comunicação. | Preposto é oficialmente designado pela empresa; Setor de Contratos apoia se necessário. | Ata de Reunião no SEI; Ofício de indicação do preposto. | Lei 14.133 (Art. 118); IN SEGES aplicável à terceirização. | Falta de registro formal dos acordos operacionais; ausência do Gestor. |
| **3\. Acompanhamento e Rotina** | Mede SLA/IMR, verifica execução local e registra ocorrências positivas e negativas. | Contratada executa o serviço; Fiscais setoriais enviam relatos ao Fiscal Técnico. | Planilhas de medição; E-mails; Relatórios no módulo Contratos (Compras.gov.br). | Lei 14.133 (Art. 117, §1º); Princípio da Segregação de Funções. | Acompanhamento "de gaveta" sem registro sistêmico; comunicação informal (WhatsApp). |
| **4\. Recebimento Provisório** | Recebe NF/Relatório da empresa, confere quantitativos/qualidade e assina Termo Provisório. | Fiscal Administrativo (se houver) confere regularidade fiscal, INSS e FGTS da empresa. | Termo de Recebimento Provisório; Relatório de Medição; CNDs válidas. | Lei 14.133 (Art. 140, I); Manuais TCU sobre recebimento. | Assinatura por pressão de prazo sem conferência real de qualidade ou CNDs vencidas. |
| **5\. Rec. Definitivo e Ateste** | Gestor avalia relatório do fiscal, emite Termo Definitivo e carimba/assina atesto na Nota Fiscal. | Gestor de Contratos consolida dados técnicos e administrativos para liberar ateste. | Termo de Recebimento Definitivo; Nota Fiscal Atestada (carimbo digital SEI). | Lei 14.133 (Art. 140, II); Lei 4.320/64 (Art. 63). | Ateste de serviços não prestados na totalidade ou ateste "cego" (Gestor que só assina). |
| **6\. Encaminhamento e Pagamento** | Autua documentos de cobrança no SEI e despacha para o setor financeiro. | Setor Financeiro liquida a despesa no SIAFI e Ordenador autoriza Ordem Bancária (OB). | Despacho de encaminhamento; Nota de Lançamento (NL) e OB no SIAFI. | Lei 4.320/64 (Liquidação); INs da STN (Secretaria do Tesouro Nacional). | Atraso no envio pelo fiscal gerando multas moratórias para a Administração. |
| **7\. Ocorrências e Sanções** | Notifica empresa sobre falhas não sanadas e autua processo apartado para penalidade. | Consultoria Jurídica (AGU) analisa devido processo; Autoridade Competente julga. | Notificação extrajudicial; Defesa prévia; Relatório de instrução de penalidade. | Lei 14.133 (Arts. 155 a 163 \- Infrações e Sanções). | Ameaça de sanção verbal sem autuação de processo; prescrição da penalidade. |
| **8\. Aditivos ou Encerramento** | Emite relatório técnico justificando renovação (com pesquisa de preço) ou atesta entrega final. | Setor de Contratos instrue repactuação/aditivo; Jurídico emite parecer; Financeiro ajusta empenho. | Relatório de Avaliação do Contrato; Termo Aditivo; Estudo Técnico de renovação. | Lei 14.133 (Arts. 132 a 136 \- Alteração dos Contratos e Preços). | Pedido de aditivo intempestivo (após vencimento do contrato), gerando contrato verbal nulo. |

## **3\. Detalhamento Narrativo por Etapa**

### **Etapa 1 e 2: O Desembarque e o Alinhamento (O Gatilho)**

A jornada do Fiscal raramente começa no planejamento; ele "herda" o contrato. O **gatilho** é uma notificação no SEI com a portaria de designação. O ritmo inicial é de alta carga cognitiva. O fiscal precisa desvendar a Matriz de Riscos, o Termo de Referência (TR) e a proposta vencedora. Ocorre frequentemente a Reunião de Kick-off, que é vital, mas muitas vezes negligenciada. Quando feita, resulta em uma Ata que define como as Ordens de Serviço (OS) ou solicitações serão enviadas ao preposto.

* **Zona de Atrito:** A falta de tempo hábil para o fiscal se apropriar do histórico da licitação antes de precisar aprovar a primeira medição.

### **Etapa 3: Acompanhamento da Execução (O Cotidiano)**

Este é o trabalho diário ou semanal. O fiscal realiza inspeções visuais, testes de software, ou mede a disponibilidade de postos de trabalho. Ele usa o Instrumento de Medição de Resultado (IMR) ou SLA.

* **Tempo/Ritmo:** Contínuo.  
* **Zona de Atrito:** Ausência de ferramentas mobile integradas. O fiscal faz anotações em cadernos ou planilhas Excel próprias, enviando mensagens ao preposto via WhatsApp, o que destrói a trilha de auditoria (evidência invisível ao back-stage). O registro no Compras.gov.br costuma ser feito de forma retroativa, apenas "para cumprir tabela".

### **Etapa 4 e 5: O Rito de Recebimento (O Gargalo Mensal)**

O **gatilho** é a entrega do objeto ou a virada do mês (serviços contínuos). A contratada envia o relatório e a Nota Fiscal. Inicia-se a segregação de funções exigida em lei:

1. O **Fiscal Técnico** atesta que o serviço foi prestado com a qualidade exigida (Termo Provisório).  
2. O **Fiscal Administrativo** verifica o recolhimento de impostos e obrigações trabalhistas.  
3. O **Gestor do Contrato** consolida ambos e emite o Termo Definitivo.  
* **Zona de Atrito:** A pressão das contratadas e do setor financeiro ("o pagamento precisa sair até o 5º dia útil") faz com que muitas inconsistências sejam toleradas. O ateste é a fase de maior risco jurídico pessoal para o servidor.

### **Etapa 6, 7 e 8: Manutenção, Sanção e Encerramento**

Enquanto o pagamento é processado no SIAFI pelo back-stage, o fiscal continua o ciclo. Caso haja reincidência de falhas apontadas na Etapa 3, o fiscal atua no papel coercitivo (Etapa 7), instruindo penalidades. Ao fim de 12 meses (ou do cronograma), o **gatilho** de encerramento exige que ele produza relatórios avaliativos que justifiquem a prorrogação ou o ateste final, baseando a decisão do Ordenador de Despesa.

## **4\. Fluxo de Rastreabilidade (O Caminho do Dinheiro)**

O fluxo de despesa pública segue um rito estrito legal e contábil. A quebra dessa sequência (como pagar antes de liquidar) constitui crime de responsabilidade. Abaixo está a sequência desde a aprovação física até o repasse bancário:

**1.Emissão e Envio da Nota Fiscal:**Ação: Contratada.  
A empresa prestadora protocola a NF e o Relatório de Medição correspondente ao período executado, acompanhados das Certidões Negativas de Débito (CNDs).

**2.Recebimento Provisório e Definitivo:**Ação: Equipe de Fiscalização (Front-stage).  
Os fiscais validam quantitativos, aplicam eventuais glosas (descontos por não atingimento de SLA) e geram os Termos de Recebimento.

**3.Ateste do Documento Fiscal:**Ação: Gestor do Contrato.  
Ocorre a aposição do "Carimbo de Atesto" digital no SEI diretamente sobre a NF, declarando, sob as penas da lei, que o objeto foi recebido a contento. O processo é despachado.

**4.Liquidação da Despesa:**Ação: Setor Financeiro no SIAFI (Back-stage).  
O Financeiro confere formalmente o ateste e as CNDs. No sistema SIAFI, converte o Empenho em Liquidação (reconhecendo que o Estado agora deve efetivamente aquele valor).

**5.Emissão da Ordem Bancária (OB):**Ação: Ordenador de Despesa (Back-stage).  
Com a despesa liquidada, o Ordenador autoriza o pagamento, gerando a Ordem Bancária no SIAFI que transfere o recurso da Conta Única do Tesouro para a empresa.

## **5\. Pontos Cegos para Investigação Interna (Destilação)**

Durante o mapeamento futuro com os atores reais, a equipe de design de serviço deve focar nestas zonas de sombra que as documentações não revelam:

1. **O "Acordo de Cavalheiros":** Como falhas pontuais da contratada são compensadas na prática sem gerar glosa ou registro em sistema? (Ex: a empresa falha hoje, mas promete fazer horas extras não cobradas amanhã).  
2. **A Herança de Contratos Problemáticos:** O que ocorre nas primeiras 48 horas quando um fiscal substituto é nomeado no meio de uma crise contratual e a gestão anterior não deixou registros sistêmicos, apenas na própria memória?  
3. **Uso de IA e Ferramentas Shadow IT:** Até que ponto os fiscais já utilizam ferramentas não homologadas (scripts locais, IA generativa comercial para redigir notificações ou planilhas macro no Excel) para superar a interface legada dos sistemas de governo?  
4. **O Efeito "Carimbador":** Qual é a real capacidade do Gestor de Contrato de discordar do Fiscal Técnico na Etapa 5? Na prática, o Gestor muitas vezes apenas endossa, sem ler, devido ao volume de processos.

## **6\. Fontes e Base de Evidências Aplicáveis**

* **Legislação:** Lei nº 14.133/2021 (Nova Lei de Licitações e Contratos); Lei nº 4.320/1964 (Estatuto Financeiro).  
* **Normas Infralegais (Poder Executivo Federal):** IN SEGES/MP nº 05/2017 e IN SEGES/ME nº 81/2022 (Terceirização e Serviços); Decreto nº 11.246/2022 (Regras de atuação dos agentes de contratação e fiscais).  
* **Jurisprudência Correlata (TCU):** Súmula 261/TCU (Vedação de pagamento antecipado sem ateste); Acórdão 1.214/2013-Plenário e Acórdão 1.186/2017-Plenário (Responsabilidade do fiscal e estrutura de trabalho).  
* **Modelos Padronizados:** Manuais e listas de verificação da Advocacia-Geral da União (AGU) e Secretaria de Gestão e Inovação (SEGES).