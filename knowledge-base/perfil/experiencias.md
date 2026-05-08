---
tipo: perfil
secao: experiencias
---

# Histórico de Experiências

## Modelo de registro

```md
## Empresa — Cargo
- Período: Mês/AAAA – Mês/AAAA (ou Presente)
- Setor: (delivery, fintech, saúde, etc.)
- Stack principal: (linguagens, frameworks, infra)
- Responsabilidades:
  - ...
- Destaques:
  - ...
```

---

## Pigz — Desenvolvedor Backend

- **Período:** Jan/2025 – Presente
- **Setor:** Delivery / Logística
- **Stack principal:** PHP (Symfony), MySQL, Docker, Linux, Git, AWS SQS, OpenTelemetry, Prometheus, Grafana, Jaeger, Loki, Metabase, Go, llphant/llphant (LLM em PHP), Meta WhatsApp Cloud API, RAG, function calling/tools (LLM)
- **Responsabilidades:**
  - Desenvolvimento e manutenção de APIs e módulos backend críticos em produção
  - Integrações com serviços externos (Google APIs, etc.)
  - Diagnóstico e resolução de incidentes em produção
  - Observabilidade: instrumentação com logs, métricas e tracing distribuído
  - Refatoração de legado com foco em previsibilidade e clareza
  - Elo técnico entre produto, suporte e comercial: resolve dúvidas técnicas de produto diariamente (especialmente fiscal) e traduz para os times repassarem ao cliente
  - Participação em reuniões e calls com clientes (poucas ocasiões diretas; frequente via suporte/comercial)
  - Explicou diretamente a um cliente uma funcionalidade que desenvolveu — conduzindo o entendimento da feature em uso real
  - Acompanhamento e mentoria de novo integrante do time (onboarding técnico)
  - Dashboards no Metabase para acompanhamento de métricas de negócio (base ativa e receita)
- **Destaques:**
  - **MVP de pedidos 100% conversacionais via WhatsApp** com LLM + RAG + tools (llphant/llphant) — entregue em 2 semanas, em piloto com cliente real e **+10% em vendas em 2 dias**
  - Arquitetura extensível por provedor de LLM (deepseek-v4-flash em uso; Gemini e OpenAI suportados) com function calling para ações reais (carrinho, fechamento de pedido, status)
  - ~50% de redução de custo em integração com Google Geolocation API via análise, cache e refatoração
  - Implementação de estratégia de observabilidade (OpenTelemetry + Jaeger + Loki) melhorando diagnóstico (MTTR)
  - Resiliência em integrações externas com padrões como Circuit Breaker
  - Dashboards no Metabase a partir do banco de produção para suporte a decisões técnicas e de negócio
  - Uso intenso de IA no fluxo de desenvolvimento (Claude Code, Cursor/Antigravity) — aumento de cobertura de testes e velocidade de entrega
  - Automações com Bash e agendamento de tarefas (Crontab)
  - Scripting em Go para integrações pontuais
