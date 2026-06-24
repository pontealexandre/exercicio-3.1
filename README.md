# Exercício 3.1 — Service Blueprint AS-IS de um Serviço Público

**Autor:** Alexandre F Ponte  
**Exercício:** 3.1  
**Serviço mapeado:** Gestão e Fiscalização de Contratos na Administração Pública Federal  
**Metodologia:** Service Blueprint AS-IS — Shostack (1984)

---

## Índice de Arquivos

| Arquivo | Descrição |
|:---|:---|
| `A_meta_prompt.md` | Meta-prompt de pesquisa: serviço nomeado, escopo de deep research, requisitos de operação/bastidor/fail points |
| `B_relatorio_assistente_v1.md` | Relatório de pesquisa AS-IS — versão 1 (draft inicial) |
| `B_relatorio_assistente_v2.md` | Relatório de pesquisa AS-IS — versão 2 (revisado após auditoria v1) |
| `B_relatorio_assistente_v3.md` | Relatório de pesquisa AS-IS — versão 3 final (revisado após auditoria v2) |
| `B_relatorio_auditoria_v1.md` | Auditoria independente da v1: falhas reais identificadas e gatilhos de correção |
| `B_relatorio_auditoria_v2.md` | Auditoria independente da v2: verificação das correções e novos gatilhos |
| `C_grill_transcript.md` | Transcript completo da sessão /grill-me — 6 rodadas de Q&A sobre o blueprint |
| `C_blueprint_asis.md` | Service Blueprint AS-IS em tabela Shostack: 5 camadas, 8 etapas, fail points marcados |
| `D_diagrama_asis.md` | Diagrama Mermaid da jornada: relações explícitas entre etapas, atores, sistemas e fail points |

---

## Estrutura do Serviço Mapeado

A jornada cobre o ciclo completo de fiscalização contratual na APF, da designação do fiscal até o encerramento ou aditamento do contrato:

1. Designação e Assunção
2. Reunião Inicial (Kick-off)
3. Acompanhamento e Rotina
4. Recebimento Provisório
5. Recebimento Definitivo e Ateste
6. Encaminhamento e Pagamento
7. Ocorrências e Sanções
8. Aditivos ou Encerramento

**Ator central:** Fiscal / Gestor de Contrato (perspectiva do "cliente" no modelo Shostack)  
**Fail points críticos identificados:** 8 (culpa in vigilando, ateste cego, Shadow IT, CND como véu, quebra de ordem cronológica, prescrição por omissão, contrato verbal)
