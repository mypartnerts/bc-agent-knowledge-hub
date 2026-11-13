# Patch de indexação para Copilot Studio

Copie o conteúdo deste ZIP para a raiz do repositório, mantendo as pastas ocultas, e faça commit.

Este patch:

- gera uma página inicial com links HTML reais;
- cria índices para `routing`, `domains`, `policies` e `sources` com base nos ficheiros existentes;
- adiciona metadados Jekyll aos Markdown que ainda não os tenham;
- gera `robots.txt` e `sitemap.xml`;
- publica o site por GitHub Actions.

## Após o commit

1. Em **Settings > Pages**, escolha **Source: GitHub Actions**.
2. Abra **Actions > Build and deploy GitHub Pages** e confirme que o workflow terminou com sucesso.
3. Valide:
   - `https://mypartnerts.github.io/bc-agent-knowledge-hub/`
   - `https://mypartnerts.github.io/bc-agent-knowledge-hub/AGENTS.html`
   - `https://mypartnerts.github.io/bc-agent-knowledge-hub/routing/`
   - `https://mypartnerts.github.io/bc-agent-knowledge-hub/sitemap.xml`
4. Atualize ou volte a adicionar a Knowledge Source no Copilot Studio.

Nota: o workflow gera os índices durante o deployment. Os ficheiros gerados não precisam de ser gravados no branch.
