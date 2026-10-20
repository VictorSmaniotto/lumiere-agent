# Skill 04: Registro Estruturado de Decisão (Decision Record)

## Objetivo
Documentar escolhas arquiteturais, de produto ou de roadmap de forma auditável e transparente, garantindo que o time lembre no futuro **por que** a decisão foi tomada, quais alternativas foram rejeitadas e sob qual condição a decisão deve ser revista.

---

## Estrutura do Decision Record

```markdown
---
id: DR-[ANO]-[NUMERO]
titulo: [Título curto da decisão]
data: YYYY-MM-DD
decisores: [PM, Tech Lead, etc.]
status: [proposta | aprovada | em_revisao | revogada]
---

# Registro de Decisão: [Título]

## 1. Contexto e Problema
- Qual situação ou problema motivou a tomada de decisão neste momento.
- Quais dados e evidências foram considerados.

## 2. A Decisão Tomada
- Descrição clara da escolha final.

## 3. Alternativas Avaliadas e Rejeitadas
| Alternativa | Por que foi considerada | Por que foi rejeitada |
|---|---|---|
| Alternativa A | ... | ... |
| Alternativa B | ... | ... |

## 4. Consequências e Trade-offs Aceitos
- **Impactos Positivos Esperados**: ...
- **Impactos Negativos / Débitos Assumidos**: ...

## 5. Gatilhos de Revisão da Decisão (Review Triggers)
*Esta decisão DEVERÁ ser reaberta e revista caso:*
- [ ] A métrica X não atinja o valor Y até a data Z;
- [ ] O custo de infraestrutura ultrapasse R$ W;
- [ ] O fornecedor/contrato X seja alterado.
```
