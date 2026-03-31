# Relatório de aderência — MK Solutions Fullstack (Jr → Pl)
**Data:** 2026-03-31

---

## Match de requisitos x experiência

| Requisito (P0) | Situação | Feito / Habilidade relacionada | Aderência |
|----------------|----------|-------------------------------|-----------|
| React.js | ❌ GAP | Não documentado na base | Nenhuma |
| Node.js | ❌ GAP | Não documentado na base | Nenhuma |
| TypeScript | ❌ GAP | Não documentado na base | Nenhuma |
| AWS | 🟡 Parcial | AWS SQS em produção (Pigz) | Baixa — só SQS |
| Docker | ✅ OK | Docker em produção (Pigz) | Alta |
| CI/CD GitHub Actions | ❌ GAP | Não documentado na base | Nenhuma |
| Microsserviços | 🟡 Parcial | AWS SQS, sistemas distribuídos, APIs REST | Parcial — sem arquitetura formal de microsserviços |
| Jest (testes unitários) | ❌ GAP | Não documentado na base | Nenhuma |
| MongoDB | ❌ GAP | Usa MySQL; MongoDB não documentado | Nenhuma |
| PostgreSQL | ❌ GAP | Usa MySQL; PostgreSQL não documentado | Nenhuma |
| API Gateway | ❌ GAP | Não documentado na base | Nenhuma |
| Kafka | ❌ GAP | Usa AWS SQS (conceito similar de filas) | Muito baixa |
| Kubernetes | 🟡 Estudo | Em estudo ativo | Muito baixa |
| Graduação TI | ✅ OK | IFRR - TADS (em andamento, conclusão Dez/2026) | Alta |

| Requisito (P1) | Situação |
|----------------|----------|
| TypeORM | ❌ GAP |
| Mongoose | ❌ GAP |

---

## Avaliação geral

**Aderência técnica estimada: ~20%**

Esta vaga exige um perfil **Fullstack com foco real em frontend (React) e backend Node.js/TypeScript**. O perfil atual de Gustavo é backend PHP/Go com forte foco em observabilidade e confiabilidade — stacks distintas.

### O que há de compatível
- **Docker em produção** — ponto sólido
- **AWS SQS** — experiência real com AWS, ainda que limitada a filas
- **APIs REST** — backend de APIs em produção
- **Mentalidade de sistemas distribuídos** — SQS, Circuit Breaker, resiliência
- **Kubernetes em estudo** — alinhado com o ambiente da empresa
- **Formação em TI em andamento** — requisito cumprido

### Gaps críticos (bloqueariam aprovação)
1. **React.js / frontend** — ausente na base; vaga exige desenvolvimento de interfaces
2. **Node.js + TypeScript** — stack principal do backend da empresa; Gustavo usa PHP e Go
3. **MongoDB / PostgreSQL** — usa MySQL; NoSQL não documentado
4. **Testes com Jest** — não documentado; é requisito explícito
5. **CI/CD** — não documentado na base

---

## Top 3 pontos para destacar no currículo (o que temos)

1. **Docker e AWS em produção** — uso real em ambiente crítico de delivery/logística
2. **APIs REST e integrações externas** — com foco em resiliência (Circuit Breaker) e performance (~50% redução de custo)
3. **Visão de sistemas distribuídos** — filas assíncronas (SQS), observabilidade e estabilidade em produção

---

## Gaps e plano realista

| Gap | Ação realista |
|-----|--------------|
| React.js | Iniciar projeto prático (dashboard, CRUD); 2–3 meses para nível básico funcional |
| Node.js + TypeScript | Mais próximo do Go atual; 1–2 meses para base sólida |
| MongoDB | Documentar se já usou pontualmente; senão, projeto rápido com Mongoose |
| Jest | Adicionar testes em projeto pessoal; relativamente rápido dado que já testa PHP |
| CI/CD GitHub Actions | Configurar pipeline em repositório próprio; 1–2 semanas para básico |

---

## Recomendação

> **Candidatura arriscada no momento atual.** A vaga exige stack específica (React + Node + TypeScript + MongoDB) que não está documentada na base. Candidatar agora teria baixa chance de passar para etapas técnicas.
>
> **Cenário mais favorável:** completar 2–3 meses de estudo focado em Node.js/TypeScript e React com projetos práticos, depois recandidatar ou buscar vagas similares. A base de Docker, AWS, APIs e sistemas distribuídos é uma fundação real para crescer nessa direção.

---

## Currículo gerado

Arquivo: `v0/2026-03-31-mk-solutions-fullstack.html`

**Estratégia adotada:** destacar o que é genuinamente compatível (Docker, AWS, APIs, sistemas distribuídos, formação), sem adicionar tecnologias ausentes da base. Currículo posicionado como "backend sólido migrando para fullstack".
