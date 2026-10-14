# Synth Wing — site (GitHub Pages)

Site estático do jogo **Synth Wing**: landing page + política de privacidade.
Não precisa de build — é HTML/CSS puro, pronto para o GitHub Pages.

## Arquivos
- `index.html` — página principal (detalhes do jogo)
- `privacidade.html` — política de privacidade (URL exigida pelo Google Play)
- `assets/splash.png`, `assets/icon.png` — artes

## Dados do desenvolvedor (já preenchidos)
- Desenvolvedor: **SOCM** (igual ao Play Console)
- Contato: **marcos.barbosa.develop@gmail.com**
- Obs.: o ID do pacote continua `com.hermes.beatneon` (não muda o nome da loja; não precisa alterar nada na política).

## Publicar no GitHub Pages (passo a passo)
```bash
cd ~/godot-projetos/synth-wing-site
git init
git add .
git commit -m "Site Synth Wing: landing + privacidade"
```
1. Crie um repositório novo no github.com (ex.: `synth-wing-site`), **público**.
2. Conecte e envie:
   ```bash
   git remote add origin https://github.com/SEU-USUARIO/synth-wing-site.git
   git branch -M main
   git push -u origin main
   ```
3. No repositório: **Settings → Pages → Source: Deploy from a branch → `main` / root → Save**.
4. Em ~1 min o site fica em:
   `https://SEU-USUARIO.github.io/synth-wing-site/`

## No Google Play Console
- **Política de privacidade** (App content → Política de privacidade): cole a URL
  `https://SEU-USUARIO.github.io/synth-wing-site/privacidade.html`
  (pode colar a URL da página inicial também, mas o link direto da privacidade é mais seguro).
- **Segurança de dados**: marque "Nenhum dado coletado" — bate com a política.
- A política deve estar no idioma da ficha da loja (pt-BR ✔). Se listar em outros idiomas,
  crie uma versão em inglês da `privacidade.html`.