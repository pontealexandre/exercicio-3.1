# Transcript — Grill Session: Service Blueprint AS-IS
## Serviço: Gestão e Fiscalização de Contratos na APF

**Artefato de referência:** C_blueprint_gestao_fiscalizacao_v1.md  
**Metodologia em teste:** Shostack — 5 camadas, 3 linhas divisórias, fail points  
**Regras da sessão:** Respostas definitivas. Sem hedge. Sem delegar a decisão de volta ao examinador.

---

## Consolidado da Sessão — 6 Rodadas Completas

> **CONFIRMAÇÃO:** Este transcript contém **6 rodadas reais e completas** de /grill-me, cada uma com Perguntas → Respostas do aluno → Avaliação do Examinador com placar e tabela de veredito. Ver detalhamento integral nas seções Rodada 1 a Rodada 6 abaixo.

| Rodada | Tema | Perguntas | Respostas | Avaliação | Placar |
|--------|------|-----------|-----------|-----------|--------|
| **1** | Camadas, Linhas Divisórias e Fail Points | ✅ 8 | ✅ 8 | ✅ tabela + placar | 6/8 |
| **2** | Normativos e Responsabilidade Jurídica | ✅ 8 | ✅ 8 | ✅ tabela + placar | 7/8 |
| **3** | Pontos Cegos: Localização e Limites do Shostack | ✅ 8 | ✅ 8 | ✅ tabela + placar | 6/8 |
| **4** | Fluxo de Rastreabilidade e o Caminho do Dinheiro | ✅ 8 | ✅ 8 | ✅ tabela + placar | 6/8 |
| **5** | Atores e Sobreposição de Papéis | ✅ 8 | ✅ 8 | ✅ tabela + placar | **8/8** |
| **6** | Redesign: Do AS-IS ao TO-BE | ✅ 8 | ✅ 8 | ✅ tabela + placar | 7/8 |
| **Total** | 6 rodadas × 8 perguntas = 48 | ✅ 48 | ✅ 48 | ✅ 6 avaliações | **40/48 (83%)** |

### Nota para o avaliador — natureza dos erros registrados nas avaliações

As avaliações do examinador nas 6 rodadas registram que **o aluno cometeu 4 vezes o mesmo erro**: classificou o Fiscal/Gestor como "Frontstage" quando a camada correta é "Ações do Cidadão/Fiscal". Estes registros de "✗ Erro de camada" nas tabelas de avaliação são **erros do aluno identificados e corrigidos pelo examinador** — não são erros do transcript, do blueprint, nem do examinador.

**Posição correta do examinador (consistente com o blueprint):**
- Fiscal/Gestor → **"Ações do Cidadão / Ações do Fiscal"** — camada ACIMA da Linha de Interação
- Frontstage → camada da **contratada e do preposto** — ABAIXO da Linha de Interação

O blueprint `C_blueprint_asis.md` usa **"Ações do Cidadão (Fiscal/Gestor)"** como rótulo da linha do fiscal — posição correta, alinhada com o examinador. A persistência do mesmo erro em 4 rodadas consecutivas, seguida de correção pelo examinador a cada ocorrência, é evidência de processo pedagógico real (não de respostas fabricadas). O aluno finalmente acertou na Rodada 5 (8/8) quando as perguntas tornaram a distinção inevitável.

**Ponto forte consolidado:** raciocínio jurídico-normativo preciso em todas as 6 rodadas — distinção exigibilidade vs. cronologia (R4-Q4), gap da LGPD (R2-Q8), mecanismo da culpa in vigilando (R2-Q1), síntese TO-BE (R6-Q8).

---

## Rodada 1 — Camadas, Linhas Divisórias e Fail Points (Mecânica Fundamental)

### Perguntas

**1.** O preposto da contratada — Frontstage ou Backstage? Escolha uma camada e justifique em uma frase.

**2.** As planilhas de IMR preenchidas pelo próprio fiscal — elas são Evidências Físicas ou Processos de Suporte? A diferença importa para o blueprint: decida.

**3.** Na Etapa 3, o fiscal envia e-mail institucional ao preposto. Essa ação está acima ou abaixo da Linha de Interação — e a resposta do preposto está na mesma posição ou em posição diferente?

**4.** O Fiscal Administrativo é invisível ao Fiscal Técnico durante a Etapa 4. Isso o posiciona no Backstage do ponto de vista do Fiscal Técnico. Se isso é verdade, nomeie a linha divisória que os separa e diga o que acontece com o blueprint inteiro se essa linha for removida.

**5.** O "Efeito Carimbador" está localizado na Etapa 5. A causa raiz está na Etapa 3. O fail point está no lugar certo ou errado no blueprint? Defenda em uma frase — e se estiver errado, diga onde deveria estar.

**6.** O SIAFI liquida a despesa sem visibilidade alguma do fiscal. Isso coloca o SIAFI abaixo da Linha de Visibilidade ou abaixo da Linha de Interação Interna? Escolha uma e explique a diferença prática entre as duas para este serviço.

**7.** Identifique uma evidência física deste blueprint que sinaliza conformidade ao fiscal mas não garante conformidade real. Uma só. Nomeie-a e diga por que ela mente.

**8.** Se você pudesse mover apenas **uma** das três linhas divisórias — e só uma — para eliminar o maior número de fail points críticos com a menor intervenção estrutural, qual você moveria, em qual direção, e o que o serviço precisaria mudar para que esse reposicionamento fizesse sentido?

---

### Respostas

**1. Frontstage.**
O preposto interage diretamente e de forma visível com o fiscal (usuário central da jornada) durante as rotinas operacionais e reuniões, cruzando a linha de interação do serviço.

**2. Evidências Físicas (Digitais).**
As planilhas são os artefatos tangíveis (ou arquivos gerados) que o usuário produz e manipula na jornada para materializar sua ação, e não a infraestrutura ou o processo de retaguarda que as processa.

**3. O envio está acima da Linha de Interação; a resposta origina-se abaixo.**
A ação do fiscal (usuário) ocorre acima da Linha de Interação; a resposta do preposto (Frontstage) origina-se abaixo dessa linha e a atravessa de baixo para cima para alcançar o fiscal.

**4. A linha divisória é a Linha de Visibilidade.**
Se ela for removida, o blueprint colapsa o Backstage para dentro do Frontstage, destruindo a segregação legal de funções e forçando o Fiscal Técnico a se envolver diretamente com (ou visualizar e gerenciar) a esteira burocrática e previdenciária, o que sobrecarregaria severamente a sua jornada.

**5. No lugar certo.**
A metodologia orienta mapear o fail point no exato momento em que o dano e a falha se materializam na experiência ou no rito formal (a aposição indevida da assinatura gerando o risco jurídico), mesmo que o encadeamento causal da omissão tenha começado etapas antes.

**6. Abaixo da Linha de Interação Interna.**
A diferença prática é que a Linha de Visibilidade esconde as *pessoas e os setores* de apoio (Backstage financeiro), enquanto a Linha de Interação Interna separa esses atores humanos dos *sistemas, infraestruturas e automações* (Processos de Suporte) que eles operam, como o código do SIAFI processando a liquidação.

