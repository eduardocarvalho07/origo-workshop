# Órigo Energia - Workshop de Objetivos Estratégicos

Plataforma web para gerenciar workshops de objetivos estratégicos com votação, refinamento IA-assistido, e painel de administrador.

## 🚀 Deploy no Vercel (3 minutos)

### Opção 1: Deploy com GitHub (Recomendado)

1. **Crie um repositório no GitHub**
   - Vá para https://github.com/new
   - Nome: `origo-workshop`
   - Descrição: "Workshop de Objetivos Estratégicos"
   - Clique em "Create repository"

2. **Clone o repositório localmente**
   ```bash
   git clone https://github.com/SEU_USUARIO/origo-workshop.git
   cd origo-workshop
   ```

3. **Copie os arquivos para o repositório**
   - Copie `origo_workshop.html` para a pasta
   - Copie `vercel.json` para a pasta
   - Copie este `README.md` para a pasta

4. **Faça commit e push**
   ```bash
   git add .
   git commit -m "Inicial: Workshop de Objetivos Estratégicos"
   git push origin main
   ```

5. **Deploy no Vercel**
   - Vá para https://vercel.com
   - Clique em "New Project"
   - Selecione seu repositório GitHub `origo-workshop`
   - Clique em "Deploy"
   - **Pronto!** Sua URL será `https://origo-workshop.vercel.app`

---

### Opção 2: Deploy via Vercel CLI (Alternativo)

1. **Instale o Vercel CLI**
   ```bash
   npm install -g vercel
   ```

2. **Deploy diretamente**
   ```bash
   vercel
   ```
   - Siga as instruções na tela
   - Responda "Y" para criar um novo projeto
   - Escolha seu account Vercel

3. **Pronto!** Você receberá uma URL pública

---

## 🔐 Acesso de Administrador

**Senha padrão:** `Falconi2024`

Para alterar a senha, edite o arquivo `origo_workshop.html`:
```javascript
const ADMIN_PASSWORD = 'SUA_NOVA_SENHA'; // Linha ~828
```

### Funcionalidades de Admin
- ⚙️ Clique no botão no canto inferior direito para acessar
- 🗑️ Deletar objetivos estratégicos individuais
- 🗑️ Deletar ambições finais
- 🗑️ Limpar todos os dados (com dupla confirmação)
- 📊 Ver estatísticas em tempo real

---

## 📋 Como Usar

### Fase 1: Votação
1. Cadastre os nomes dos diretores
2. Cada um insere objetivos para as 3 dimensões
3. Todos votam nas opções que veem

### Fase 2: Refinamentos
1. O sistema identifica automaticamente os mais votados
2. Digite sugestões de refinamento
3. IA gera 5 opções melhoradas
4. Selecione qual será incorporada

### Fase 3: Mapa Final
1. Visualize os 3 objetivos eleitos
2. Pronto para apresentação

### Fase 4: Ambição Final
1. Cada diretor escreve sua ambição para a Órigo
2. Votação e seleção da ambição vencedora
3. Veja o resumo final com tudo integrado

---

## 💾 Dados Persistidos Automaticamente

Todos os dados são salvos automaticamente no navegador (LocalStorage):
- Objetivos estratégicos
- Votos
- Refinamentos
- Ambições
- Seleções finais

**Backup:** Exporte em JSON ou CSV a qualquer momento (botão na Fase 3/4)

---

## 🎨 Padrões Visuais

- **Cores Falconi:** Olive (#7A7423), Lime (#A7E82B), Off-white (#EAEBE9)
- **Responsivo:** Funciona em desktop, tablet e mobile
- **Sem dependências externas:** Roda 100% offline

---

## 🔧 Customização

### Alterar a senha de admin
Edite `origo_workshop.html`, linha ~828:
```javascript
const ADMIN_PASSWORD = 'SUA_SENHA_AQUI';
```

### Alterar cores Falconi
Edite as variáveis CSS no início do arquivo:
```css
--falconi-olive: #7A7423;
--falconi-lime: #A7E82B;
--falconi-off-white: #EAEBE9;
```

### Adicionar mais dimensões
No JavaScript, modifique:
```javascript
const DIMENSIONS = ['Eficiência', 'Clientes', 'Expansão/Novos Negócios', 'Sua Nova Dimensão'];
```

---

## 📊 Exportação de Dados

- **JSON:** Estrutura completa para processamento
- **CSV:** Para análise em Excel/Sheets
- **Impressão:** Print-friendly para documentação

---

## 🐛 Suporte

Dúvidas ou problemas?
- Verifique o console do navegador (F12)
- Limpe o cache e recarregue (Ctrl+Shift+Del)
- Teste em outro navegador

---

## 📝 Notas de Versão

### v1.0 (Atual)
- ✅ 4 fases completas
- ✅ Painel de administrador com delete
- ✅ Geração de refinamentos por IA
- ✅ Exportação JSON/CSV
- ✅ Persistência local
- ✅ Design responsivo

---

**Workshop de Objetivos Estratégicos - Órigo Energia**  
Desenvolvido com ❤️ pela Falconi Consultoria
