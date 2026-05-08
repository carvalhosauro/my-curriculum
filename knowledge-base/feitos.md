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

## 2026-05-07 - Pedidos 100% conversacionais via WhatsApp com LLM + RAG + tools (Pigz)
- Contexto: MVP construído em 2 semanas para permitir que clientes finais façam pedidos completos via WhatsApp, em conversa natural, sem precisar abrir app/site. Em piloto com cliente real.
- Atribuicao: backend, IA, integrações
- Acoes:
  - projetei e implementei a integração com a Meta WhatsApp Cloud API (envio/recebimento, mídia, sessão de conversa);
  - estruturei o motor conversacional sobre `llphant/llphant` (PHP) com arquitetura **extensível por provedor de LLM** (atualmente em uso: deepseek-v4-flash; suporte preparado para Gemini e OpenAI);
  - implementei **function calling / tools** para que o LLM execute ações reais (buscar produto, montar carrinho, calcular taxa, fechar pedido, consultar status);
  - implementei **RAG** sobre catálogo/regras do estabelecimento para respostas ancoradas em dados reais do tenant;
  - cuidei de orquestração de turnos, controle de contexto e fallback determinístico para fluxos críticos (pagamento, fechamento de pedido).
- Tecnologias: PHP, Symfony, llphant/llphant, Meta WhatsApp Cloud API, RAG, function calling/tools, deepseek-v4-flash, MySQL, Docker.
- Impacto:
  - **+10% em vendas em 2 dias** no piloto com primeiro cliente;
  - canal de vendas conversacional novo, com baixa fricção para o cliente final;
  - MVP entregue em 2 semanas (velocidade alavancada por uso intenso de IA no desenvolvimento — ver feito abaixo).
- Evidencias:
  - piloto em produção com cliente;
  - métrica de vendas no Metabase (antes/depois).
- Tags: [ia], [llm], [rag], [tools], [function-calling], [whatsapp], [backend], [api], [produto], [mvp]

## 2026-05-07 - IA aplicada ao próprio desenvolvimento (Claude Code, Cursor/Antigravity)
- Contexto: Adoção intensa de assistentes de IA como parte do fluxo de desenvolvimento diário — tanto em features novas quanto em refactor de legado.
- Atribuicao: produtividade, qualidade
- Acoes:
  - uso intenso de **Claude Code** e **Cursor/Antigravity** em brainstorm de design, debug, escrita de código, geração de testes e refatoração;
  - hábito de prompts iterativos, revisão crítica do output e integração ao fluxo de PR;
  - aplicação direta no MVP do WhatsApp conversacional, viabilizando entrega em 2 semanas.
- Tecnologias: Claude Code, Cursor/Antigravity, PHP, Symfony, PHPUnit.
- Impacto:
  - **aumento da cobertura de testes** em módulos onde antes não havia;
  - **aumento da velocidade de desenvolvimento** — entregas que antes levavam semanas reduzidas a dias;
  - melhor qualidade em refactor de legado por geração + validação assistidas.
- Evidencias:
  - PRs com testes adicionados;
  - MVP do WhatsApp conversacional em 2 semanas.
- Tags: [ia], [produtividade], [testes], [refactor], [dev-experience]

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
