# Relatório de aderência — Escavador Fullstack Pleno
**Data:** 2026-05-07

---

## Match de requisitos × experiência

| Requisito (P0) | Situação | Feito / Habilidade | Aderência |
|----------------|----------|---------------------|-----------|
| JavaScript / TypeScript | ❌ GAP | Não documentado | Nenhuma |
| React (preferencialmente Next.js) | ❌ GAP | Não documentado | Nenhuma |
| APIs Node.js **ou** PHP/Laravel | ✅ OK (PHP) | PHP/Symfony em produção (Pigz) — Symfony é primo direto de Laravel; Laravel listado como familiaridade | Alta no PHP / Nenhuma no Node |
| Banco relacional (PostgreSQL/MySQL) | ✅ OK | MySQL em produção: queries, modelagem, análise | Alta |
| Consumo e integração REST | ✅ OK | APIs REST + integrações externas em produção | Alta |
| Git e versionamento | ✅ OK | Uso diário | Alta |
| Investigação estruturada de problemas | ✅ OK | Diagnóstico de incidentes em produção, observabilidade | Alta |
| Autonomia frontend↔backend | 🟡 Parcial | Backend forte; frontend não documentado | Baixa |
| Inglês técnico de leitura | ✅ OK | Leitura de documentação | Alta |

| Diferencial (P1) | Situação | Evidência |
|------------------|----------|-----------|
| Sistemas em produção com alto volume | ✅ OK | Backend crítico de delivery/logística (Pigz) |
| Performance backend | ✅ OK | ~50% redução de custo em integração Google Geolocation via cache + refactor |
| Observabilidade (logs/métricas/tracing) | ✅ OK | OpenTelemetry + Jaeger + Loki + Prometheus + Grafana em produção |
| Docker + ambientes isolados | ✅ OK | Docker em produção |
| Testes automatizados | ❌ GAP | Não documentado na base |
| CI/CD | ❌ GAP | Não documentado na base |
| Open-source | ❌ GAP | Não documentado |
| SaaS | ✅ OK | Pigz é SaaS de delivery |

---

## Avaliação geral

**Aderência técnica estimada: ~55–60%** — apoiada na cláusula "Node.js **ou** PHP/Laravel".

### Pontos fortes
- **Backend PHP de produção (Symfony)** — atende a alternativa "PHP/Laravel" da vaga; transição Symfony→Laravel é trivial (mesma família, mesmos conceitos).
- **MySQL em produção** — atende o requisito de banco relacional.
- **APIs REST + integrações externas com falhas reais** — a vaga pede explicitamente isso ("cenários reais de inconsistência e falhas").
- **Investigação de causa raiz** — vaga é categórica ("não apenas sintomas") e Gustavo tem feito direto: ~50% de redução de custo via análise + cache.
- **Docker, observabilidade, alto volume, SaaS** — quatro diferenciais simultâneos.

### Gaps reais
1. **Frontend (React/Next.js)** — gap claro; não documentado.
2. **JavaScript/TypeScript** — não documentado.
3. **Testes automatizados** e **CI/CD** — não documentados.

---

## Top 3 impactos para destacar

1. **+10% em vendas em 2 dias** no piloto do MVP de pedidos 100% conversacionais via WhatsApp (LLM + RAG + tools, llphant/llphant) — entregue em 2 semanas; integração ponta-a-ponta com Meta WhatsApp Cloud API. Demonstra entrega de produto SaaS em alto ritmo, com IA + integração externa real.
2. **~50% de redução de custo** em integração Google Geolocation via análise, cache e refatoração.
3. **Observabilidade end-to-end** (OTel + Jaeger + Loki + Prometheus + Grafana) reduzindo MTTR em incidentes de produção.

---

## Gaps e plano realista

| Gap | Plano |
|-----|-------|
| React/Next.js | Projeto prático em 4–8 semanas; mencionar como "em estudo" sem inflar |
| TypeScript | Adjacente a Go que já estuda; 2–3 semanas |
| CI/CD | Configurar pipeline pessoal; 1–2 semanas |
| Testes automatizados | Adicionar PHPUnit em projeto pessoal |

---

## Recomendação

> **Candidatura viável** com posicionamento honesto: backend Pleno em PHP com forte cultura de produção (observabilidade, resiliência, performance), em transição para fullstack. A cláusula "Node.js **ou** PHP/Laravel" é o que abre a porta — Symfony é praticamente Laravel. Sinalizar abertura para crescer no frontend sem prometer o que não há.

---

## Currículo gerado

Arquivo: `v1/2026-05-07-escavador-fullstack.html`
