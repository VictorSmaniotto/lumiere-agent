---
id: prd-modelo-aprovado
tipo: referencia
produto: [TEMPLATE]
atualizado_em: YYYY-MM-DD
fonte: engenharia-produto
confianca: alta
---

# PRD de Referência (Padrão Ouro)

## 1. Problema & Evidências
- **Problema**: 44% das novas contas abandonam o produto na etapa de importação de dados cadastrais porque o sistema rejeita arquivos sem explicar o erro na linha.
- **Evidências**: 
  - `[FATO]` Funil analytics dos últimos 30 dias (queda de 94% para 56% na etapa 3);
  - `[FATO]` 120 chamados de suporte categorizados como "erro genérico de importação";
  - `[FATO]` Entrevistas qualitativas E1 e E3 com clientes cancelados.
- **Custo da Inação**: Perda de R$ 180.000/ano em receita recorrente desperdiçada no onboarding.

---

## 2. Hipótese de Valor & Métricas
- **Hipótese**: Se indicarmos a linha exata do erro e oferecermos download do arquivo corrigido, a taxa de conclusão da importação aumentará em pelo menos 15 pontos percentuais.
- **Métrica Primária**: Conclusão da importação $\ge 70\%$.
- **Métrica de Guarda-Corpo**: Tempo de resposta do processamento $< 5$ segundos para arquivos até 5.000 linhas.

---

## 3. Escopo Estrito
### No Escopo:
1. Validação prévia de colunas obrigatórias no momento do upload.
2. Relatório de erro com número da linha e motivo em linguagem simples.
3. Botão "Baixar linhas com erro".

### Fora do Escopo:
- ❌ Criação de assistente por IA generativa para preencher campos vazios.
- ❌ Suporte a formatos legados de banco de dados (apenas CSV e XLSX).

---

## 4. Critérios de Aceite (Gherkin)

### Cenário 1: Arquivo com formato inválido em uma coluna
- **Dado que** o cliente envia um arquivo CSV com texto na coluna "Preço";
- **Quando** o sistema processar a linha 42;
- **Então** o sistema deve exibir: *"Linha 42: O campo Preço deve conter apenas números (ex: 19.90)"* e permitir o reenvio apenas dessa linha corrigida.
