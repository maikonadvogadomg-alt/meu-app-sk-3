# PLANO DO PROJETO: Meu App

> Gerado em: 14/07/2026, 17:54:53
> Arquivos: 115 | Linhas de código: ~37.428

---

## RESUMO EXECUTIVO

- **Tipo:** Full-Stack (React + Express)
- **Frontend/Stack:** React + Vite, TypeScript, Tailwind CSS
- **Backend/Dados:** Node.js + Express, PostgreSQL
- **Versão:** 1.0.0



---

## ESTRUTURA DE ARQUIVOS

```
Meu App/
├── electron/
│   ├── main.cjs
│   └── preload.cjs
├── public/
│   └── manifest.webmanifest
├── src/
│   ├── components/
│   │   ├── ui/
│   │   │   ├── accordion.tsx
│   │   │   ├── alert-dialog.tsx
│   │   │   ├── alert.tsx
│   │   │   ├── aspect-ratio.tsx
│   │   │   ├── avatar.tsx
│   │   │   ├── badge.tsx
│   │   │   ├── breadcrumb.tsx
│   │   │   ├── button-group.tsx
│   │   │   ├── button.tsx
│   │   │   ├── calendar.tsx
│   │   │   ├── card.tsx
│   │   │   ├── carousel.tsx
│   │   │   ├── chart.tsx
│   │   │   ├── checkbox.tsx
│   │   │   ├── collapsible.tsx
│   │   │   ├── command.tsx
│   │   │   ├── context-menu.tsx
│   │   │   ├── dialog.tsx
│   │   │   ├── drawer.tsx
│   │   │   ├── dropdown-menu.tsx
│   │   │   ├── empty.tsx
│   │   │   ├── field.tsx
│   │   │   ├── form.tsx
│   │   │   ├── hover-card.tsx
│   │   │   ├── input-group.tsx
│   │   │   ├── input-otp.tsx
│   │   │   ├── input.tsx
│   │   │   ├── item.tsx
│   │   │   ├── kbd.tsx
│   │   │   ├── label.tsx
│   │   │   ├── menubar.tsx
│   │   │   ├── navigation-menu.tsx
│   │   │   ├── pagination.tsx
│   │   │   ├── popover.tsx
│   │   │   ├── progress.tsx
│   │   │   ├── radio-group.tsx
│   │   │   ├── resizable.tsx
│   │   │   ├── scroll-area.tsx
│   │   │   ├── select.tsx
│   │   │   ├── separator.tsx
│   │   │   ├── sheet.tsx
│   │   │   ├── sidebar.tsx
│   │   │   ├── skeleton.tsx
│   │   │   ├── slider.tsx
│   │   │   ├── sonner.tsx
│   │   │   ├── spinner.tsx
│   │   │   ├── switch.tsx
│   │   │   ├── table.tsx
│   │   │   ├── tabs.tsx
│   │   │   ├── textarea.tsx
│   │   │   ├── toast.tsx
│   │   │   ├── toaster.tsx
│   │   │   ├── toggle-group.tsx
│   │   │   ├── toggle.tsx
│   │   │   └── tooltip.tsx
│   │   ├── AIChat.tsx
│   │   ├── AssistenteJuridico.tsx
│   │   ├── BuildPanel.tsx
│   │   ├── CampoLivre.tsx
│   │   ├── CodeEditor.tsx
│   │   ├── CombinarApps.tsx
│   │   ├── DatabasePanel.tsx
│   │   ├── DeployPanel.tsx
│   │   ├── DriveBackupPanel.tsx
│   │   ├── EditorLayout.tsx
│   │   ├── ElectronTerminal.tsx
│   │   ├── FileScanner.tsx
│   │   ├── FileTree.tsx
│   │   ├── GitHubPanel.tsx
│   │   ├── HTMLPlayground.tsx
│   │   ├── Manual.tsx
│   │   ├── PackageSearch.tsx
│   │   ├── Preview.tsx
│   │   ├── QuickPrompt.tsx
│   │   ├── RealTerminal.tsx
│   │   ├── SiteExtractor.tsx
│   │   ├── SKTerminal.tsx
│   │   ├── StreamTerminal.tsx
│   │   ├── SystemStatusPanel.tsx
│   │   ├── TemplateSelector.tsx
│   │   ├── Terminal.tsx
│   │   ├── VoiceCard.tsx
│   │   ├── VoiceMode.tsx
│   │   ├── WebContainerTerminal.tsx
│   │   └── XTermConnector.tsx
│   ├── hooks/
│   │   ├── use-mobile.tsx
│   │   └── use-toast.ts
│   ├── lib/
│   │   ├── ai-service.ts
│   │   ├── github-service.ts
│   │   ├── idb-storage.ts
│   │   ├── projects.ts
│   │   ├── store.ts
│   │   ├── templates.ts
│   │   ├── tts-service.ts
│   │   ├── utils.ts
│   │   ├── virtual-fs.ts
│   │   └── zip-service.ts
│   ├── App.tsx
│   ├── index.css
│   └── main.tsx
├── código.htlm
├── index.html
├── package.json
├── PLANO.md
├── pnpm-workspace.yaml
├── README-SK-EDITOR-V3.md
├── replit.md
├── replit.nix
├── server.cjs
├── SISTEMA.md
├── tsconfig.json
└── vite.config.ts
```

