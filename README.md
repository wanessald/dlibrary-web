# dlibrary-web

Frontend do D.Library — interface de gestão de leituras com recomendações via grafo.

**Stack:** Next.js · TypeScript · Tailwind CSS  
**Deploy:** Fly.io — `https://dlibrary-web.fly.dev` _(em breve)_

---

## Sprint 0 — Fundação do Projeto

> **Status:** ✅ Completo  
> **Repositório:** dlibrary-web

### O que foi construído

No Sprint 0, geramos a estrutura inicial do frontend com Next.js, Typescript e Tailwind CSS. Criamos o `lib/api.ts`, cliente HTTP centralizado que encapsula toda a comunicação com a API. Dessa forma, em vez de cada componente fazer requisições diretamente para URLs, as chamadas passam por esse cliente, que já inclui o header de autenticação e a URL base configurada via variável de ambiente `NEXT_PUBLIC_API_URL`.

### Ambientes

- **Local:** `http://localhost:3001`
- **Produção:** Fly.io _(Sprint 11)_

### Como rodar localmente

```bash
npm install
npm run dev
```

Verificar: `http://localhost:3001` carrega a página inicial

### Variáveis de ambiente

Copie `.env.local.example` para `.env.local` e preencha:

```
NEXT_PUBLIC_API_URL=http://localhost:3000
```
