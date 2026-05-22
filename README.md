# Iara Modas Calçados

Site institucional da Iara Modas Calçados — Leme/SP.
Arquivo único em HTML/CSS/JS puro, sem frameworks.

🌐 **Site em produção:** https://iara-modas.surge.sh

## Conteúdo

- `index.html` — site completo (HTML + CSS + JS inline)
- `CNAME` — domínio do Surge.sh
- `.github/workflows/deploy.yml` — deploy automático a cada push

## Deploy

### Automático (GitHub Actions)
Todo `git push` para a branch `main` dispara um deploy para `iara-modas.surge.sh`.

Para funcionar, configure dois secrets no repositório GitHub
(Settings → Secrets and variables → Actions → New repository secret):

| Secret         | Valor                                                              |
| -------------- | ------------------------------------------------------------------ |
| `SURGE_LOGIN`  | E-mail da conta no Surge (ex.: `seuemail@gmail.com`)               |
| `SURGE_TOKEN`  | Token gerado com `surge token` no terminal local                   |

### Manual (local)
```bash
npm install -g surge
surge ./ iara-modas.surge.sh
```

## Stack

- HTML semântico
- CSS puro com variáveis (Custom Properties)
- JS vanilla (IntersectionObserver, sem libs)
- Google Fonts: Fraunces + Inter
- Paleta extraída da fachada real da loja