---

## ROTAS DA API DETECTADAS (30 endpoint(s))

```
GET    /api/items  (src/lib/templates.ts)
GET    /api/items/:id  (src/lib/templates.ts)
POST   /api/items  (src/lib/templates.ts)
GET    /api/health  (src/lib/templates.ts)
USE    /api/auth  (src/lib/templates.ts)
USE    /api/usuarios  (src/lib/templates.ts)
POST   /register  (src/lib/templates.ts)
POST   /login  (src/lib/templates.ts)
GET    /perfil  (src/lib/templates.ts)
GET    /api/provedores  (src/lib/templates.ts)
POST   /api/chat  (src/lib/templates.ts)
GET    /health  (src/lib/templates.ts)
POST   /auth/login  (src/lib/templates.ts)
POST   /auth/registro  (src/lib/templates.ts)
GET    /clientes  (src/lib/templates.ts)
GET    /clientes/:id  (src/lib/templates.ts)
POST   /clientes  (src/lib/templates.ts)
PUT    /clientes/:id  (src/lib/templates.ts)
GET    /processos  (src/lib/templates.ts)
GET    /processos/:id  (src/lib/templates.ts)
POST   /processos  (src/lib/templates.ts)
GET    /audiencias  (src/lib/templates.ts)
POST   /audiencias  (src/lib/templates.ts)
GET    /prazos/proximos  (src/lib/templates.ts)
GET    /dashboard  (src/lib/templates.ts)
GET    /api/registros  (src/lib/templates.ts)
GET    /api/registros/:id  (src/lib/templates.ts)
POST   /api/registros  (src/lib/templates.ts)
PUT    /api/registros/:id  (src/lib/templates.ts)
DELETE /api/registros/:id  (src/lib/templates.ts)
```

---

## SCRIPTS DISPONÍVEIS (package.json)

```bash
npm run dev           # vite --config vite.config.ts --host 0.0.0.0
npm run build         # vite build --config vite.config.ts
npm run serve         # vite preview --config vite.config.ts --host 0.0.0.0
npm run typecheck     # tsc -p tsconfig.json --noEmit
npm run build:zips    # node scripts/build-zips.mjs
npm run electron:build  # pnpm build && electron-builder --linux AppImage --win nsis --x64
npm run electron:build:linux  # pnpm build && electron-builder --linux AppImage --x64
npm run electron:build:win  # pnpm build && electron-builder --win nsis --x64
```

---

## VARIÁVEIS DE AMBIENTE NECESSÁRIAS

Crie o arquivo `.env` na raiz do projeto:

