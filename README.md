# Central de Checklists Fiscais — Nascel

Checklist operacional de fechamento mensal (Simples Nacional, Lucro Presumido, Lucro Real e MEI).

Site estático: abra `index.html` no navegador ou publique no Render / GitHub Pages.

As marcações ficam salvas no `localStorage` do navegador de cada usuário.

## Publicar no GitHub + Render

### 1) GitHub

1. Crie um repositório novo (ex.: `checklists-fiscais-nascel`).
2. Pode ser **Private** (só o time) ou Public.
3. Não marque "Add README" se for subir esta pasta já pronta.
4. No computador, nesta pasta, rode:

```bash
git init
git add .
git commit -m "Primeira versão do checklist fiscal"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/checklists-fiscais-nascel.git
git push -u origin main
```

### 2) Render (Static Site)

1. Em [dashboard.render.com](https://dashboard.render.com) → **New +** → **Static Site**.
2. Conecte a conta GitHub e selecione o repositório.
3. Configure:
   - **Name:** `checklists-fiscais-nascel`
   - **Branch:** `main`
   - **Build Command:** (deixe vazio)
   - **Publish Directory:** `.`
4. Clique em **Create Static Site**.
5. (Opcional) Em **Settings → Custom Domains**, adicione seu domínio e aponte o DNS conforme o Render indicar.

Pronto: a cada `git push` na `main`, o site atualiza sozinho.
