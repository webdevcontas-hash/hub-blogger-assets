# hub-blogger-assets — Contexto para IA

> Atualizado em: 30/07/2026 | Leia este arquivo antes de qualquer alteração no projeto.

---

## O que é este projeto

Repositório de **imagens hospedadas publicamente** usadas nos posts do blog `hub-blogger`. As imagens são geradas automaticamente por IA (NVIDIA Flux) a cada novo post publicado, e este repo serve apenas para hospedar essas imagens via GitHub (raw/CDN) para embutir nos posts do Blogger.

**Pasta local:** `C:\Github\publicados\hub-blogger-assets\`
**Repositório:** `https://github.com/webdevcontas-hash/hub-blogger-assets.git`

---

## Stack e tecnologias

- **Frontend:** N/A (repositório é só storage de imagens estáticas)
- **Backend:** N/A — alimentado pelo pipeline de automação do projeto `hub-blogger`
- **Banco de dados:** N/A
- **Infra/Deploy:** GitHub (arquivos servidos via raw.githubusercontent.com ou similar)

---

## Estrutura de arquivos relevante

```
hub-blogger-assets/
├── README.md
├── posts/          ← imagens PNG geradas por post (nome = UUID)
├── PROGRESSO.md
├── CONTEXTO-IA.md
└── HANDOFF.md
```

---

## Módulos / Funcionalidades

| Módulo | Caminho/Arquivo | Descrição |
|--------|-----------------|-----------|
| Imagens de posts | `posts/*.png` | Uma imagem por post do blog, nome de arquivo = UUID gerado no momento da criação |

---

## Regras técnicas importantes

1. Este repositório é alimentado automaticamente pelo pipeline do projeto `hub-blogger` — não editar manualmente os arquivos em `posts/` a menos que seja para remover uma imagem obsoleta/quebrada.
2. Não renomear arquivos existentes em `posts/` — os nomes (UUID) são referenciados diretamente nos posts já publicados no Blogger.

---

## Máquinas e responsáveis

| Máquina | Responsável | IA | Última sessão |
|---------|-------------|-----|---------------|
| DELL (Renan Notebook Gordon) | Renan | Claude Code | 30/07/2026 |

---

## Como testar localmente

Não aplicável — repositório sem build/execução, apenas armazenamento de imagens.
