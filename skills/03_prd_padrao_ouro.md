# Skill 03: Redação de PRDs Padrão Ouro

## Objetivo
Gerar um Documento de Requisitos de Produto (PRD) de alta qualidade técnica e de negócio, focado no problema real, sem palavras vagas, com escopo estrito e critérios de aceite testáveis.

---

## Estrutura Obrigatória do PRD

1. **Cabeçalho & Metadados**:
   - `id`, `iniciativa`, `autor`, `data`, `status: rascunho | em_revisao | aprovado`.
2. **Contexto & Enquadramento do Problema**:
   - Qual é a dor real e quem sofre com ela.
   - Citação de evidências (entrevistas, chamados, métricas do funil).
   - O que acontece se nada for feito (*Custo da Inação*).
3. **Hipótese de Valor & Métricas de Sucesso**:
   - Acreditamos que ao entregar `[Solução]`, atingiremos `[Métrica / KR]` em `[Prazo]`.
   - Métricas primárias e métricas de guarda-corpo (*guardrail metrics*).
4. **Escopo Estrito (In / Out)**:
   - **O que ESTÁ no escopo**: Lista numerada e precisa.
   - **O que NÃO ESTÁ no escopo**: Limites deliberados para evitar inchaço (*scope creep*).
5. **Requisitos Funcionais e Critérios de Aceite (Gherkin)**:
   - Formato *Dado que / Quando / Então* para cada caso de uso principal e cenários de erro.
6. **Requisitos Não-Funcionais & Restrições Técnicas**:
   - Performance, segurança, privacidade (LGPD), compatibilidade.
7. **Riscos e Dependências**:
   - Riscos mapeados e plano de mitigação.
