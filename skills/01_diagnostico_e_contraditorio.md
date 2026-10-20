# Skill 01: Diagnóstico de Causa Raiz e Contraditório

## Objetivo
Analisar um problema de negócio ou de métrica cruzando múltiplos dados de campo (`dados/`) contra o contexto oficial (`contexto/`), isolando a causa raiz real de falsos sintomas e apontando contradições.

---

## Passo a Passo Operacional do Agente

1. **Leitura do Sinal / Sintoma**:
   - Identificar a métrica que caiu ou o problema reportado (ex: queda na retenção D30, aumento de churn, queda na conversão de uma etapa do funil).
2. **Triangulação de Dados**:
   - **Quantitativo**: Onde exatamente a métrica desaba no funil? A partir de qual data/coorte?
   - **Qualitativo (Entrevistas)**: O que os usuários que desistiram declaram no momento do abandono?
   - **Operacional (Chamados)**: Quais são os termos mais frequentes nos chamados de suporte dos clientes daquela coorte?
3. **Mapeamento de Contradições**:
   - O que o time acreditava que era o problema vs o que os dados mostram?
   - Ex: O time achava que os usuários queriam uma funcionalidade nova, mas os dados mostram que 70% deles desistem por erro de validação em um formulário básico.
4. **Formulação do Diagnóstico Final**:
   - **Sintoma Aparente**: O que é visível na superfície.
   - **Causa Raiz Comprovada**: O gargalo estrutural evidenciado pelos dados.
   - **Custo de Inação**: O impacto financeiro e operacional se nada for feito.
   - **Lacunas de Evidência**: O que ainda não pode ser afirmado com 100% de certeza por falta de instrumentação.