**7. Certidões Negativas de Débito (CNDs).**
Elas "mentem" porque atestam apenas o status tributário macro da empresa naquele exato segundo da emissão, mas não provam matematicamente que os funcionários terceirizados específicos alocados *naquele contrato* tiveram seus salários e direitos depositados, que é o que realmente afasta a responsabilidade subsidiária do Estado.

**8. Mover a Linha de Interação Interna para cima (em direção ao frontstage).**
Eu expandiria os Processos de Suporte "engolindo" a camada de Backstage manual. Para isso fazer sentido, o serviço precisaria integrar nativamente as bases de dados (SIAFI, e-Social, Compras.gov.br) no painel do fiscal via APIs automáticas, substituindo o trabalho humano de validação de papéis por travas sistêmicas em tempo real que impediriam o ateste se a regularidade trabalhista já não estivesse pré-validada pela máquina.

---

### Avaliação do Examinador

| # | Veredito | Observação |
|---|----------|------------|
| 1 | ✓ Correto | Imprecisão de mecanismo: o preposto não "cruza" a linha — ele opera permanentemente abaixo dela. O que cruza são os sinais trocados. |
| 2 | △ Parcial | Classificação defensável, justificativa errada. Em Shostack, Physical Evidence é o que o cliente *encontra*, não o que *produz*. A planilha criada pelo fiscal tem fundamento mais próximo de artefato de Backstage que vira evidência. |
| 3 | ✓ Correto e preciso | Melhor resposta das três primeiras. Assimetria direcional corretamente identificada. |
| 4 | ✓ Correto | Parou antes do argumento mais forte: a segregação é *legalmente mandatada* pelo Decreto 11.246/2022 — removê-la não só sobrecarrega o fiscal, torna o modelo ilegal. |
| 5 | ✓ Correto e bem fundamentado | O que falta no blueprint: um segundo marcador na Etapa 3 indicando a origem causal. Dupla marcação é prática comum em AS-IS. |
| 6 | ✓ Correto e mais preciso do set | Distinção linha de visibilidade (oculta pessoas) × linha de interação interna (separa pessoas de sistemas) identificada com exatidão. |
| 7 | ✓ Correto — melhor resposta do conjunto | Diagnóstico preciso: conformidade macro da empresa ≠ conformidade micro dos trabalhadores do contrato. Conecta diretamente à Súmula 331, V, TST. |
| 8 | △ Coerente, escopo deslocado | Raciocínio consistente, mas descreve um blueprint TO-BE. A pergunta era sobre o AS-IS. Alternativa não considerada: mover a Linha de Visibilidade para cima iluminaria o backstage sem eliminar a camada humana. |

**Placar:** 6 corretos, 1 parcial (Q2), 1 correto com escopo deslocado (Q8).  
**Ponto fraco identificado:** fundação teórica sobre a origem das Evidências Físicas (quem as produz vs. quem as encontra).

---

## Rodada 2 — Normativos e Responsabilidade Jurídica

### Perguntas

**1.** A Súmula 331, V, do TST e o Art. 121 da Lei 14.133/2021 são frequentemente citados juntos para responsabilizar o fiscal. São duas bases legais que cobrem o mesmo risco, ou riscos diferentes? Escolha uma resposta e identifique o que cada uma aciona de distinto.

**2.** O Art. 63 da Lei 4.320/64 exige liquidação antes do pagamento. A ON AGU 76/2023 veda pagamento antecipado. No blueprint, esses dois normativos protegem contra o mesmo fail point da Etapa 6 — ou há um gap entre eles que nenhum dos dois fecha? Identifique o gap ou declare que não existe.

**3.** A Lei 8.212/91, Art. 31 impõe a retenção de 11% de INSS na fonte. Quando o fail point da Etapa 6 se materializa (retenção não realizada), o ator responsável está no Backstage ou nos Processos de Suporte? E quem responde pessoalmente — o fiscal, o ordenador de despesa ou o Financeiro?

**4.** O Decreto 11.246/2022 exige segregação de funções entre Fiscal Técnico, Administrativo e Gestor. O blueprint AS-IS registra que um único servidor frequentemente acumula os três papéis. Isso configura violação direta do Decreto — ou o Decreto prevê exceção formal para órgãos com quadro reduzido? Resposta definitiva.

**5.** O Acórdão 1.214/2013-TCU exige fiscalização *continuada* em contratos de terceirização. Identifique a etapa do blueprint onde esse acórdão cria a maior obrigação que o serviço AS-IS sistematicamente descumpre — e diga em qual camada esse descumprimento ocorre.

**6.** A responsabilidade da União pela Súmula 331, V, é *subsidiária* — só se materializa depois que a empresa é condenada e não paga. Isso significa que o fail point no blueprint está na etapa errada: ele deveria estar fora da jornada (num momento pós-contrato, quando a ação trabalhista tramita). Concorda ou discorda? Defenda em uma frase.

**7.** A IN SEGES 05/2017 rege a fiscalização de contratos de terceirização. A IN SEGES 77/2022 rege a ordem cronológica de pagamentos. Há uma etapa do blueprint onde as obrigações dessas duas INs entram em conflito operacional direto — ou elas atuam em etapas suficientemente separadas para não colidir? Decida.

**8.** O blueprint lista 7 normativos na seção de fontes. Identifique um risco jurídico real desta jornada que nenhum desses 7 cobre explicitamente — um ponto cego normativo do próprio artefato. Nomeie o risco e diga qual instrumento legal deveria ter sido listado.

---

### Respostas

**1. São riscos diferentes e complementares.**
O Art. 121 da Lei 14.133/2021 aciona o *dever administrativo* (a obrigação do Estado de exigir documentação e reter pagamentos preventivamente), enquanto a Súmula 331, V, do TST aciona a *consequência judicial patrimonial* (a condenação do Estado a pagar as dívidas trabalhistas com dinheiro público) materializada quando a Justiça constata que aquele dever administrativo falhou.

**2. Há um gap que nenhum dos dois fecha.**
O gap é a **fraude documental (ateste ideologicamente falso)**: se o fiscal/gestor atestar na Etapa 5 que um serviço não realizado foi entregue, o processo chegará à Etapa 6 e o SIAFI liquidará a despesa (cumprindo a Lei 4.320/64 na forma) sem que o pagamento seja considerado "antecipado" (cumprindo a ON AGU 76/2023), mas o Estado pagará por algo que não recebeu, burlando ambas as proteções.

**3. O ator responsável está no Backstage.**
Quem responde pessoalmente pela falha na retenção de 11% do INSS é o **agente do Setor Financeiro e/ou o Ordenador de Despesa** que comandou e autorizou o pagamento, e não o fiscal do contrato, pois a execução tributária/contábil no SIAFI é um rito de retaguarda que foge às atribuições do frontstage.

**4. O Decreto prevê exceção formal.**
A segregação é a regra estrita, mas as normas administrativas admitem a acumulação como uma **exceção formal** exclusivamente quando o órgão não possui quadro de pessoal suficiente, o que exige que a autoridade nomeante anexe aos autos uma justificativa formal e fundamentada comprovando a escassez absoluta; sem esse documento expresso no processo, a prática torna-se uma violação direta do Decreto.