```env
PORT=seu_valor_aqui
ALLOWED_ORIGINS=seu_valor_aqui
JWT_SECRET=seu_valor_aqui
JWT_EXPIRES_IN=seu_valor_aqui
DATABASE_URL=seu_valor_aqui
GROQ_API_KEY=seu_valor_aqui
OPENAI_API_KEY=seu_valor_aqui
GEMINI_API_KEY=seu_valor_aqui
ANTHROPIC_API_KEY=seu_valor_aqui
XAI_API_KEY=seu_valor_aqui
OPENROUTER_API_KEY=seu_valor_aqui
PERPLEXITY_API_KEY=seu_valor_aqui
TELEGRAM_TOKEN=seu_valor_aqui
BASE_PATH=seu_valor_aqui
REPL_ID=seu_valor_aqui
```

---

## DEPENDÊNCIAS (80 pacotes)

### Produção (15)
- `@isomorphic-git/lightning-fs` ^4.6.2
- `@monaco-editor/react` ^4.7.0
- `@neondatabase/serverless` ^1.1.0
- `@webcontainer/api` ^1.6.4
- `@xterm/addon-fit` ^0.11.0
- `@xterm/addon-web-links` ^0.12.0
- `@xterm/xterm` ^6.0.0
- `express` ^5.2.1
- `file-saver` ^2.0.5
- `highlight.js` ^11.11.1
- `jszip` ^3.10.1
- `react-markdown` ^10.1.0
- `rehype-highlight` ^7.0.2
- `remark-gfm` ^4.0.1
- `sql.js` ^1.14.1

### Desenvolvimento (65)
- `@hookform/resolvers` ^3.10.0
- `@radix-ui/react-accordion` ^1.2.4
- `@radix-ui/react-alert-dialog` ^1.1.7
- `@radix-ui/react-aspect-ratio` ^1.1.3
- `@radix-ui/react-avatar` ^1.1.4
- `@radix-ui/react-checkbox` ^1.1.5
- `@radix-ui/react-collapsible` ^1.1.4
- `@radix-ui/react-context-menu` ^2.2.7
- `@radix-ui/react-dialog` ^1.1.7
- `@radix-ui/react-dropdown-menu` ^2.1.7
- `@radix-ui/react-hover-card` ^1.1.7
- `@radix-ui/react-label` ^2.1.3
- `@radix-ui/react-menubar` ^1.1.7
- `@radix-ui/react-navigation-menu` ^1.2.6
- `@radix-ui/react-popover` ^1.1.7
- `@radix-ui/react-progress` ^1.1.3
- `@radix-ui/react-radio-group` ^1.2.4
- `@radix-ui/react-scroll-area` ^1.2.4
- `@radix-ui/react-select` ^2.1.7
- `@radix-ui/react-separator` ^1.1.3
- `@radix-ui/react-slider` ^1.2.4
- `@radix-ui/react-slot` ^1.2.0
- `@radix-ui/react-switch` ^1.1.4
- `@radix-ui/react-tabs` ^1.1.4
- `@radix-ui/react-toast` ^1.2.7
- `@radix-ui/react-toggle` ^1.1.3
- `@radix-ui/react-toggle-group` ^1.1.3
- `@radix-ui/react-tooltip` ^1.2.0
- `@replit/vite-plugin-cartographer` catalog:
- `@replit/vite-plugin-dev-banner` catalog:
- `@replit/vite-plugin-runtime-error-modal` catalog:
- `@tailwindcss/typography` ^0.5.15
- `@tailwindcss/vite` catalog:
- `@tanstack/react-query` catalog:
- `@types/file-saver` ^2.0.7
- `@types/node` catalog:
- `@types/react` catalog:
- `@types/react-dom` catalog:
- `@vitejs/plugin-react` catalog:
- `class-variance-authority` catalog:
- `clsx` catalog:
- `cmdk` ^1.1.1
- `date-fns` ^3.6.0
- `electron` ^42.4.0
- `electron-builder` ^26.15.3
- `embla-carousel-react` ^8.6.0
- `framer-motion` catalog:
- `input-otp` ^1.4.2
- `lucide-react` catalog:
- `next-themes` ^0.4.6
- `react` catalog:
- `react-day-picker` ^9.11.1
- `react-dom` catalog:
- `react-hook-form` ^7.55.0
- `react-icons` ^5.4.0
- `react-resizable-panels` ^2.1.7
- `recharts` ^2.15.2
- `sonner` ^2.0.7
- `tailwind-merge` catalog:
- `tailwindcss` catalog:
- `tw-animate-css` ^1.4.0
- `vaul` ^1.1.2
- `vite` catalog:
- `wouter` ^3.3.5
- `zod` catalog:

