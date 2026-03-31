---
name: curriculo-agent-like
description: Gerencia a base de carreira e gera currículos customizados. Use quando o usuário avisar novo emprego/habilidade/certificação (Fluxo A) ou compartilhar um link de vaga para gerar currículo customizado (Fluxo B).
---

# Curriculo Agent-Like

## Fontes de dados

```
knowledge-base/perfil/          ← dados estruturados da carreira
  dados-pessoais.md             ← contato, links
  experiencias.md               ← histórico de empregos
  habilidades.md                ← inventário de habilidades com nível
  certificacoes.md              ← certificações
  formacao.md                   ← formação acadêmica + idiomas

knowledge-base/feitos.md        ← realizações com impacto mensurável
knowledge-base/vagas/           ← contextos de vagas (gerados pelo Fluxo B)
knowledge-base/relatorios/      ← relatórios gerados (output do Fluxo B)
v0/                             ← currículos HTML (output do Fluxo B)
```

---

## Fluxo A — Atualizar dados do perfil

**Ativar quando:** usuário avisar "novo emprego", "nova habilidade", "nova certificação", "novo feito" ou semelhante.

**Passos:**

1. Consultar `knowledge-base/QUANDO-ATUALIZAR.md` para identificar qual(is) arquivo(s) atualizar.
2. Ler o(s) arquivo(s) alvo para entender o formato existente.
3. Se faltar informação, perguntar ao usuário o mínimo necessário (ver guia `QUANDO-ATUALIZAR.md`).
4. Atualizar o(s) arquivo(s) seguindo o modelo já existente no arquivo.
5. Se o evento for "novo feito", verificar se alguma habilidade nova surgiu e perguntar se deve atualizar `habilidades.md` também.

**Regra:** nunca inventar dados — atualizar apenas com o que o usuário forneceu.

---

## Fluxo B — Gerar currículo customizado por URL

**Ativar quando:** usuário compartilhar link de vaga.

**Passos:**

1. **Buscar e extrair a vaga**
   - `WebFetch(url)` para obter o conteúdo da página
   - Extrair: empresa, cargo, senioridade, requisitos obrigatórios, stack, diferenciais, responsabilidades

2. **Criar contexto de vaga**
   - Salvar em `knowledge-base/vagas/YYYY-MM-DD-empresa.md` usando o template de `knowledge-base/vagas/template-vaga.md`
   - Classificar requisitos em P0 (obrigatório), P1 (forte diferencial), P2 (nice-to-have)

3. **Ler a base completa**
   - Ler todos os arquivos de `knowledge-base/perfil/`
   - Ler `knowledge-base/feitos.md`

4. **Mapear aderência**
   - Para cada requisito P0/P1: `requisito → feito/habilidade → evidência → nível de aderência`
   - Identificar gaps reais (sem minimizar)

5. **Gerar relatório**
   - Salvar em `knowledge-base/relatorios/YYYY-MM-DD-empresa.md`
   - Usar template de `knowledge-base/relatorios/template-relatorio-vaga.md`
   - Incluir: match de requisitos, top 3 impactos, ajustes de narrativa, gaps com plano realista

6. **Gerar currículo HTML customizado**
   - Usar o HTML existente mais próximo do perfil da vaga (em `v0/`) como base
   - Reordenar bullets por relevância para a vaga
   - Ajustar resumo, tagline e competências
   - Salvar como `v0/YYYY-MM-DD-empresa.html`

---

## Regras de escrita (ambos os fluxos)

- Bullet: **contexto + ação + resultado mensurável**
- Usar verbos de impacto: `implementei`, `reduzi`, `estabilizei`, `instrumentei`, `automatizei`
- Priorizar números e evidências concretas
- Nunca inflar senioridade ou inventar experiência
- Sinalizar gaps com plano realista, sem exagero

---

## Checklist rápido (Fluxo B)

- [ ] Buscou a URL e extraiu requisitos reais da vaga
- [ ] Criou arquivo de contexto em `vagas/`
- [ ] Leu todos os arquivos de `perfil/` + `feitos.md`
- [ ] Gerou relatório de aderência em `relatorios/`
- [ ] HTML gerado tem apenas fatos da base
- [ ] Gaps foram sinalizados sem exagero