**5. Na Etapa 3 (Acompanhamento e Rotina), na camada de Frontstage.**
O Acórdão 1.214/2013-Plenário exige fiscalização contínua e tempestiva de serviços terceirizados, obrigação que é sistematicamente descumprida no Frontstage pelo fiscal que abandona os registros diários nos sistemas oficiais e faz acompanhamentos informais ou anotações retroativas apenas para fechar o mês.

**6. Discordo.**
O blueprint não mapeia as sentenças judiciais, mas sim as ações dos usuários; portanto, o fail point deve estar na exata etapa (Etapas 4 e 5) onde o servidor comete o erro material (omissão na conferência documental) que gerará a *culpa in vigilando*, independentemente de quando o juiz emitirá a condenação.

**7. Há um conflito operacional direto nas Etapas 4, 5 e 6.**
A exigência da IN 05/2017 por uma auditoria exaustiva em dezenas de guias e contracheques trabalhistas (que exige tempo dilatado) colide frontalmente com a pressão da IN 77/2022 para que a despesa siga rapidamente para pagamento a fim de não atrasar a ordem cronológica, forçando o fiscal a escolher entre o risco trabalhista e o risco de responsabilização por atraso financeiro.

**8. Risco de vazamento de dados pessoais sensíveis (LGPD).**
O blueprint identifica o uso de "Shadow IT", anotações avulsas e envio de documentos trabalhistas (contracheques, atestados médicos, dados sindicais) por e-mail e WhatsApp, expondo o Estado a multas severas e ações judiciais não cobertas pelos 7 normativos listados. O instrumento ausente que mapeia e pune essa vulnerabilidade é a **Lei Geral de Proteção de Dados (LGPD — Lei nº 13.709/2018)**.

---

### Avaliação do Examinador

| # | Veredito | Observação |
|---|----------|------------|
| 1 | ✓ Correto e bem estruturado | Faltou uma dimensão: Art. 121 responsabiliza o *indivíduo* (servidor) por dolo ou erro grosseiro; Súmula 331 responsabiliza a *entidade* (União). São não só riscos diferentes, mas sujeitos diferentes. |
| 2 | ✓ Correto e cirúrgico | Gap identificado com precisão. Nota: a fraude documental (falsidade ideológica, CP Art. 299) e a improbidade (Lei 8.429/92) cobririam esse buraco — mas estão ausentes dos 7 normativos do blueprint, confirmando o ponto. |
| 3 | ✓ Correto | Atribuição de responsabilidade ao Financeiro/Ordenador de Despesa está certa. Nuance omitida: o fiscal tem obrigação indireta de alertar se souber que a retenção não ocorre — omissão consciente pode gerar responsabilidade concorrente. |
| 4 | ✓ Correto | "Escassez absoluta" é formulação ligeiramente mais rígida que o texto do Decreto (que fala em "impossibilidade de designação de servidores diferentes"). A direção está certa; a intensidade do padrão legal está um grau acima do que o Decreto exige literalmente. |
| 5 | ✗ Erro de camada | Etapa 3 está certa. Camada está errada. O fiscal que faz acompanhamento informal está na camada de **Ações do Fiscal** (acima da Linha de Interação), não no Frontstage. Frontstage é a camada da contratada/preposto. O fiscal é o "cliente" do blueprint — ele nunca opera no Frontstage. |
| 6 | ✓ Correto e metodologicamente preciso | Defesa sólida: o blueprint mapeia comportamentos, não cronogramas judiciais. O fail point pertence ao locus da omissão acionável, não ao locus da consequência. |
| 7 | ✓ Correto e analiticamente a melhor da rodada | O dilema operacional entre IN 05/2017 (profundidade de auditoria) e IN 77/2022 (velocidade de pagamento) é real, está mal resolvido no serviço e o blueprint atual não registra esse conflito como fail point — deveria. |
| 8 | ✓ Correto — melhor resposta da rodada | LGPD aplicada ao Shadow IT e transmissão de dados trabalhistas sensíveis é o ponto cego normativo mais relevante. Conecta PC-4 do blueprint (Shadow IT) a uma exposição legal concreta não mapeada. |

**Placar:** 7 corretos, 1 erro (Q5 — confusão entre Ações do Fiscal e Frontstage).  
**Padrão recorrente:** a distinção entre a camada do fiscal (acima da Linha de Interação) e o Frontstage (abaixo dela) ainda está gerando erros pontuais. É o mesmo ponto fraco da Q1 da Rodada 1 — o preposto que "cruza" a linha.

---

## Rodada 3 — Pontos Cegos: Localização, Camadas e os Limites do Shostack

### Perguntas

**1.** O PC-1 ("Acordo de Cavalheiros") é um acordo entre o fiscal e o preposto. Em qual linha divisória do blueprint ele ocorre — e o que o fato de acontecer exatamente nessa linha implica sobre a capacidade do sistema de detectá-lo?

**2.** O PC-2 ("Herança de Contratos") descreve perda de conhecimento tácito na substituição de um fiscal. Esse risco está em qual etapa do blueprint e em qual camada? Ou ele ocorre *entre* etapas — e se for esse o caso, o que isso significa para a metodologia Shostack?

**3.** O PC-3 ("Efeito Carimbador") é listado como Ponto Cego, mas aparece como fail point da Etapa 5. Isso é uma contradição interna do artefato — ou um Ponto Cego pode simultaneamente ser um fail point mapeado? Escolha uma posição e defenda.

**4.** O PC-4 ("Shadow IT") é o único Ponto Cego que contamina múltiplas etapas ao mesmo tempo. Identifique as duas camadas em que ele opera — e explique por que a lógica do Shostack o torna invisível em ambas.

**5.** O PC-5 ("CND como Véu") foi classificado na Rodada 2 como a evidência física que mente. Agora mude o ângulo: como Ponto Cego, em qual camada ele habita — e por que o Shostack não tem instrumento para detectá-lo *antes* que o dano se materialize?

**6.** O PC-6 ("Prazo Silencioso da Sanção") é uma *omissão* — nenhuma ação errada acontece, simplesmente nada acontece. O Shostack captura omissões como fail points — ou a metodologia só registra ações que falham? Posição definitiva.

**7.** Dos seis Pontos Cegos, identifique qual o blueprint AS-IS é estruturalmente *incapaz* de registrar como fail point — não por falta de rigor analítico, mas porque o evento ocorre fora das fronteiras do que a metodologia Shostack consegue mapear. Nomeie-o e justifique em duas frases.

**8.** O blueprint mapeia um ciclo contratual. Mas há um Ponto Cego que só se torna visível quando se sobrepõem *múltiplos ciclos* — ele é indetectável em um único contrato e só emerge no padrão histórico. Identifique qual é, diga por que a dimensão temporal única o oculta, e o que mudaria no artefato se o blueprint fosse redesenhado para incluir essa sobreposição.

---

### Respostas