---

## GUIA COMPLETO PARA RECRIAR DO ZERO

> Siga este passo a passo em qualquer máquina com Node.js instalado para recriar o projeto Meu App.

### Pré-requisitos

```bash
# Verificar Node.js 20+ instalado
node -v   # precisa ser v20 ou superior
npm -v    # precisa ser 10 ou superior
```

> Não tem Node.js? Baixe em: https://nodejs.org (escolha LTS)

---

### Passo 1 — Criar a estrutura do projeto

```bash
# React + Vite + TypeScript
npm create vite@latest meu-app -- --template react-ts
cd meu-app
```

---

### Passo 2 — Instalar dependências

```bash
# Dependências de produção
npm install @isomorphic-git/lightning-fs @monaco-editor/react @neondatabase/serverless @webcontainer/api @xterm/addon-fit @xterm/addon-web-links @xterm/xterm express file-saver highlight.js jszip react-markdown rehype-highlight remark-gfm sql.js

# Dependências de desenvolvimento
npm install --save-dev @hookform/resolvers @radix-ui/react-accordion @radix-ui/react-alert-dialog @radix-ui/react-aspect-ratio @radix-ui/react-avatar @radix-ui/react-checkbox @radix-ui/react-collapsible @radix-ui/react-context-menu @radix-ui/react-dialog @radix-ui/react-dropdown-menu @radix-ui/react-hover-card @radix-ui/react-label @radix-ui/react-menubar @radix-ui/react-navigation-menu @radix-ui/react-popover @radix-ui/react-progress @radix-ui/react-radio-group @radix-ui/react-scroll-area @radix-ui/react-select @radix-ui/react-separator @radix-ui/react-slider @radix-ui/react-slot @radix-ui/react-switch @radix-ui/react-tabs @radix-ui/react-toast @radix-ui/react-toggle @radix-ui/react-toggle-group @radix-ui/react-tooltip @replit/vite-plugin-cartographer @replit/vite-plugin-dev-banner @replit/vite-plugin-runtime-error-modal @tailwindcss/typography @tailwindcss/vite @tanstack/react-query @types/file-saver @types/node @types/react @types/react-dom @vitejs/plugin-react class-variance-authority clsx cmdk date-fns electron electron-builder embla-carousel-react framer-motion input-otp lucide-react next-themes react react-day-picker react-dom react-hook-form react-icons react-resizable-panels recharts sonner tailwind-merge tailwindcss tw-animate-css vaul vite wouter zod
```

---

### Passo 3 — Recriar os arquivos do projeto

> Importe o ZIP do projeto pelo SK Editor (ícone 📁 → Importar ZIP)
> ou copie os 115 arquivos manualmente:

