---
id: index
tipo: index
produto: [NOME-DO-PRODUTO]
atualizado_em: YYYY-MM-DD
fonte: base-de-contexto-produto
confianca: alta
---

# Índice da Base de Contexto

Este é o mapa central da base de conhecimento do produto. Ele lista a finalidade, a data da última atualização e o nível de confiança de cada documento.

---

## Fontes da Verdade (Contexto)

| id | tipo | atualizado | confiança | O que responde |
|---|---|---|---|---|
| `produto-visao` | visao | YYYY-MM-DD | alta | O que o produto é, para quem serve e o que ele **NÃO** é |
| `personas` | persona | YYYY-MM-DD | alta/media | Quem usa, em que proporção e onde cada um sofre/desiste |
| `metricas` | metrica | YYYY-MM-DD | alta | North Star Metric, KRs do trimestre e metas de negócio |
| `funil` | metrica | YYYY-MM-DD | alta | Etapas da jornada, taxas de conversão e gargalos |
| `restricoes` | restricao | YYYY-MM-DD | alta | Limites de capacidade do time, contratos, segurança e LGPD |
| `stakeholders` | stakeholder | YYYY-MM-DD | media/alta | Quem decide, o que valoriza cada liderança e riscos políticos |
| `criterios-de-priorizacao` | criterio | YYYY-MM-DD | alta | Critérios formais com peso e o que **NÃO** é critério |
| `decisoes-anteriores` | decisao | YYYY-MM-DD | alta | O que já foi decidido e os resultados apurados |
| `glossario-do-time` | glossario | YYYY-MM-DD | alta | Vocabulário oficial e palavras proibidas |

---

## Avisos e Lacunas Conhecidas

- **Documentos com Confiança Média/Baixa**: `[Listar documentos que necessitam de revalidação]`
- **O que a base ainda não cobre**: `[Listar métricas ou instrumentações ausentes]`