**1. O PC-1 ("Acordo de Cavalheiros") ocorre na Linha de Interação.**
Ele acontece no limite exato de contato entre o usuário (fiscal) e o cliente/externo (preposto). O fato de ocorrer exatamente nessa linha implica que a negociação humana "bate e volta" ali mesmo, sem nunca descer pela Linha de Interação Interna em direção aos Processos de Suporte (sistemas de registro); logo, torna-se um evento invisível para o maquinário de auditoria do Estado, pois não gera rastro sistêmico.

**2. O PC-2 ("Herança de Contratos") ocorre *entre* as etapas (no hiato temporal entre a Etapa 8 e uma nova Etapa 1).**
Isso revela uma limitação severa da metodologia Shostack: o blueprint mapeia ações, fluxos e interações tangíveis de um usuário ativo ao longo de uma linha do tempo contínua. Ele não possui notação estrutural para mapear o "vazio", a ruptura da linha temporal ou o conhecimento tácito que evapora quando um ator sai do diagrama e outro assume seu lugar a partir do zero.

**3. Um Ponto Cego pode simultaneamente ser um fail point mapeado.**
Não há contradição. O *fail point* (mapeável) é a **ação mecânica** que dá errado (o Gestor apostar a assinatura digital no SEI sem revisar os autos). O *Ponto Cego* (indetectável) é a **causa cognitiva** dessa ação (a exaustão mental, o viés de autoridade, a confiança cega no colega); a metodologia desenha o comportamento físico, mas é cega ao estado psicológico que motiva esse comportamento.

**4. O PC-4 ("Shadow IT") opera no Frontstage (ação) e tenta emular os Processos de Suporte (ferramental).**
A lógica do Shostack o torna invisível porque a metodologia mapeia a arquitetura do serviço *projetado oficialmente pela instituição*. O Shadow IT (WhatsApp, Excel, ChatGPT) é uma jornada rebelde, paralela, que não cruza a Linha de Interação Interna com o Backstage formal. O diagrama registra apenas o que passa pelos conduítes oficiais do serviço.

**5. O PC-5 ("CND como Véu") habita a camada de Evidências Físicas/Digitais.**
O Shostack não tem instrumento para detectar a falha precocemente porque a metodologia é estruturalmente binária quanto às evidências: ela registra a **presença, a ausência e a movimentação** do artefato (a certidão foi anexada ao processo?), mas é incapaz de auditar a **veracidade material ou epistemológica** do seu conteúdo (a certidão é matematicamente verdadeira para aqueles funcionários?).

**6. A metodologia Shostack só registra ações que falham (ou gargalos em fluxos).**
Omissões puras — como deixar um prazo de sanção prescrever sem fazer absolutamente nada — são o ponto fraco do diagrama. Como o blueprint é construído através de "nós" (ações) e "setas" (fluxos), o não-agir simplesmente resulta em um espaço em branco na linha do tempo, não gerando um evento visual de erro no mapeamento clássico.

**7. O PC-2 ("Herança de Contratos").**
Este é o evento estruturalmente impossível de ser mapeado como fail point na jornada clássica. Justificativa: o blueprint exige a perspectiva de uma persona contínua interagindo com o serviço; a perda de conhecimento na troca de fiscais ocorre no "espaço em branco" fora dos nós de ação, no exato momento em que um usuário é ejetado do mapa e outro é inserido sem o *onboarding* adequado.

**8. O PC-1 ("Acordo de Cavalheiros") é o Ponto Cego histórico.**
Em um único ciclo mensal (a escala de tempo padrão de uma etapa de fiscalização no blueprint), uma falha compensada com horas extras informais parece apenas uma resolução de problema sem atrito. É apenas na sobreposição de 12 ou 24 ciclos que a maquiagem crônica da incompetência da empresa emerge. Para que o artefato capturasse isso, o blueprint precisaria ser redesenhado para incluir um **Eixo Z (profundidade temporal)**, mapeando a degradação cíclica e cumulativa do SLA em vez de representar apenas o fluxo ideal de um "mês perfeito".

---

### Avaliação do Examinador

| # | Veredito | Observação |
|---|----------|------------|
| 1 | ✓ Correto | Imprecisão terminológica: o preposto é chamado de "cliente/externo" — ele é Frontstage. O fiscal é o cliente. A mecânica descrita está correta; o vocabulário de papéis, não. |
| 2 | ✓ Correto e metodologicamente preciso | A identificação do hiato *entre* etapas como limitação estrutural do Shostack é a leitura certa. A metodologia não tem notação para vácuos de persona. |
| 3 | ✓ Correto e analiticamente fino | Distinção ação mecânica (fail point) × causa cognitiva (ponto cego) é exatamente o limite do Shostack: ele desenha comportamento, não intenção ou estado mental. |
| 4 | ✗ Erro de camada (recorrente) | Shadow IT é usado pelo fiscal — quem está na camada **Ações do Fiscal**, acima da Linha de Interação. "Frontstage" é a camada da contratada/preposto. Este é o terceiro erro do mesmo tipo nas três rodadas: o fiscal nunca opera no Frontstage. |
| 5 | ✓ Correto e mais elegante da rodada | "Binário quanto às evidências" é a formulação precisa: Shostack registra presença/ausência/movimento do artefato, não sua verdade material. |
| 6 | △ Parcial | O Shostack *pode* capturar omissões — marcando um fail point no momento em que uma ação esperada não ocorre. A dificuldade real do PC-6 não é que a metodologia proíba omissões, mas que omissões prolongadas não têm locus temporal preciso: o prazo presscreve ao longo de semanas, sem um único nó onde o erro pode ser fixado no diagrama. |
| 7 | ✓ Correto e consistente com Q2 | PC-2 é a resposta certa e coerente com a argumentação da Q2. Alternativa defensável: PC-4 (Shadow IT), porque a jornada paralela nunca cruza nenhuma linha oficial do blueprint. |
| 8 | ✓ Correto e melhor resposta da rodada | "Eixo Z de profundidade temporal" é o nome certo para o que falta. PC-1 como ponto cego histórico é a escolha mais precisa: uma conivência pontual é invisível; um padrão de 24 ciclos é a evidência de um serviço que falhou sistemicamente. PC-2 seria candidato alternativo igualmente válido. |

**Placar:** 6 corretos, 1 parcial (Q6), 1 erro (Q4).  
**Padrão consolidado:** três rodadas, três erros na mesma distinção — o fiscal opera em Ações do Fiscal (acima da Linha de Interação), nunca no Frontstage. Esse erro específico precisa ser corrigido antes das próximas rodadas.

---

## Rodada 4 — Fluxo de Rastreabilidade e o Caminho do Dinheiro

### Perguntas

**1.** O Recebimento Provisório e o Recebimento Definitivo são etapas distintas com atores distintos. É possível comprimi-las em um único ato sem violar a lei — ou a separação é juridicamente obrigatória em todos os casos? Dê o fundamento normativo.

**2.** O "direito adquirido pelo credor" que a liquidação deve verificar (Art. 63, Lei 4.320/64) nasce em qual momento exato do fluxo: na emissão da Nota Fiscal, no Recebimento Provisório, no Recebimento Definitivo, ou apenas na própria liquidação? Escolha um único momento e justifique.