```
PLANO.md
README-SK-EDITOR-V3.md
SISTEMA.md
código.htlm
electron/main.cjs
electron/preload.cjs
index.html
package.json
pnpm-workspace.yaml
public/manifest.webmanifest
replit.md
replit.nix
server.cjs
src/App.tsx
src/components/AIChat.tsx
src/components/AssistenteJuridico.tsx
src/components/BuildPanel.tsx
src/components/CampoLivre.tsx
src/components/CodeEditor.tsx
src/components/CombinarApps.tsx
src/components/DatabasePanel.tsx
src/components/DeployPanel.tsx
src/components/DriveBackupPanel.tsx
src/components/EditorLayout.tsx
src/components/ElectronTerminal.tsx
src/components/FileScanner.tsx
src/components/FileTree.tsx
src/components/GitHubPanel.tsx
src/components/HTMLPlayground.tsx
src/components/Manual.tsx
src/components/PackageSearch.tsx
src/components/Preview.tsx
src/components/QuickPrompt.tsx
src/components/RealTerminal.tsx
src/components/SKTerminal.tsx
src/components/SiteExtractor.tsx
src/components/StreamTerminal.tsx
src/components/SystemStatusPanel.tsx
src/components/TemplateSelector.tsx
src/components/Terminal.tsx
src/components/VoiceCard.tsx
src/components/VoiceMode.tsx
src/components/WebContainerTerminal.tsx
src/components/XTermConnector.tsx
src/components/ui/accordion.tsx
src/components/ui/alert-dialog.tsx
src/components/ui/alert.tsx
src/components/ui/aspect-ratio.tsx
src/components/ui/avatar.tsx
src/components/ui/badge.tsx
src/components/ui/breadcrumb.tsx
src/components/ui/button-group.tsx
src/components/ui/button.tsx
src/components/ui/calendar.tsx
src/components/ui/card.tsx
src/components/ui/carousel.tsx
src/components/ui/chart.tsx
src/components/ui/checkbox.tsx
src/components/ui/collapsible.tsx
src/components/ui/command.tsx
src/components/ui/context-menu.tsx
src/components/ui/dialog.tsx
src/components/ui/drawer.tsx
src/components/ui/dropdown-menu.tsx
src/components/ui/empty.tsx
src/components/ui/field.tsx
src/components/ui/form.tsx
src/components/ui/hover-card.tsx
src/components/ui/input-group.tsx
src/components/ui/input-otp.tsx
src/components/ui/input.tsx
src/components/ui/item.tsx
src/components/ui/kbd.tsx
src/components/ui/label.tsx
src/components/ui/menubar.tsx
src/components/ui/navigation-menu.tsx
src/components/ui/pagination.tsx
src/components/ui/popover.tsx
src/components/ui/progress.tsx
src/components/ui/radio-group.tsx
src/components/ui/resizable.tsx
src/components/ui/scroll-area.tsx
src/components/ui/select.tsx
src/components/ui/separator.tsx
src/components/ui/sheet.tsx
src/components/ui/sidebar.tsx
src/components/ui/skeleton.tsx
src/components/ui/slider.tsx
src/components/ui/sonner.tsx
src/components/ui/spinner.tsx
src/components/ui/switch.tsx
src/components/ui/table.tsx
src/components/ui/tabs.tsx
src/components/ui/textarea.tsx
src/components/ui/toast.tsx
src/components/ui/toaster.tsx
src/components/ui/toggle-group.tsx
src/components/ui/toggle.tsx
src/components/ui/tooltip.tsx
src/hooks/use-mobile.tsx
src/hooks/use-toast.ts
src/index.css
src/lib/ai-service.ts
src/lib/github-service.ts
src/lib/idb-storage.ts
src/lib/projects.ts
src/lib/store.ts
src/lib/templates.ts
src/lib/tts-service.ts
src/lib/utils.ts
src/lib/virtual-fs.ts
src/lib/zip-service.ts
src/main.tsx
tsconfig.json
vite.config.ts
```

---

### Passo 4 — Configurar variáveis de ambiente

```bash
# Crie o arquivo .env na raiz do projeto:
cat > .env << 'EOF'
PORT=seu_valor_aqui
ALLOWED_ORIGINS=seu_valor_aqui
JWT_SECRET=seu_valor_aqui
JWT_EXPIRES_IN=seu_valor_aqui
DATABASE_URL=seu_valor_aqui
GROQ_API_KEY=seu_valor_aqui
OPENAI_API_KEY=seu_valor_aqui
GEMINI_API_KEY=seu_valor_aqui
ANTHROPIC_API_KEY=seu_valor_aqui
XAI_API_KEY=seu_valor_aqui
OPENROUTER_API_KEY=seu_valor_aqui
PERPLEXITY_API_KEY=seu_valor_aqui
TELEGRAM_TOKEN=seu_valor_aqui
BASE_PATH=seu_valor_aqui
REPL_ID=seu_valor_aqui
EOF
```

> ⚠️ NUNCA versione o .env no GitHub! Adicione ao .gitignore.

---

### Passo 5 — Rodar o projeto

```bash
npm run dev
# O projeto estará disponível em http://localhost:5173
```

---

### Passo extra — Configurar banco de dados

