# Skill 02: Avaliação e Priorização de Iniciativas de Backlog

## Objetivo
Avaliar uma lista de iniciativas candidatas para o roadmap e ranqueá-las com rigor matemático e metodológico contra os critérios formais definidos em `contexto/criterios-de-priorizacao.md`, respeitando a capacidade máxima do time declarada em `contexto/restricoes.md`.

---

## Passo a Passo Operacional do Agente

1. **Intake da Lista de Iniciativas**:
   - Listar todas as iniciativas candidatas com descrição e escopo resumido.
2. **Avaliação Individual por Critério**:
   - Para cada iniciativa, atribuir nota de 1 a 5 em cada critério formal:
     - **Impacto no KR**: 1 (Nulo) a 5 (Alavanca direta comprovada).
     - **Confiança na Evidência**: 1 (Achismo) a 5 (Fatos e dados comprovados).
     - **Facilidade / Baixo Esforço**: 1 (Altíssimo esforço) a 5 (Rápido e simples).
     - **Redução de Fricção Operacional**: 1 (Sem alívio) a 5 (Elimina sobrecarga).
3. **Cálculo da Pontuação Ponderada**:
   $$\text{Score} = \sum (\text{Nota}_i \times \text{Peso}_i)$$
4. **Filtro de Restrições e Linha de Corte (*Capacity Cut*)**:
   - Classificar as iniciativas por pontuação decrescente.
   - Aplicar o limite de capacidade do time (ex: selecionar apenas as Top 3 ou Top 4 para o trimestre).
   - Justificar por que as iniciativas rejeitadas ficaram abaixo da linha de corte.