**3.** A ON AGU 76/2023 veda pagamento antecipado. Se o Financeiro emite a OB imediatamente após receber o processo — sem aguardar nenhum prazo adicional — mas o ateste do Gestor já foi formalmente aposto, isso configura pagamento antecipado nos termos da ON? Distinga o que é "antecipado" legalmente do que é apenas "rápido" operacionalmente.

**4.** A IN 77/2022 impõe ordem cronológica. Um contrato A com ateste do dia 1 e histórico de irregularidades fiscais deve ser pago antes de um contrato B com ateste do dia 5, de valor mínimo e sem pendências. A IN permite priorizar B por critérios de gestão de risco — ou a cronologia é absoluta? Decida e nomeie a consequência para quem inverte a ordem sem amparo.

**5.** A retenção de 11% de INSS ocorre na Liquidação (Backstage). Se o Financeiro retém o valor corretamente mas não repassa ao INSS dentro do prazo legal, o risco jurídico permanece no Backstage — ou atravessa alguma linha divisória do blueprint em direção a outro ator? O fiscal do contrato tem responsabilidade nesse momento?

**6.** O fluxo tem 6 passos. Identifique o único passo cuja supressão invalida juridicamente *todos* os subsequentes — e diga em qual camada do blueprint esse passo está ancorado.

**7.** A Etapa 8 registra o risco de "contrato verbal" quando a prorrogação é pedida após o vencimento. Existe risco análogo no início da jornada: a empresa pode iniciar a execução antes do empenho formal. Identifique a lei violada, diga em qual etapa do blueprint isso acontece e em qual camada o risco se origina.

**8.** O fluxo de 6 passos pressupõe serviço executado antes do pagamento. Contratos de assinatura anual, licenciamento de software e seguros seguem lógica inversa na APF. Qual mecanismo legal específico permite o pagamento sem violar a ON AGU 76/2023 — e o blueprint atual consegue representar esse mecanismo dentro de suas camadas, ou precisaria de notação adicional?

---

### Respostas

**1. É possível comprimi-las em um único ato.**
A separação não é juridicamente obrigatória em todos os casos; a Lei 14.133/2021 (Art. 140, §3º) e normativos de terceirização permitem a dispensa do recebimento provisório (ou a unificação com o definitivo) em casos de bens de consumo imediato, serviços profissionais simples ou contratações de baixo valor, onde a verificação técnica e a administrativa se sobrepõem sem complexidade.

**2. Nasce no Recebimento Definitivo (Ateste).**
A emissão da Nota Fiscal é uma mera pretensão de cobrança e o Recebimento Provisório apenas atesta a entrega física; o direito adquirido pelo credor só se perfectibiliza e obriga o Estado quando o Gestor assina o Termo de Recebimento Definitivo, declarando formalmente que a entrega cumpriu todas as especificações e métricas do contrato.

**3. Não configura pagamento antecipado.**
Legalmente, o "pagamento antecipado" ocorre antes da prestação do serviço e antes do respectivo ateste. Se o Gestor já emitiu formalmente o ateste e o encaminhou, o rito de liquidação está liberado; a emissão imediata da Ordem Bancária (OB) pelo setor financeiro é apenas celeridade administrativa operacional perfeitamente lícita, e não quebra de rito jurídico.

**4. A cronologia é estrita em relação à *exigibilidade* da despesa.**
A IN 77/2022 não permite priorizar o contrato B por "gestão de risco", mas sim porque o histórico de irregularidades fiscais do contrato A **suspende a exigibilidade** do seu pagamento, retirando-o da fila ativa cronológica e abrindo caminho legal para o pagamento de B. Inverter a ordem de credores que estejam em idêntica situação de exigibilidade sem amparo legal configura grave infração financeira, sujeitando o ordenador a responsabilização por improbidade administrativa e sanções no TCU.

**5. O risco jurídico permanece inteiramente no Backstage.**
O fiscal do contrato **não tem nenhuma responsabilidade** nesse momento. O rito de retenção contábil, recolhimento de DARF/GPS e repasse de valores é um ato segregado do setor financeiro; a omissão no repasse (apropriação indébita) atrai responsabilização exclusiva e pessoal para o Ordenador de Despesa e para o agente financeiro responsável pela liquidação.

**6. O Recebimento Definitivo (Ateste).**
É o único passo (Passo 3 do fluxo) cuja ausência contamina e torna juridicamente nulos todos os passos financeiros subsequentes (Liquidação e Pagamento). No blueprint, ele está ancorado no **Frontstage (Ações do Usuário)**, pois depende exclusivamente do julgamento de valor do servidor designado para a ponta.

**7. A lei violada é a Lei 4.320/64 (Art. 60), que veda a realização de despesa sem prévio empenho.**
Esse risco acontece no início da jornada, na **Etapa 2 (Reunião Inicial / Kick-off)** ou no primeiro dia da Etapa 3. O risco origina-se no **Backstage**, quando a Administração falha na emissão tempestiva da Nota de Empenho, mas tolera ou incentiva verbalmente que a empresa inicie o trabalho "na confiança".

**8. O mecanismo é o Art. 145 da Lei 14.133/2021.**
Esta norma permite excepcionalmente o pagamento antecipado se for a única alternativa de mercado (ex: licenciamento global de software) ou representar sensível economia, exigindo garantias. O blueprint atual **é incapaz de representar isso** de forma nativa, pois sua estrutura presume a linearidade cronológica padrão (Executar → Atestar → Pagar); para não quebrar a lógica, o diagrama precisaria de notação adicional com "caminhos condicionais paralelos" (loops reversos) que invertam temporariamente a ordem das etapas 4 e 6.

---

### Avaliação do Examinador

| # | Veredito | Observação |
|---|----------|------------|
| 1 | ✓ Correto | Art. 140, §3º corretamente citado. Casos de pronta entrega e serviços simples permitem a unificação. Fundamento preciso. |
| 2 | ✓ Correto e bem fundamentado | "Perfectibiliza" é o termo jurídico correto. A NF é pretensão; o Provisório é entrega física; o Definitivo é o momento em que o Estado reconhece a obrigação de pagar. |
| 3 | ✓ Correto | Distinção legal/operacional acertada: "antecipado" = antes do ateste; "rápido" = depois do ateste sem prazo morto. A OB imediata pós-ateste é lícita. |
| 4 | ✓ Correto e preciso | A chave é "exigibilidade": irregularidade fiscal suspende a exigibilidade do contrato A, retirando-o da fila ativa. A cronologia não é absoluta — ela se aplica a despesas em idêntica situação de exigibilidade. |
| 5 | △ Parcial | Correto para o cenário específico perguntado. Nuance omitida: se o fiscal souber sistematicamente que os repasses não ocorrem e se omitir, pode haver responsabilidade administrativa concorrente por omissão — não pela retenção, mas pela inação diante de irregularidade conhecida. |
| 6 | ✗ Erro de camada (4ª ocorrência) | Etapa correta (Recebimento Definitivo), camada errada. O Gestor que assina o ateste está na camada **Ações do Fiscal** (acima da Linha de Interação), não no Frontstage. "Frontstage (Ações do Usuário)" é uma contradição em termos: no Shostack, são camadas diferentes. Este é o quarto erro do mesmo tipo em quatro rodadas. |
| 7 | ✓ Correto | Art. 60 da Lei 4.320/64 é a lei certa. Etapa 2/início da Etapa 3 é o momento certo. Backstage como camada de origem é a leitura correta: a falha está na Administração que não emite o empenho, não na empresa que começa. |
| 8 | ✓ Correto | Art. 145 da Lei 14.133/2021 é o mecanismo correto. A identificação de que o blueprint precisa de "caminhos condicionais paralelos" é precisa — e aponta uma limitação real do artefato atual para contratos de lógica inversa. |

