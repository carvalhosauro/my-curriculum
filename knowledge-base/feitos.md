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
