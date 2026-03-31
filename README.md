# My curriculum

Repositório de dados de carreira e geração de currículos customizados em HTML/PDF.

## Casos de uso

### 1. Atualizar dados da carreira

Sempre que acontecer um evento (novo emprego, nova habilidade, nova certificação), consulte `knowledge-base/QUANDO-ATUALIZAR.md` — ou simplesmente avise o agente o que mudou e ele sabe o que atualizar.

### 2. Gerar currículo customizado por vaga

Compartilhe o link da vaga. O agente:
1. Busca e extrai os requisitos da página
2. Cria o contexto em `knowledge-base/vagas/`
3. Lê sua base de perfil + feitos
4. Gera um relatório de aderência em `knowledge-base/relatorios/`
5. Gera o currículo HTML customizado em `v0/`

---

## Estrutura

```
knowledge-base/
├── perfil/                   ← fonte de dados da carreira
│   ├── dados-pessoais.md    ← contato, links
│   ├── experiencias.md      ← histórico de empregos
│   ├── habilidades.md       ← inventário de habilidades com nível
│   ├── certificacoes.md     ← certificações
│   └── formacao.md          ← formação acadêmica + idiomas
│
├── feitos.md                 ← realizações com impacto mensurável
├── QUANDO-ATUALIZAR.md       ← guia: qual arquivo atualizar para cada evento
│
├── vagas/                    ← contextos de vagas (gerado pelo agente)
├── atribuicoes/              ← contextos por tipo de responsabilidade
└── relatorios/               ← relatórios de aderência (output do agente)

v0/                           ← currículos HTML (customizados por vaga ou por perfil)
```

## Exportar para PDF

1. Abra o HTML desejado no navegador.
2. Use **Print** (`Ctrl+P` / `Cmd+P`).
3. Escolha **Save as PDF**.
4. Use papel **A4** e ative fundos/gráficos para manter o layout.