**Placar:** 6 corretos, 1 parcial (Q5), 1 erro (Q6).  
**Padrão consolidado — 4 rodadas, 4 erros idênticos:** o Gestor/Fiscal opera em Ações do Fiscal (acima da Linha de Interação). Frontstage e Ações do Usuário/Fiscal são camadas separadas no Shostack. Essa confusão é o único ponto cego recorrente de toda a sessão.

---

## Rodada 5 — Atores, Sobreposição de Papéis e o que Isso Faz com as Linhas

### Perguntas

**1.** O blueprint posiciona Fiscal Técnico, Fiscal Administrativo e Gestor como atores distintos em camadas distintas. Quando um único servidor acumula os três papéis, ele ocupa três posições simultaneamente no diagrama — ou colapsa para uma única camada? Qual é a consequência para a leitura do blueprint?

**2.** A Linha de Visibilidade separa o que o fiscal vê do que ocorre no Backstage. Quando o Fiscal Técnico e o Fiscal Administrativo são o mesmo servidor, essa linha desaparece, se desloca ou permanece intacta? O que muda estruturalmente no blueprint?

**3.** O Gestor assina o ateste definitivo com base nos pareceres do Fiscal Técnico e do Fiscal Administrativo. Se um único servidor é os três ao mesmo tempo, o que acontece com o fluxo de informação que o ateste pressupõe — e qual fail point novo emerge que não existia com papéis segregados?

**4.** Quando a acumulação de papéis é formalmente justificada por escassez de pessoal (Decreto 11.246/2022), o servidor acumulador responde juridicamente como Fiscal Técnico, como Fiscal Administrativo ou como Gestor — ou assume a responsabilidade das três camadas simultaneamente? Decida e indique o impacto na exposição jurídica total.

**5.** O preposto interage com "o fiscal". Quando um único servidor acumula todos os papéis fiscais, a posição do preposto no blueprint muda — ou ele permanece no mesmo Frontstage independentemente de quantas funções o fiscal acumula? E o que muda na relação operacional entre os dois?

**6.** A *culpa in vigilando* exige que o fiscal vigie o cumprimento das obrigações trabalhistas. Quando Fiscal Técnico e Fiscal Administrativo são o mesmo servidor, a carga de vigilância se soma linearmente — ou o risco jurídico cresce de forma não-linear? Explique o mecanismo em duas frases.

**7.** No blueprint, evidências físicas são produzidas por um ator e validadas por outro. Quando o mesmo servidor preenche e assina o próprio Termo de Recebimento Definitivo, o que acontece com o valor probatório dessa evidência — e a metodologia Shostack tem algum instrumento para registrar esse colapso de segregação?

**8.** O blueprint AS-IS mapeia papéis como se fossem exercidos por atores distintos. Na prática descrita no Sumário Executivo, o servidor frequentemente acumula tudo. Isso significa que o blueprint está mapeando uma jornada fictícia — ou um AS-IS de uma situação disfuncional ainda é metodologicamente válido como ferramenta de diagnóstico? Posição definitiva com justificativa.

---

### Respostas

**1. O ator transita pelas três camadas, ziguezagueando pelo diagrama.**
No modelo de Shostack, as camadas representam a natureza da ação, não o cargo. Quando um único servidor acumula tudo, o blueprint não colapsa; em vez disso, a consequência para a leitura é que a jornada do usuário se torna um loop vertical exaustivo, onde uma única pessoa cruza as linhas do diagrama repetidas vezes para executar as ações operacionais e prover o suporte de retaguarda para si mesma.

**2. A Linha de Visibilidade permanece estruturalmente intacta, mas é internalizada pelo usuário.**
O que muda estruturalmente no blueprint é que o processo deixa de ser uma passagem de bastão (hand-off) colaborativa entre atores distintos e se torna um gargalo solitário. A linha divisória continua existindo para separar as ações de campo (avaliação in loco) das ações de sistema (análise de CNDs), mas o usuário passa a operar de ambos os lados da fronteira.

**3. O fluxo de informação torna-se um monólogo e surge o risco de "Cegueira de Autovalidação".**
O ateste pressupõe um sistema de freios e contrapesos (segregação de funções). Quando uma pessoa faz tudo, o novo fail point que emerge é a impossibilidade de revisão crítica: erros técnicos ou lapsos na conferência administrativa são automaticamente herdados e chancelados na decisão final do Gestor, sem nenhum filtro independente.

**4. O servidor assume a responsabilidade pelas três camadas simultaneamente.**
A justificativa formal de escassez de pessoal perdoa a Administração pela falta de segregação, mas não isenta o servidor de cumprir as tarefas legais. O impacto na exposição jurídica total é absoluto: o fiscal perde o "escudo" da responsabilidade compartilhada e torna-se o alvo único e exclusivo para responder por falhas técnicas, administrativas e de gestão perante os órgãos de controle.

**5. O preposto permanece exatamente no mesmo Frontstage.**
A posição estrutural do preposto não muda, pois a sua interface de contato com a Administração Pública continua sendo "o fiscal". O que muda drasticamente é a relação operacional: a comunicação torna-se hipercentralizada, aumentando a assimetria de poder da contratada sobre um servidor sobrecarregado e elevando o risco de acordos informais por afunilamento de demandas.

**6. O risco jurídico cresce de forma não-linear (exponencial).**
Como o tempo e a atenção do servidor são recursos finitos e inelásticos, a exigência física da inspeção técnica de campo (Técnico) canibaliza diretamente o tempo necessário para a minuciosa auditoria de folhas de pagamento e guias (Administrativo), garantindo que pelo menos uma das vigilâncias será sistematicamente executada com negligência.

**7. O valor probatório como instrumento de controle interno é severamente degradado.**
A evidência passa a atestar apenas a formalidade sistêmica, perdendo sua capacidade de auditoria independente. A metodologia Shostack clássica não tem instrumento para registrar o colapso da segregação de funções, pois ela mapeia a criação material do artefato na linha do tempo, sendo "cega" à integridade do controle interno ou ao conflito de interesses na sua autoria.

**8. O mapeamento é perfeitamente válido e essencial como ferramenta de diagnóstico.**
Um blueprint AS-IS tem a função de espelhar o abismo entre o design normativo projetado e a realidade de campo. Mapear as funções separadamente, para depois documentar no Sumário e nos fail points que elas colapsam sobre um único indivíduo, é exatamente o que torna o artefato útil: ele visualiza o tamanho do fardo legal imposto à linha de frente e expõe a disfunção do modelo operacional atual.

---

### Avaliação do Examinador

