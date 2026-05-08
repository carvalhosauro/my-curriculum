# Relatório de aderência — Escavador IA & Backend Pleno
**Data:** 2026-05-07

---

## Match de requisitos × experiência

| Requisito (P0) | Situação | Feito / Habilidade | Aderência |
|----------------|----------|---------------------|-----------|
| Python moderno + padrões + código limpo | ❌ GAP | Não documentado (linguagem principal: PHP/Symfony) | Nenhuma |
| Programação assíncrona | 🟡 Parcial | AWS SQS em produção (mentalidade async via filas); sem asyncio formal | Média (conceitual) |
| Criação de APIs e comunicação entre sistemas | ✅ OK | APIs REST em produção (Pigz) + integrações externas | Alta |
| SQL | ✅ OK | MySQL em produção: queries, modelagem, análise | Alta |
| Bancos vetoriais (conceito) | 🟡 Parcial | Conceito aplicado via RAG no MVP WhatsApp (llphant/llphant); sem uso direto de pgvector/Qdrant | Média |
| Docker + CI/CD | 🟡 Parcial | Docker em produção (alta); CI/CD não documentado | Parcial |
| TDD + versionamento | 🟡 Parcial | Git em produção (alto); TDD não documentado | Parcial |
| Otimização de performance em produção | ✅ OK | ~50% redução de custo + melhoria de latência (Google Geolocation); observabilidade end-to-end | Alta |
| Documentação técnica complexa | ✅ OK | Inglês técnico + tradução de problemas técnicos para times não-técnicos | Alta |

| Diferencial (P1) | Situação |
|------------------|----------|
| OpenAI / LLMs | ✅ OK — arquitetura extensível por provedor (deepseek-v4-flash em uso; Gemini e OpenAI suportados) no MVP WhatsApp |
| RAG | ✅ OK — RAG em produção no MVP WhatsApp (catálogo/regras do tenant) |
| Function calling / Tools | ✅ OK — em produção (carrinho, fechar pedido, status) |
| GitLab CI/CD | ❌ GAP |
| asyncio / SQLAlchemy / FastAPI | ❌ GAP |
| Open-source | ❌ GAP |
| Mentoria | ✅ OK — onboarding de novo integrante na Pigz |

---

## Avaliação geral

**Aderência técnica estimada: ~60–65%** (atualizado após o feito do MVP de WhatsApp conversacional).

A vaga é específica: **Python + LLMs/IA + bancos vetoriais**. Stack principal de Gustavo é PHP/Symfony, mas há agora **experiência real e em produção com LLMs, RAG, function calling e integração WhatsApp** — apenas em PHP em vez de Python. Restante (APIs, SQL, Docker, async via SQS, otimização, mentoria, observabilidade) já era ponto forte.

### Pontos fortes (genuínos)
- **Otimização de produção com números** — match direto com "monitorar, diagnosticar e otimizar performance, garantindo baixa latência".
- **Observabilidade end-to-end** — vantagem competitiva real para sistemas IA em produção (latência, custo de inferência, falhas).
- **Sistemas assíncronos via fila (AWS SQS)** — mentalidade que se transfere para asyncio/pipelines.
- **Mentoria** — atende ao requisito de "mentoria técnica para juniores".
- **Tradução técnica** — atende "traduzir desafios de negócio em soluções técnicas robustas e documentadas".

### Gaps críticos
1. **Python** — linguagem principal da vaga; gap claro.
2. **LLMs / RAG / Bancos vetoriais** — todo o domínio de IA.
3. **FastAPI / SQLAlchemy / asyncio** — bibliotecas específicas.
4. **CI/CD documentado**.

---

## Top 3 impactos para destacar

1. **+10% em vendas em 2 dias** no piloto do MVP de pedidos 100% conversacionais via WhatsApp (LLM + RAG + tools, llphant/llphant, arquitetura extensível por provedor) — entregue em 2 semanas. Match direto com "sistemas baseados em IA / NLP", "buscas semânticas" e "traduzir desafios de negócio".
2. **~50% de redução de custo + melhoria de latência** em integração externa via análise, cache e refactor — match com "otimizar performance, baixa latência".
3. **Observabilidade end-to-end** (OTel + Jaeger + Loki + Prometheus + Grafana) — fundação para operar IA em produção com SLO real.

---

## Gaps e plano realista

| Gap | Plano |
|-----|-------|
| Python moderno | Estudo focado: 1–2 meses para base sólida vinda de PHP/Go |
| FastAPI + asyncio | Projeto API com FastAPI + httpx; 3–4 semanas após base de Python |
| SQLAlchemy | Naturalmente adjacente — vem com FastAPI |
| Bancos vetoriais | Tutorial prático com pgvector ou Qdrant; 1–2 semanas para conceito + uso básico |
| LLMs / RAG | Projeto prático com OpenAI API + pgvector (RAG mínimo); 3–4 semanas |
| GitLab CI/CD | 1–2 semanas |

---

## Recomendação

> **Candidatura claramente recomendada.** Com o MVP de WhatsApp conversacional (LLM + RAG + tools em produção) o perfil saiu de "backend interessado em IA" para **"engenheiro com IA aplicada em produção"** — em PHP, sim, mas com os conceitos centrais da vaga (LLMs, RAG, function calling, integração com Meta API, arquitetura extensível por provedor) já vividos e com impacto de negócio mensurável (+10% vendas). O gap real e único é a linguagem Python como ferramenta principal — sinalizar como em estudo ativo, sem inflar.

---

## Currículo gerado

Arquivo: `v1/2026-05-07-escavador-ia-backend.html`
