---
id: restricoes
tipo: restricao
produto: [NOME-DO-PRODUTO]
atualizado_em: YYYY-MM-DD
fonte: engenharia-juridico-operacoes
confianca: alta
relacionado: [criterios-de-priorizacao]
---

# Restrições Inegociáveis do Produto

*Toda recomendação de produto, PRD ou priorização de backlog DEVE respeitar estas restrições. Recomendações que ignoram restrições são descartadas.*

---

## 1. Capacidade do Time de Engenharia
- **Capacidade Máxima**: `[Ex: 3 a 4 iniciativas de médio porte por trimestre / Squad de 4 devs + 1 designer]`
- **Débito Técnico / Manutenção Obrigatória**: `[Ex: 20% do sprint alocado para infraestrutura e sustentação]`

---

## 2. Restrições Técnicas e Arquitetura
- **Infraestrutura**: `[Ex: Ausência de feature flags / Monolito legado / Limite de concorrência em jobs]`
- **Integrações de Terceiros**: `[Ex: Contrato de fornecedor de API vigente até dezembro / Custo por requisição]`

---

## 3. Restrições Legais, Regulatórias e de Segurança
- **LGPD / Privacidade**: `[Ex: Proibição de envio de dados sensíveis para APIs públicas não homologadas]`
- **Conformidade / Auditoria**: `[Ex: Logs de auditoria obrigatórios para qualquer alteração financeira]`
