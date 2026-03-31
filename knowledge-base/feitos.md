# Feitos (base principal)

Use este arquivo para alimentar o "motor" de adaptacao de curriculos.

## Modelo de registro

```md
## YYYY-MM-DD - Titulo curto do feito
- Contexto: (sistema, time, problema)
- Atribuicao: (backend | sre | observability | dados | etc.)
- Acoes:
  - ...
  - ...
- Tecnologias: PHP, Symfony, MySQL, OpenTelemetry, etc.
- Impacto:
  - metrica 1
  - metrica 2
- Evidencias:
  - link interno/doc
  - dashboard/query/pr
- Tags: [performance], [confiabilidade], [custo], [api], [incidente]
```

---

## 2026-03-31 - Elo técnico entre produto e cliente na Pigz
- Contexto: Startup enxuta onde dúvidas técnicas de clientes chegam via time de suporte e comercial; ocasionalmente direto ao dev.
- Atribuicao: produto, comunicação, suporte técnico
- Acoes:
  - resolvo diariamente dúvidas técnicas de produto (especialmente módulo fiscal) repassadas pelo suporte/comercial;
  - traduzo linguagem técnica em explicações claras para times não-técnicos repassarem ao cliente;
  - conduzi diretamente a explicação de uma funcionalidade (que desenvolvi) para um cliente em call;
  - participo de reuniões e calls com clientes em situações específicas.
- Tecnologias: PHP, Symfony, MySQL (contexto do produto).
- Impacto:
  - redução do tempo de resposta a dúvidas técnicas dos clientes;
  - clareza e adoção da funcionalidade pelo cliente atendido diretamente.
- Evidencias:
  - histórico de chamados/tickets resolvidos;
  - call com cliente sobre funcionalidade fiscal.
- Tags: [produto], [comunicação], [cliente], [suporte-tecnico]

## 2026-03-31 - Mentoria e onboarding de novo integrante do time
- Contexto: Entrada de novo desenvolvedor no time da Pigz.
- Atribuicao: comunicação, liderança técnica
- Acoes:
  - acompanho o novato no dia a dia;
  - explico codebase, fluxos e decisões técnicas;
  - tiro dúvidas e oriento nas primeiras entregas.
- Tecnologias: PHP, Symfony, Docker, Git.
- Impacto:
  - onboarding técnico estruturado;
  - redução do tempo para o novato se tornar produtivo.
- Evidencias:
  - acompanhamento ativo em andamento.
- Tags: [comunicação], [mentoria], [onboarding], [liderança]

## 2026-03-31 - Exemplo inicial
- Contexto: Integracao de geolocalizacao com custo alto e latencia variavel.
- Atribuicao: backend
- Acoes:
  - investiguei consumo por endpoint e padrao de chamadas;
  - implementei cache e refatorei modulo de integracao.
- Tecnologias: PHP, Symfony, MySQL.
- Impacto:
  - ~50% de reducao de custo na integracao;
  - melhoria de latencia em horarios de pico.
- Evidencias:
  - dashboard de consumo por dia;
  - consultas SQL de comparativo antes/depois.
- Tags: [performance], [custo], [api], [backend]
