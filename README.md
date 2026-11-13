# Landing Page - Dra. Thaiany B. Benito

Site institucional e protótipo de apresentação para a médica Dra. Thaiany B. Benito (Medicina Estética · CRM-SP 135211). Desenvolvido pela RogerWeb.

---

## 🚀 Como publicar no GitHub Pages

Este projeto está pronto e configurado para publicação automática no **GitHub Pages** através do **GitHub Actions**.

### 1. Criar o repositório no GitHub
1. Acesse [github.com/new](https://github.com/new).
2. Dê um nome ao repositório (exemplo: `dra-thaiany` ou `dra-thaiany-site`).
3. Mantenha o repositório como **Público** (ou Privado se tiver conta GitHub Pro).
4. Não adicione README, `.gitignore` ou licença (já criados localmente).
5. Clique em **Create repository**.

### 2. Conectar e enviar os arquivos locais para o GitHub
No terminal desta pasta, execute os comandos abaixo substituindo `<SEU_USUARIO>` e `<SEU_REPOSITORIO>`:

```bash
git remote add origin https://github.com/<SEU_USUARIO>/<SEU_REPOSITORIO>.git
git branch -M main
git push -u origin main
```

### 3. Ativar o GitHub Pages
1. No seu repositório no GitHub, clique na aba **Settings** (Configurações).
2. No menu lateral esquerdo, clique em **Pages** (dentro da seção *Code and automation*).
3. Em **Build and deployment** > **Source**, selecione:
   - **GitHub Actions** (Recomendado - utilizará o workflow automático em `.github/workflows/deploy.yml`).
   *(Alternativa clássica: se preferir sem actions, selecione `Deploy from a branch`, escolha a branch `main` e a pasta `/ (root)`, depois clique em Save).*

### 4. Acessar o site
Assim que o deploy for concluído (geralmente leva menos de 1 minuto), o link do site estará visível na página de **Pages** ou na aba **Actions**:
`https://<SEU_USUARIO>.github.io/<SEU_REPOSITORIO>/`

---

## 🌐 Domínio Personalizado (Opcional)

Se desejar apontar um domínio próprio (ex: `drathaianybbenito.com.br` ou `proposta.drathaianybbenito.com.br`):
1. Crie um arquivo chamado `CNAME` na raiz com o seu domínio (ex: `proposta.drathaianybbenito.com.br`).
2. No seu provedor de DNS (ex: Cloudflare, Registro.br, Hostinger), crie o apontamento CNAME para `<SEU_USUARIO>.github.io`.
3. Nas configurações do GitHub Pages (**Settings > Pages**), preencha o campo **Custom domain** e marque **Enforce HTTPS**.

---

## 📁 Estrutura de Arquivos

- `index.html`: Página principal responsiva com quiz interativo, detalhes de procedimentos e integração com WhatsApp.
- `404.html`: Página de erro 404 personalizada.
- `.nojekyll`: Desativa o processador Jekyll padrão do GitHub Pages para garantir o carregamento correto de todos os recursos.
- `.github/workflows/deploy.yml`: Workflow do GitHub Actions para deploy automático a cada push na branch `main`.
- `.gitignore`: Arquivos e diretórios ignorados pelo Git.