> Configure a variável DATABASE_URL no .env com sua connection string PostgreSQL.

---


## CONTEXTO PARA IA

> Copie e cole este bloco para continuar o projeto em qualquer IA (ChatGPT, Gemini, Claude...):

```
Projeto: Meu App
Tipo: Full-Stack (React + Express)
Stack: React + Vite, TypeScript, Tailwind CSS, Node.js + Express, PostgreSQL
Arquivos: 115 | Linhas: ~37.428
Rotas API detectadas: 30
GET    /api/items  (src/lib/templates.ts)
GET    /api/items/:id  (src/lib/templates.ts)
POST   /api/items  (src/lib/templates.ts)
GET    /api/health  (src/lib/templates.ts)
USE    /api/auth  (src/lib/templates.ts)
USE    /api/usuarios  (src/lib/templates.ts)
POST   /register  (src/lib/templates.ts)
POST   /login  (src/lib/templates.ts)
GET    /perfil  (src/lib/templates.ts)
GET    /api/provedores  (src/lib/templates.ts)
POST   /api/chat  (src/lib/templates.ts)
GET    /health  (src/lib/templates.ts)
POST   /auth/login  (src/lib/templates.ts)
POST   /auth/registro  (src/lib/templates.ts)
GET    /clientes  (src/lib/templates.ts)
GET    /clientes/:id  (src/lib/templates.ts)
POST   /clientes  (src/lib/templates.ts)
PUT    /clientes/:id  (src/lib/templates.ts)
GET    /processos  (src/lib/templates.ts)
GET    /processos/:id  (src/lib/templates.ts)
POST   /processos  (src/lib/templates.ts)
GET    /audiencias  (src/lib/templates.ts)
POST   /audiencias  (src/lib/templates.ts)
GET    /prazos/proximos  (src/lib/templates.ts)
GET    /dashboard  (src/lib/templates.ts)
GET    /api/registros  (src/lib/templates.ts)
GET    /api/registros/:id  (src/lib/templates.ts)
POST   /api/registros  (src/lib/templates.ts)
PUT    /api/registros/:id  (src/lib/templates.ts)
DELETE /api/registros/:id  (src/lib/templates.ts)
Variáveis de ambiente: PORT, ALLOWED_ORIGINS, JWT_SECRET, JWT_EXPIRES_IN, DATABASE_URL, GROQ_API_KEY, OPENAI_API_KEY, GEMINI_API_KEY, ANTHROPIC_API_KEY, XAI_API_KEY, OPENROUTER_API_KEY, PERPLEXITY_API_KEY, TELEGRAM_TOKEN, BASE_PATH, REPL_ID

Estrutura completa do projeto:
PLANO.md
README-SK-EDITOR-V3.md
SISTEMA.md
código.htlm
electron/main.cjs
electron/preload.cjs
index.html
package.json
pnpm-workspace.yaml
public/manifest.webmanifest
replit.md
replit.nix
server.cjs
src/App.tsx
src/components/AIChat.tsx
src/components/AssistenteJuridico.tsx
src/components/BuildPanel.tsx
src/components/CampoLivre.tsx
src/components/CodeEditor.tsx
src/components/CombinarApps.tsx
src/components/DatabasePanel.tsx
src/components/DeployPanel.tsx
src/components/DriveBackupPanel.tsx
src/components/EditorLayout.tsx
src/components/ElectronTerminal.tsx
src/components/FileScanner.tsx
src/components/FileTree.tsx
src/components/GitHubPanel.tsx
src/components/HTMLPlayground.tsx
src/components/Manual.tsx
src/components/PackageSearch.tsx
src/components/Preview.tsx
src/components/QuickPrompt.tsx
src/components/RealTerminal.tsx
src/components/SKTerminal.tsx
src/components/SiteExtractor.tsx
src/components/StreamTerminal.tsx
src/components/SystemStatusPanel.tsx
src/components/TemplateSelector.tsx
src/components/Terminal.tsx
src/components/VoiceCard.tsx
src/components/VoiceMode.tsx
src/components/WebContainerTerminal.tsx
src/components/XTermConnector.tsx
src/components/ui/accordion.tsx
src/components/ui/alert-dialog.tsx
src/components/ui/alert.tsx
src/components/ui/aspect-ratio.tsx
src/components/ui/avatar.tsx
src/components/ui/badge.tsx
src/components/ui/breadcrumb.tsx
src/components/ui/button-group.tsx
src/components/ui/button.tsx
src/components/ui/calendar.tsx
src/components/ui/card.tsx
src/components/ui/carousel.tsx
src/components/ui/chart.tsx
src/components/ui/checkbox.tsx
src/components/ui/collapsible.tsx
src/components/ui/command.tsx
src/components/ui/context-menu.tsx
src/components/ui/dialog.tsx
src/components/ui/drawer.tsx
src/components/ui/dropdown-menu.tsx
src/components/ui/empty.tsx
src/components/ui/field.tsx
src/components/ui/form.tsx
src/components/ui/hover-card.tsx
src/components/ui/input-group.tsx
src/components/ui/input-otp.tsx
src/components/ui/input.tsx
src/components/ui/item.tsx
src/components/ui/kbd.tsx
src/components/ui/label.tsx
src/components/ui/menubar.tsx
src/components/ui/navigation-menu.tsx
src/components/ui/pagination.tsx
src/components/ui/popover.tsx
src/components/ui/progress.tsx
src/components/ui/radio-group.tsx
src/components/ui/resizable.tsx
src/components/ui/scroll-area.tsx
src/components/ui/select.tsx
src/components/ui/separator.tsx
src/components/ui/sheet.tsx
src/components/ui/sidebar.tsx
src/components/ui/skeleton.tsx
src/components/ui/slider.tsx
src/components/ui/sonner.tsx
src/components/ui/spinner.tsx
src/components/ui/switch.tsx
src/components/ui/table.tsx
src/components/ui/tabs.tsx
src/components/ui/textarea.tsx
src/components/ui/toast.tsx
src/components/ui/toaster.tsx
src/components/ui/toggle-group.tsx
src/components/ui/toggle.tsx
src/components/ui/tooltip.tsx
src/hooks/use-mobile.tsx
src/hooks/use-toast.ts
src/index.css
src/lib/ai-service.ts
src/lib/github-service.ts
src/lib/idb-storage.ts
src/lib/projects.ts
src/lib/store.ts
src/lib/templates.ts
src/lib/tts-service.ts
src/lib/utils.ts
src/lib/virtual-fs.ts
src/lib/zip-service.ts
src/main.tsx
tsconfig.json
vite.config.ts
```

