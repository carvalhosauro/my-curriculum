# Playbook Agent-Like para atualizar curriculos

Este playbook padroniza como um agente deve trabalhar com sua base.

## Entrada minima

- `feitos.md` atualizado;
- um contexto de `vagas/` OU `atribuicoes/`.

## Passos do agente

1. Ler feitos recentes e selecionar os mais relevantes ao contexto.
2. Mapear requisitos (vaga) ou resultado esperado (atribuicao).
3. Gerar relatorio padrao em `relatorios/` usando o template correto.
4. Propor ajustes no curriculo alvo em `v0/` com foco em impacto.
5. Preservar fatos; nao inventar experiencia.

## Regras de qualidade

- Priorizar impacto mensuravel;
- Usar verbos de acao claros (implementei, reduzi, estabilizei, instrumentei);
- Limitar narrativa a contexto + acao + resultado;
- Sinalizar gaps com plano realista;
- Evitar inflar senioridade.

## Prompt sugerido para uso rapido

```txt
Use a base em knowledge-base/feitos.md e o contexto em [arquivo de vaga ou atribuicao].
Gere um relatorio padrao em knowledge-base/relatorios/ com:
1) match de requisitos,
2) top impactos,
3) bullets prontas para curriculo,
4) gaps e plano curto.
Depois proponha ajustes no curriculo mais adequado dentro de v0/.
Nao invente dados.
```
