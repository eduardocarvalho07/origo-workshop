# 🚀 Setup Vercel - Guia Rápido

## Passo 1: Prepare o Repositório GitHub

```bash
# Crie uma pasta local
mkdir origo-workshop
cd origo-workshop

# Inicie um repositório Git
git init

# Copie os arquivos aqui:
# - origo_workshop.html
# - vercel.json
# - README.md
# - .gitignore

# Faça o primeiro commit
git add .
git commit -m "Inicial: Workshop Objetivos Estratégicos"
```

## Passo 2: Suba para GitHub

1. Vá para https://github.com/new
2. Crie um repositório chamado `origo-workshop`
3. Copie a URL do repositório
4. No terminal:

```bash
git remote add origin https://github.com/SEU_USUARIO/origo-workshop.git
git branch -M main
git push -u origin main
```

## Passo 3: Deploy no Vercel

### Opção A: Via Vercel Dashboard (Recomendado)

1. Vá para https://vercel.com
2. Se não tiver conta, crie uma (grátis)
3. Clique em **"Add New..."** → **"Project"**
4. Clique em **"Import Git Repository"**
5. Cole a URL do seu repositório GitHub
6. Clique em **"Import"**
7. Clique em **"Deploy"**

**Pronto!** Você terá uma URL como:
```
https://origo-workshop.vercel.app
```

### Opção B: Via Vercel CLI

```bash
# Instale o CLI
npm install -g vercel

# Na pasta do projeto, execute:
vercel

# Siga as instruções na tela
# Resultado: seu projeto estará online
```

## Passo 4: Teste a Ferramenta

1. Abra sua URL no navegador
2. Adicione alguns diretores e objetivos
3. Clique no botão ⚙️ (canto inferior direito)
4. Digite a senha: `Falconi2024`
5. Teste a funcionalidade de delete

## Passo 5: Personalize (Opcional)

### Mudar a Senha de Admin

No arquivo `origo_workshop.html`, procure por:
```javascript
const ADMIN_PASSWORD = 'Falconi2024';
```

Altere para sua senha:
```javascript
const ADMIN_PASSWORD = 'SUA_SENHA_AQUI';
```

Depois faça:
```bash
git add origo_workshop.html
git commit -m "Alterar senha de admin"
git push
```

**O Vercel atualiza automaticamente!**

## 🔄 Atualizações Futuras

Sempre que precisar fazer mudanças:

```bash
# Edite os arquivos localmente
nano origo_workshop.html

# Faça commit
git add .
git commit -m "Descrever a mudança"

# Faça push
git push

# Vercel atualiza automaticamente em ~30 segundos
```

---

## 📱 Compartilhe com os Diretores

Envie esta URL para todos:
```
https://origo-workshop.vercel.app
```

Cada um acessa, contribui, e os dados são salvos localmente no navegador deles.

Você como admin pode:
- Acessar a URL
- Clique no ⚙️
- Senha: `Falconi2024`
- Deletar objetivos ou ambições que tenham erros

---

## 🆘 Troubleshooting

### "Erro ao fazer deploy no Vercel"
- Certifique-se que todos os arquivos foram feito push
- Verifique se o repositório é público
- Tente novamente em alguns minutos

### "Página em branco"
- Verifique o console (F12 → Console)
- Recarregue a página (Ctrl+Shift+R)
- Tente em outro navegador

### "Dados sumiram"
- Os dados são salvos no navegador
- Limpe cache raramente apaga dados
- Exporte em JSON regularmente para backup

---

**Dúvidas? Consulte o README.md para mais informações.**