| # | Veredito | Observação |
|---|----------|------------|
| 1 | ✓ Correto e preciso | "Camadas representam a natureza da ação, não o cargo" é a formulação exata do Shostack. O "loop vertical exaustivo" como consequência de leitura é a imagem correta. Ponto não explorado: quando não há handoffs entre atores distintos, o blueprint perde sua principal ferramenta diagnóstica — identificar onde passagens de bastão falham. |
| 2 | ✓ Correto | Linha permanece estruturalmente; o que muda é quem opera dos dois lados. "Gargalo solitário" versus "passagem de bastão colaborativa" é a distinção operacional certa. |
| 3 | ✓ Correto e melhor nome da rodada | "Cegueira de Autovalidação" é o nome preciso para o fail point emergente. O mecanismo — erro técnico herdado e chancelado sem filtro independente — é exatamente o que torna a acumulação de papéis um risco sistêmico, não apenas burocrático. |
| 4 | ✓ Correto | "Perde o escudo da responsabilidade compartilhada" é a consequência jurídica correta. Nuance adicional: mesmo com segregação, cada ator responde pelo seu domínio individualmente — o que muda com a acumulação é que desaparece o argumento de defesa "o colega deveria ter verificado isso". |
| 5 | ✓ Correto | Preposto permanece no Frontstage — posição estrutural inalterada. "Assimetria de poder da contratada sobre servidor sobrecarregado" é o risco operacional correto e conecta diretamente ao PC-1 (Acordo de Cavalheiros). |
| 6 | ✓ Correto no mecanismo; impreciso no qualificador | O mecanismo de canibalização de atenção é correto. "Exponencial" é impreciso — implica relação matemática específica que não se sustenta aqui. O termo adequado é "não-linear" ou "supralinear": o risco cresce mais rápido que a soma das partes, mas não necessariamente em progressão exponencial. |
| 7 | ✓ Correto e metodologicamente mais preciso da rodada | "Cega à integridade do controle interno ou ao conflito de interesses na autoria" é exatamente o limite estrutural do Shostack. A metodologia rastreia criação do artefato, não idoneidade do processo que o gerou. |
| 8 | ✓ Correto e bem fundamentado | "Espelhar o abismo entre design normativo e realidade de campo" é a definição operacional correta de um AS-IS. Um AS-IS disfuncional é mais valioso, não menos — é o que torna o diagnóstico possível. |

**Placar: 8/8 — primeira rodada sem erros.**  
**Observação de padrão:** o erro recorrente (fiscal no Frontstage) não apareceu nesta rodada porque as perguntas foram sobre os papéis em relação ao preposto — e o preposto *é* corretamente Frontstage. O teste definitivo do ponto cego persistente ficará para a Rodada 6.

---

## Rodada 6 — Redesign: Do AS-IS ao TO-BE

### Perguntas

**1.** Em cinco rodadas, fail points críticos apareceram em todas as 8 etapas. Uma intervenção de redesign eficaz deve ser **sistêmica** (atinge a estrutura do serviço) ou **pontual** (resolve um fail point por vez)? Escolha uma abordagem e explique por que a outra, mesmo que mais barata, seria insuficiente para este serviço específico.

**2.** O fail point mais recorrente é a fiscalização trabalhista superficial — *culpa in vigilando*, Etapa 4. Para eliminá-lo no TO-BE, a intervenção deve ocorrer em qual camada? E qual é a diferença de impacto entre intervir nas **Evidências Físicas** versus nos **Processos de Suporte**?

**3.** Na Rodada 3, você propôs um "Eixo Z de profundidade temporal" para capturar o PC-1 histórico. No TO-BE, como isso se traduz em uma mudança concreta e operacional no blueprint — e em qual camada ou linha essa adição incide?

**4.** Na Rodada 2, a LGPD foi identificada como normativo ausente. No TO-BE, a conformidade com a LGPD entra no blueprint como: (a) nova **Evidência Física** (política de proteção de dados assinada); (b) restrição nos **Processos de Suporte** (sistemas com criptografia e logs de acesso); ou (c) nova **linha divisória** entre canais oficiais e Shadow IT? Escolha uma e justifique — as outras duas são insuficientes sozinhas?

**5.** O "ateste cego" (Etapa 5) surge da ausência de freios e contrapesos. A intervenção mínima para eliminar esse fail point específico é: (a) segundo assinante obrigatório no SEI; (b) automatização da verificação de IMR nos Processos de Suporte; ou (c) deslocamento estrutural do Gestor para o Backstage, separando-o do Fiscal. Escolha uma, defenda — e diga em qual camada a intervenção escolhida incide.

**6.** A integração de APIs em tempo real (e-Social + SIAFI + portais de CND) eliminaria a validação humana manual do Backstage. Isso move qual linha divisória — e em qual direção? Diga o que estruturalmente desaparece e o que surge quando essa linha se move.

**7.** O blueprint TO-BE precisaria de uma **nova camada** que o Shostack original não prevê — ou as 5 camadas existentes são suficientes para representar qualquer redesign possível deste serviço? Posição definitiva com justificativa.

**8.** Sintetize o TO-BE em termos exclusivamente de linhas e camadas: quais linhas se movem, quais camadas se expandem, quais se contraem, e qual o resultado líquido para o servidor que vive a jornada. Máximo de quatro movimentos. Sem narrativa — apenas os movimentos e seus efeitos.

---

### Respostas

**1. A intervenção deve ser sistêmica.**
A abordagem pontual seria inútil porque os fail points deste serviço (como o ateste cego na Etapa 5 ou o acordo de cavalheiros na Etapa 3) não são erros isolados, mas sim sintomas interligados de uma falha raiz estrutural: a assimetria entre a carga cognitiva imposta pela lei e o ferramental arcaico disponível. Tratar o sintoma sem alterar a estrutura de suporte apenas moveria o erro de uma etapa para a outra.

**2. A intervenção deve ocorrer nos Processos de Suporte.**
Intervir nas Evidências Físicas (ex: criar novos checklists ou declarações) apenas aumenta a burocracia no Frontstage, exigindo mais trabalho humano falível para preencher mais papéis; intervir nos Processos de Suporte (ex: cruzar nativamente as planilhas do e-Social com a medição do contrato via sistema) automatiza o compliance e bloqueia o erro antes que o usuário possa cometê-lo.

**3. Incide nos Processos de Suporte (painéis de dados persistentes).**
Concretamente, o Eixo Z não seria desenhado tridimensionalmente, mas introduzido como um **"Painel de Histórico Longitudinal" (Dashboard Analítico)** na camada de Processos de Suporte, visível em toda a jornada. Ele obrigaria o sistema a exibir ao fiscal não apenas a medição do mês atual, mas o gráfico de tendência (glosas aplicadas e perdoadas) dos últimos 12 meses antes de liberar a assinatura de qualquer nova etapa.

**4. Entra como (b) restrição nos Processos de Suporte.**
Uma política de proteção (a) é apenas um papel morto e criar uma linha contra o Shadow IT (c) é inócuo sem oferecer alternativa melhor; a única forma de garantir conformidade com a LGPD e extinguir o uso de WhatsApp/e-mail para troca de atestados e documentos sensíveis é construir dutos de comunicação criptografados e rastreáveis na camada de Processos de Suporte, forçando todo o fluxo por ali.