---

## CHECKLIST DE RECRIAÇÃO

- [ ] Node.js 20+ instalado
- [ ] Projeto criado (`npm create vite` ou similar)
- [ ] Dependências instaladas (`npm install`)
- [ ] Arquivo .env configurado com as variáveis necessárias
- [ ] Banco de dados PostgreSQL configurado e acessível

- [ ] Projeto rodando localmente sem erros
- [ ] Build de produção testado (`npm run build`)
- [ ] Deploy/publicação configurado (Netlify, Vercel, Replit...)

---

## FASES DE PUBLICAÇÃO

### Web (mais fácil — recomendado primeiro)
1. Baixe o ZIP **Netlify** em Build & Deploy
2. Extraia → `npm install && npm run build`
3. Arraste a pasta `dist/` para https://app.netlify.com/drop
4. ✅ URL pública em segundos!

### PWA no celular (sem APK)
1. Publique na web (passo acima)
2. Acesse no Chrome do Android → Menu → "Adicionar à tela inicial"
3. ✅ App instalado sem loja!

### APK Android
1. Baixe o ZIP **Capacitor** ou **EAS** em Build & Deploy
2. Siga as instruções do README dentro do ZIP

### Executável Desktop (Windows/Linux)
1. Baixe **MaikonJuridicoPro-windows.zip** ou **MaikonJuridicoPro-linux.AppImage**
   na seção "Executável Desktop — Electron"
2. Extraia e execute — roda offline, sem instalar nada

---

*Plano gerado automaticamente pelo SK Code Editor — 14/07/2026, 17:54:53*
