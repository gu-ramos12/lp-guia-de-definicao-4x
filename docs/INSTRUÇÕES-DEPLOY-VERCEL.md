# 📦 Instruções para Deploy no Vercel - Guia de Definição 4X

## 🖼️ PASSO 1: Preparar as Imagens

### A) Imagens de Transformação

1. **Salve suas imagens de transformação** no diretório:
   ```
   public/images/transformations/
   ```

2. **Nomeie as imagens** exatamente como:
   - `transformation1.png`
   - `transformation2.png`
   - `transformation3.png`
   - `transformation4.png`
   - `transformation5.png`
   - `transformation6.png`
   - `transformation7.png`

### B) Logo

1. **Salve a logo** no diretório:
   ```
   public/images/logo/
   ```

2. **Nome obrigatório**:
   - `logo.png`

### C) Imagens da Seção "Conheça Rodrigo Brasileiro"

1. **Salve as 8 imagens do carrossel** no diretório:
   ```
   public/images/coach/
   ```

2. **Nomeie as imagens** exatamente como:
   - `coach1.png` - Foto profissional do Rodrigo
   - `coach2.png` - Quem é Rodrigo Brasileiro
   - `coach3.png` - Formação Acadêmica
   - `coach4.png` - Certificação Internacional
   - `coach5.png` - Vivência no Esporte
   - `coach6.png` - Estilo de Trabalho
   - `coach7.png` - Treino Individualizado
   - `coach8.png` - Venha fazer parte do time

   ⚠️ **IMPORTANTE**: Use exatamente esses nomes! O código está configurado para buscar essas imagens.

## 📁 PASSO 2: Preparar os Arquivos

### Arquivos que você DEVE usar no deploy (todos com prefixo "USAR"):

#### Arquivos de Configuração:
1. **USAR-package.json** → Renomeie para `package.json`
2. **USAR-vite.config.ts** → Renomeie para `vite.config.ts`
3. **USAR-vercel.json** → Renomeie para `vercel.json`
4. **USAR-tsconfig.json** → Renomeie para `tsconfig.json`
5. **USAR-tsconfig.node.json** → Renomeie para `tsconfig.node.json`

#### Arquivos Principais:
6. **USAR-index.html** → Renomeie para `index.html`
7. **USAR-App.tsx** → Renomeie para `App.tsx`
8. **USAR-main.tsx** → Renomeie para `main.tsx` e coloque na pasta `src/`

### Estrutura Final do Projeto:

```
seu-projeto/
├── public/
│   └── images/
│       ├── logo/
│       │   └── logo.png
│       ├── coach/
│       │   ├── coach1.png
│       │   ├── coach2.png
│       │   ├── coach3.png
│       │   ├── coach4.png
│       │   ├── coach5.png
│       │   ├── coach6.png
│       │   ├── coach7.png
│       │   └── coach8.png
│       └── transformations/
│           ├── transformation1.png
│           ├── transformation2.png
│           ├── transformation3.png
│           ├── transformation4.png
│           ├── transformation5.png
│           ├── transformation6.png
│           └── transformation7.png
├── src/
│   └── main.tsx
├── components/
├── styles/
├── App.tsx
├── index.html
├── package.json
├── vite.config.ts
├── vercel.json
├── tsconfig.json
└── tsconfig.node.json
```

## 🚀 PASSO 3: Deploy no Vercel

### Opção A: Deploy via Interface Web (Recomendado)

1. Acesse [vercel.com](https://vercel.com)
2. Faça login ou crie uma conta
3. Clique em **"Add New Project"**
4. Clique em **"Import Git Repository"** ou faça upload do projeto
5. Configure o projeto:
   - **Framework Preset**: Vite
   - **Build Command**: `npm run build`
   - **Output Directory**: `dist`
   - **Install Command**: `npm install`
6. Clique em **"Deploy"**

### Opção B: Deploy via CLI

1. Instale o Vercel CLI:
   ```bash
   npm install -g vercel
   ```

2. No diretório do projeto, execute:
   ```bash
   vercel login
   vercel
   ```

3. Siga as instruções no terminal

## ✅ Verificações Finais

Antes de fazer o deploy, certifique-se de que:

### Imagens:
- [ ] Logo (`logo.png`) está em `public/images/logo/`
- [ ] 8 imagens do coach (coach1.png a coach8.png) estão em `public/images/coach/`
- [ ] 7 imagens de transformação (transformation1.png a transformation7.png) estão em `public/images/transformations/`
- [ ] Todas as imagens estão nomeadas exatamente como especificado

### Arquivos:
- [ ] Todos os arquivos com "USAR" foram renomeados removendo o prefixo
- [ ] `main.tsx` foi movido para dentro da pasta `src/`
- [ ] Os arquivos de configuração estão na raiz do projeto:
  - [ ] `package.json`
  - [ ] `vite.config.ts`
  - [ ] `vercel.json`
  - [ ] `tsconfig.json`
  - [ ] `tsconfig.node.json`
  - [ ] `index.html`
  - [ ] `App.tsx`

## 🔧 Solução de Problemas

### Imagens não aparecem após o deploy:

1. Verifique se as imagens estão no diretório `public/images/transformations/`
2. Confirme os nomes dos arquivos (devem ser exatamente como especificado)
3. Limpe o cache do Vercel e faça redeploy

### Erro de build:

1. Execute localmente: `npm install` e depois `npm run build`
2. Corrija quaisquer erros que aparecerem
3. Faça commit das correções e redeploy

## 📞 Contato

Se precisar de ajuda, entre em contato via WhatsApp: (19) 99297-1195

---

**Rodrigo Brasileiro Team** 💪
Landing Page - Guia de Definição 4X
