---
id: prd-anti-exemplo
tipo: referencia
produto: [TEMPLATE]
atualizado_em: YYYY-MM-DD
fonte: exemplos-rejeitados
confianca: alta
---

# Anti-Exemplo de PRD (Por que foi REJEITADO)

> ⚠️ **Este documento exemplifica os 4 erros mais comuns que causam a rejeição de um PRD pelo comitê de engenharia e produto.**

---

## 1. O Problema não é um Problema (É uma Solução Disfarçada)
- ❌ *"Problema: O produto não tem uma tela de inteligência artificial generativa moderna."*
- ✅ **Correção**: A ausência de uma tecnologia não é problema do cliente. O problema é a dor de negócio (ex: *"O usuário gasta 4 horas por semana digitando dados manualmente"*).

---

## 2. Uso de Palavras Vazias e Não Testáveis (*Fluff*)
- ❌ *"A nova tela deve ser intuitiva, fluida, robusta e muito amigável."*
- ✅ **Correção**: *"O usuário deve ser capaz de concluir o cadastro em até 3 cliques, com tempo de carregamento inferior a 800ms."*

---

## 3. Ausência de Métricas de Sucesso Falseáveis
- ❌ *"Meta: Melhorar a experiência do usuário e deixar os clientes satisfeitos."*
- ✅ **Correção**: *"Meta: Reduzir a taxa de abertura de chamados na categoria 'Dúvida no Onboarding' de 32% para menos de 10% em 60 dias."*

---

## 4. Violação de Restrições Conhecidas
- ❌ *"Requisito: Fazer deploy com teste A/B para 10% da base."* (Quando a infraestrutura da empresa não possui feature flags).