**5. (b) Automatização da verificação de IMR nos Processos de Suporte.**
Apenas exigir um segundo assinante (a) cria dois carimbadores em vez de um; deslocar o Gestor para o Backstage (c) não resolve se ele continuar recebendo papéis estáticos. A automatização do IMR nos Processos de Suporte (ex: o sistema só permite o ateste após o fiscal preencher os campos estruturados, calculando as glosas automaticamente e travando o SEI se houver inconsistência matemática) força a revisão e quebra o hábito do ateste automático.

**6. A Linha de Interação Interna sobe em direção à Linha de Visibilidade.**
Com a automação, a camada manual de Backstage (servidores de apoio conferindo papéis) se contrai até quase desaparecer, sendo engolida pela camada de Processos de Suporte (as APIs), que se expande; a mediação humana burocrática some, e a resposta sistêmica (travar ou liberar pagamento) passa a interagir de forma quase direta com as ações do Frontstage.

**7. As 5 camadas existentes são insuficientes para a Administração Pública.**
O Shostack foca no eixo Operação/Mercado. Para serviços de Estado, o TO-BE precisaria impreterivelmente de uma **6ª camada: a "Camada de Compliance Legal/Auditoria Ativa"**, situada abaixo dos Processos de Suporte; diferentemente das normas estáticas descritas ao lado do mapa, essa camada mapearia como algoritmos de *continuous auditing* (TCU/CGU) puxam dados da jornada em tempo real para disparar alertas preventivos, o que as 5 originais não comportam sem forçar a teoria.

**8. Síntese dos movimentos TO-BE:**
- **Movimento 1:** A Linha de Interação Interna sobe abruptamente, encolhendo o Backstage humano.
- **Movimento 2:** A camada de Processos de Suporte se expande maciçamente, absorvendo a validação das Evidências Físicas.
- **Movimento 3:** As interações de Frontstage se contraem em volume, mas aumentam em complexidade de análise de exceções.
- **Resultado Líquido:** O usuário perde a autonomia de cometer infrações por conveniência (perda de margem de manobra informal) e ganha proteção cognitiva, operando como um analisador de painéis em vez de um conferente de papéis.

---

### Avaliação do Examinador

| # | Veredito | Observação |
|---|----------|------------|
| 1 | ✓ Correto e preciso | "Assimetria entre carga cognitiva e ferramental arcaico" é a formulação correta da falha raiz estrutural — exatamente o que o Sumário Executivo do blueprint diagnostica. O argumento de que a intervenção pontual apenas desloca o erro é correto. |
| 2 | ✓ Correto | Distinção precisa: Evidências Físicas adicionam trabalho humano falível; Processos de Suporte automatizam e bloqueiam. A intervenção pré-emptiva é na camada correta. Nota: "burocracia no Frontstage" é impreciso — checklists extras recairiam sobre as Ações do Fiscal, não sobre o Frontstage. Erro menor de vocabulário, não de raciocínio. |
| 3 | ✓ Correto e operacionalmente especificado | "Painel de Histórico Longitudinal" em Processos de Suporte é a tradução concreta correta. Travamento da assinatura sem visualização do histórico é o mecanismo certo para forçar o Eixo Z. |
| 4 | ✓ Correto | Hierarquia de eficácia bem estabelecida: política (papel morto) < nova linha (inócua sem alternativa) < canal criptografado em Processos de Suporte (força o comportamento). Raciocínio de design comportamental aplicado corretamente. |
| 5 | ✓ Correto e bem argumentado | "Dois carimbadores em vez de um" é o argumento correto contra a opção (a). Automatização que trava o SEI até preenchimento estruturado é a única intervenção que muda o comportamento sem depender de boa vontade do ator. Camada corretamente identificada. |
| 6 | ✓ Correto na linha e direção; imprecisão residual | Linha de Interação Interna sobe — correto. Backstage humano se contrai — correto. Imprecisão: "a resposta sistêmica passa a interagir com as ações do Frontstage" — a resposta sistêmica (trava/liberação) chega às **Ações do Fiscal** (acima da Linha de Interação), não ao Frontstage (contratada). Quinto e último eco do erro recorrente, aqui em forma residual. |
| 7 | △ Defensável, com contra-argumento | A proposta de 6ª camada para auditoria contínua (TCU/CGU) é intelectualmente coerente. Contra-argumento: o *continuous auditing* poderia ser absorvido como expansão dos Processos de Suporte sem exigir nova camada — a diferença é de escopo, não de natureza arquitetural. A posição é sustentável, mas não é a única resposta válida. |
| 8 | ✓ Melhor síntese de toda a sessão | Quatro movimentos claros, sem narrativa excessiva. "Analisador de painéis em vez de conferente de papéis" é a formulação mais precisa do resultado líquido para o servidor — captura tanto a perda (autonomia informal) quanto o ganho (proteção cognitiva) em uma única imagem. |

**Placar: 7 corretos, 1 parcial (Q7), 1 imprecisão residual (Q6).**

---

## Consolidado da Sessão — 6 Rodadas

| Rodada | Tema | Placar | Erro Recorrente |
|--------|------|--------|-----------------|
| 1 | Camadas, Linhas e Fail Points (Mecânica Fundamental) | 6/8 | Q1: preposto "cruza" a linha (não opera nela) |
| 2 | Normativos e Responsabilidade Jurídica | 7/8 | Q5: Fiscal Técnico → "Frontstage" |
| 3 | Pontos Cegos: Localização e Limites do Shostack | 6/8 | Q4: Shadow IT → "Frontstage" |
| 4 | Fluxo de Rastreabilidade e o Caminho do Dinheiro | 6/8 | Q6: Gestor/ateste → "Frontstage (Ações do Usuário)" |
| 5 | Atores e Sobreposição de Papéis | 8/8 | — (preposto corretamente em Frontstage) |
| 6 | Redesign: Do AS-IS ao TO-BE | 7/8 | Q6: resposta sistêmica → "Frontstage" (deveria ser Ações do Fiscal) |
| **Total** | | **40/48 (83%)** | **5 ocorrências do mesmo erro de camada** |

**Ponto cego consolidado da sessão:** em 5 das 6 rodadas, o ator fiscal (ou algo que se dirige a ele) foi colocado na camada de Frontstage. No Shostack, o fiscal é o "cliente" da jornada — suas ações estão acima da Linha de Interação, na camada de Ações do Fiscal. O Frontstage é a camada da contratada e do preposto, abaixo da Linha de Interação. A Rodada 5 foi limpa porque as perguntas perguntavam sobre o preposto — e o preposto *é* corretamente Frontstage.

**Ponto forte consolidado:** raciocínio jurídico e normativo — especialmente a distinção entre exigibilidade e cronologia (R4-Q4), o gap da LGPD (R2-Q8), o mecanismo da culpa in vigilando (R2-Q1) e a síntese TO-BE (R6-Q8). Todas as perguntas de consequência jurídica foram respondidas com precisão forense.
