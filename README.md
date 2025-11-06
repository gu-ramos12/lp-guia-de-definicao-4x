_# 🎯 Guia de Definição 4X - Landing Page

Projeto de landing page para o programa **Guia de Definição 4X** do coach Rodrigo Brasileiro.

## 🚀 Tecnologias

- **React 18.2**
- **TypeScript**
- **Vite 5.2**
- **Tailwind CSS 4.0**
- **Radix UI** (componentes)
- **Lucide React** (ícones)

## 📦 Instalação

```bash
# Instalar dependências
npm install

# Rodar em desenvolvimento
npm run dev

# Build para produção
npm run build

# Preview do build
npm run preview
```

## 🖼️ Configuração de Imagens

Antes de fazer o deploy, adicione suas imagens nas seguintes pastas:

### 1. Logo
📁 `public/images/logo/logo.png`

### 2. Imagens do Coach (8 imagens)
📁 `public/images/coach/`
- coach1.png até coach8.png

### 3. Imagens de Transformação (7 imagens)
📁 `public/images/transformations/`
- transformation1.png até transformation7.png

📖 **Veja instruções detalhadas em:** `docs/GUIA-RAPIDO-IMAGENS.md`

## 🌐 Deploy no Vercel

### Opção 1: Via Interface Web (Recomendado)

1. Acesse [vercel.com](https://vercel.com)
2. Clique em "Add New Project"
3. Importe seu repositório Git
4. Configure:
   - **Framework Preset:** Vite
   - **Build Command:** `npm run build`
   - **Output Directory:** `dist`
5. Clique em "Deploy"

### Opção 2: Via CLI

```bash
npm install -g vercel
vercel login
vercel --prod
```

📖 **Instruções completas em:** `docs/INSTRUÇÕES-DEPLOY-VERCEL.md`

## 📁 Estrutura do Projeto

```
guia-definicao-4x/
├── src/
│   ├── components/     # Componentes React
│   ├── styles/         # Estilos globais
│   ├── App.tsx         # Componente principal
│   └── main.tsx        # Entry point
├── public/
│   └── images/         # Imagens estáticas
├── docs/               # Documentação
├── package.json        # Dependências
├── vite.config.ts      # Configuração Vite
└── vercel.json         # Configuração Vercel
```

## 📞 Contato

**Rodrigo Brasileiro Team**
- WhatsApp: (19) 99297-1195
- Horário: Seg-Sex, 9h às 18h

---

Desenvolvido com ❤️ para transformar vidas através do fitness_
