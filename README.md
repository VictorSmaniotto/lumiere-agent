# Copiloto de Produto: Sistema de Contexto, Decisão e Operação Contínua

Este workspace implementa um **Agente de Gestão Contínua de Produto (PM Thinking Partner)**, parametrizável para **qualquer produto digital**, inspirado nos melhores padrões de bases de contexto em Markdown, frontmatter com metadados de confiança, separação estrita entre Contexto e Dados Brutos, e registro auditável de decisões.

---

## 🎯 Objetivo do Agente

Atuar como o parceiro de raciocínio analítico do Product Manager para:
1. **Cruzar dados de campo (entrevistas, chamados, funis) com a fonte da verdade do produto**;
2. **Apontar contradições e lacunas** sem suavizar dados desfavoráveis;
3. **Avaliar e priorizar iniciativas de backlog** com base em critérios objetivos e pesos declarados;
4. **Gerar PRDs no padrão de ouro** (claros, sem palavras vazias, com restrições e critérios de aceite testáveis);
5. **Registrar Decisões (Decision Records)** com gatilhos explícitos de revisão.

---

## 📂 Estrutura do Workspace

```
lumiere-agent/
├── README.md                           # Guia do sistema de contexto e operação
├── SYSTEM_PROMPT.md                    # Prompt mestre do copiloto de produto
├── contexto/                           # FONTE DA VERDADE (Persistente, muda pouco)
│   ├── INDEX.md                        # O mapa central da base com metadados e confiança
│   ├── produto-visao.md                # Visão, proposta de valor e o que o produto NÃO é
│   ├── personas.md                     # Segmentação, proporções e pontos de abandono
│   ├── metricas.md                     # North Star, KRs do trimestre e séries históricas
│   ├── funil.md                        # Etapas do funil, taxas de conversão e gargalos
│   ├── restricoes.md                   # Capacidade do time, restrições técnicas, legais e contratuais
│   ├── stakeholders.md                 # Quem decide, incentivos e critérios de convicção
│   ├── criterios-de-priorizacao.md     # Critérios formais com peso e o que NÃO é critério
│   ├── decisoes-anteriores.md          # Histórico de decisões passadas e resultados
│   └── glossario-do-time.md            # Vocabulário padrão e palavras proibidas
├── dados/                              # INSUMOS BRUTOS DE ANÁLISE (Entrevistas, chamados, métricas)
│   ├── README.md                       # Como alimentar a pasta de dados
│   ├── entrevistas.md                  # Notas de entrevistas não editadas
│   ├── chamados-suporte.csv            # Amostra de chamados categorizados
│   └── notas-reuniao.md                # Transcrições ou notas de reuniões de alinhamento
├── skills/                             # PLAYBOOKS DE RACIOCÍNIO DO COPILOTO
│   ├── 01_diagnostico_e_contraditorio.md  # Cruzamento de dados e identificação de causas-raiz
│   ├── 02_priorizacao_de_iniciativas.md   # Avaliação de backlog contra critérios formais
│   ├── 03_prd_padrao_ouro.md             # Redação de PRDs aprováveis sem retrabalho
│   ├── 04_decision_record.md             # Registro estruturado de decisões de produto
│   └── 05_alinhamento_estrategico.md     # Preparação de apresentações e defesas para comitê
├── decisoes/                           # HISTÓRICO DE DECISÕES ATIVAS
│   └── README.md                       # Diretório onde as decisões geradas são arquivadas
└── referencias/                        # PADRÕES DE QUALIDADE DO TIME
    ├── prd-modelo-aprovado.md          # Exemplo de PRD de referência
    └── prd-anti-exemplo.md             # O que NÃO fazer em um PRD
```

---

## ⚙️ Regras Fundamentais de Operação

1. **`contexto/` é Fonte da Verdade. `dados/` é Insumo Bruto.**
   - Um número em `dados/` que contraria `contexto/` não é erro: é um achado ou anomalia a ser investigada.
2. **Respeito aos Metadados de Confiança e Data**:
   - Todo arquivo em `contexto/` possui frontmatter com `atualizado_em` e `confianca: alta | media | baixa`.
   - Se o agente usar uma fonte desatualizada ou de confiança média/baixa, ele deve **sinalizar explicitamente na resposta**.
3. **Proibição de Inventar Números ou Fatos**:
   - Se o dado não existir, o agente responde `SEM EVIDÊNCIA` ou `MÉTRICA A DEFINIR` e lista o que precisa ser medido.
4. **Respeito às Restrições**:
   - Nenhuma recomendação pode violar restrições conhecidas (capacidade do time, contratos, limitações técnicas ou regulatórias).
