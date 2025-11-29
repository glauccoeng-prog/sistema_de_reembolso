# 🧾 Sistema de Reembolso (Refund System)

Um sistema completo e responsivo para gerenciamento de solicitações de reembolso corporativo. Desenvolvido com foco em performance, usabilidade, boas práticas de engenharia de software e pronto para instalação como PWA (Progressive Web App).

![Status do Projeto](https://img.shields.io/badge/Status-Concluído-green)
![CI/CD](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-2088FF)
![React](https://img.shields.io/badge/React-18.2-blue)
![TypeScript](https://img.shields.io/badge/TypeScript-5-blue)
![Vite](https://img.shields.io/badge/Vite-6.0.4-purple)
![PWA](https://img.shields.io/badge/PWA-Ready-orange)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.4.16-38B2AC)
![Vitest](https://img.shields.io/badge/Vitest-3.2.4-6E9F18)
![Tests](https://img.shields.io/badge/Tests-52%20passing-brightgreen)
![ESLint](https://img.shields.io/badge/ESLint-9.39.1-4B32C3)
![Prettier](https://img.shields.io/badge/Prettier-3.7.2-F7B93E)

---

## 📋 Índice

- [Visão Geral](#-visão-geral)
- [Demo](#-demo)
- [Tecnologias](#-tecnologias-e-ferramentas)
- [Funcionalidades](#-funcionalidades-implementadas)
- [Arquitetura Completa](#-arquitetura-completa-do-projeto)
- [Estrutura de Pastas](#-estrutura-de-pastas-detalhada)
- [Componentes](#-componentes)
- [Hooks Customizados](#-hooks-customizados)
- [Serviços](#-serviços)
- [Testes](#-testes)
- [ESLint e Prettier](#-eslint-e-prettier)
- [CI/CD](#-cicd-com-github-actions)
- [PWA](#-progressive-web-app-pwa)
- [SEO](#-seo-e-meta-tags)
- [Design System](#-design-system)
- [Instalação](#-instalação-e-execução)
- [Scripts](#-scripts-disponíveis)
- [Decisões Técnicas](#-decisões-técnicas-importantes)
- [Licença](#-licença)

---

## 🎯 Visão Geral

Este projeto simula um ambiente real de controle de despesas corporativas, permitindo que colaboradores enviem solicitações de reembolso com comprovantes, e que administradores visualizem, filtrem e gerenciem essas solicitações.

### Principais Características:

- ✅ **CRUD Completo** de reembolsos
- ✅ **PWA Instalável** em dispositivos móveis e desktop
- ✅ **Busca com Debounce** para otimização de performance
- ✅ **Upload de Arquivos** com validação (JPG, PNG, PDF até 5MB)
- ✅ **Visualizador de Comprovantes** com suporte a imagens e PDFs
- ✅ **Persistência Local** via LocalStorage (simula backend)
- ✅ **100% Responsivo** (Mobile First)
- ✅ **Animações Fluidas** com Framer Motion
- ✅ **SEO Otimizado** com meta tags dinâmicas
- ✅ **Acessibilidade** com componentes Radix UI
- ✅ **Testes Automatizados** com Vitest + Testing Library

---

## 🌐 Site

**Produção:** []()

---

## 🚀 Tecnologias e Ferramentas

### Core
| Tecnologia | Versão | Descrição |
|------------|--------|-----------|
| [React](https://react.dev/) | 18.2.0 | Biblioteca para construção de interfaces |
| [TypeScript](https://www.typescriptlang.org/) | 5.x | Tipagem estática e segurança de código |
| [Vite](https://vitejs.dev/) | 6.0.4 | Build tool ultra-rápida |

### Gerenciamento de Estado e Dados
| Tecnologia | Versão | Descrição |
|------------|--------|-----------|
| [TanStack Query](https://tanstack.com/query/latest) | 5.59.0 | Gerenciamento de estado assíncrono e cache |
| [React Hook Form](https://react-hook-form.com/) | 7.53.0 | Gerenciamento de formulários performático |
| [React Router DOM](https://reactrouter.com/) | 6.8.1 | Roteamento declarativo para SPA |

### Estilização e UI
| Tecnologia | Versão | Descrição |
|------------|--------|-----------|
| [Tailwind CSS](https://tailwindcss.com/) | 3.4.16 | Framework CSS utility-first |
| [Radix UI](https://www.radix-ui.com/) | 1.x | Primitivos acessíveis (Dialog, Select, Toast, etc.) |
| [Framer Motion](https://www.framer.com/motion/) | latest | Animações fluidas e interativas |
| [Lucide React](https://lucide.dev/) | 0.453.0 | Biblioteca de ícones |
| [CVA](https://cva.style/) | 0.7.0 | Variantes de componentes |

### PWA e SEO
| Tecnologia | Versão | Descrição |
|------------|--------|-----------|
| [vite-plugin-pwa](https://vite-pwa-org.netlify.app/) | latest | Geração automática de Service Worker |
| [react-helmet-async](https://github.com/staylor/react-helmet-async) | latest | Meta tags dinâmicas |
| [Workbox](https://developer.chrome.com/docs/workbox/) | - | Caching avançado |

### Testes
| Tecnologia | Versão | Descrição |
|------------|--------|-----------|
| [Vitest](https://vitest.dev/) | 3.2.4 | Framework de testes para Vite |
| [Testing Library](https://testing-library.com/) | 16.3.0 | Utilitários para testar React |
| [jest-dom](https://github.com/testing-library/jest-dom) | 6.9.1 | Matchers para asserções de DOM |
| [jsdom](https://github.com/jsdom/jsdom) | 27.2.0 | Ambiente de navegador simulado |

### Qualidade de Código
| Tecnologia | Versão | Descrição |
|------------|--------|-----------|
| [ESLint](https://eslint.org/) | 9.39.1 | Linter para JavaScript/TypeScript |
| [Prettier](https://prettier.io/) | 3.7.2 | Formatador de código automático |
| [typescript-eslint](https://typescript-eslint.io/) | 8.48.0 | Regras ESLint para TypeScript |
| [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) | 7.37.5 | Regras ESLint para React |
| [eslint-plugin-react-hooks](https://www.npmjs.com/package/eslint-plugin-react-hooks) | 7.0.1 | Regras para React Hooks |

---

## ✨ Funcionalidades Implementadas

### 1. 📝 Gestão de Reembolsos (CRUD)
- **Listagem**: Visualização paginada (6 itens/página) com loading states
- **Criação**: Modal com formulário validado + upload de comprovante
- **Leitura**: Página de detalhes com todas as informações
- **Exclusão**: Confirmação de segurança com modal

### 2. 🔍 Busca Inteligente
- Filtro em tempo real por nome do solicitante
- **Debounce de 500ms** para evitar sobrecarga
- Reset automático de paginação ao buscar

### 3. 📁 Upload e Visualização de Arquivos
- **Drag & Drop** inteligente
- Suporte: JPG, PNG, PDF (máx. 5MB)
- Validação de tipo e tamanho
- **Visualizador modal** para imagens e PDFs
- **Download seguro** via Blob URLs

### 4. 📱 PWA (Progressive Web App)
- Instalável em celulares e desktops
- **Prompt de instalação** customizado
- Funciona offline (assets cacheados)
- Ícones otimizados (192x192, 512x512)

### 5. 🎨 UX/UI
- **Design System** consistente
- **Toasts** para feedback (sucesso, erro, info)
- **Loading spinners** durante operações
- **Animações em cascata** na listagem
- Estados de **hover, focus e active**

### 6. 📊 SEO
- Meta tags dinâmicas por página
- Open Graph para compartilhamento social
- JSON-LD para dados estruturados
- Sitemap e robots.txt

---

## 🏗️ Arquitetura Completa do Projeto

O projeto segue uma arquitetura híbrida baseada em **Feature-Sliced Design** e **Shared Resources**, facilitando escalabilidade e manutenção.

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                              ARQUITETURA                                     │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                              │
│  ┌──────────────┐    ┌──────────────┐    ┌──────────────┐                   │
│  │   SCREENS    │───▶│  FEATURES    │───▶│   SERVICES   │                   │
│  │   (Páginas)  │    │  (Domínio)   │    │ (API/Storage)│                   │
│  └──────────────┘    └──────────────┘    └──────────────┘                   │
│         │                   │                    │                          │
│         ▼                   ▼                    ▼                          │
│  ┌──────────────────────────────────────────────────────────────────┐       │
│  │                        SHARED                                     │       │
│  │  ┌────────────┐ ┌────────────┐ ┌────────────┐ ┌────────────┐    │       │
│  │  │ Components │ │   Hooks    │ │   Utils    │ │ Constants  │    │       │
│  │  └────────────┘ └────────────┘ └────────────┘ └────────────┘    │       │
│  └──────────────────────────────────────────────────────────────────┘       │
│         │                                                                    │
│         ▼                                                                    │
│  ┌──────────────────────────────────────────────────────────────────┐       │
│  │                     COMPONENTS (UI)                               │       │
│  │  Button │ Input │ Card │ Dialog │ Select │ Toast │ Avatar        │       │
│  └──────────────────────────────────────────────────────────────────┘       │
│                                                                              │
└─────────────────────────────────────────────────────────────────────────────┘
```

### Fluxo de Dados

```
┌─────────────┐      ┌─────────────┐      ┌─────────────┐      ┌─────────────┐
│   Usuário   │─────▶│    Screen   │─────▶│    Hook     │─────▶│   Service   │
│  (Ação)     │      │ (Componente)│      │(useReimb...)│      │(reimbServ.) │
└─────────────┘      └─────────────┘      └─────────────┘      └─────────────┘
                            ▲                    │                    │
                            │                    ▼                    ▼
                            │              ┌─────────────┐      ┌─────────────┐
                            └──────────────│ React Query │◀─────│ localStorage│
                                           │   (Cache)   │      │  (Storage)  │
                                           └─────────────┘      └─────────────┘
```

---

## 📂 Estrutura de Pastas Detalhada

```
sistema_de_reembolso/
├── 📄 index.html                    # Entry point HTML
├── 📄 package.json                  # Dependências e scripts
├── 📄 vite.config.ts                # Configuração do Vite + PWA
├── 📄 tailwind.config.js            # Configuração do Tailwind CSS
├── 📄 tailwind.css                  # CSS global com variáveis
├── 📄 tsconfig.json                 # Configuração TypeScript
├── 📄 tsconfig.app.json             # Config TS para aplicação
├── 📄 tsconfig.node.json            # Config TS para Node
├── 📄 vitest.config.ts              # Configuração do Vitest
├── 📄 .gitignore                    # Arquivos ignorados pelo Git
│
├── 📁 static/                       # Assets públicos (publicDir)
│   ├── 🖼️ favicon.svg              # Favicon SVG
│   ├── 🖼️ pwa-192x192.png          # Ícone PWA 192x192
│   ├── 🖼️ pwa-512x512.png          # Ícone PWA 512x512
│   ├── 🖼️ apple-touch-icon.png     # Ícone Apple Touch
│   ├── 📄 robots.txt               # Instruções para crawlers
│   ├── 📄 sitemap.xml              # Mapa do site para SEO
│   │
│   └── 📁 assets/
│       ├── 🖼️ logo.svg             # Logo principal
│       └── 📁 icons/
│           ├── 🖼️ refund.svg       # Texto "refund" do logo
│           ├── 🖼️ success.svg      # Ícone de sucesso
│           ├── 🖼️ food.svg         # Categoria: Alimentação
│           ├── 🖼️ hosting.svg      # Categoria: Hospedagem
│           ├── 🖼️ transport.svg    # Categoria: Transporte
│           ├── 🖼️ service.svg      # Categoria: Serviços
│           └── 🖼️ other.svg        # Categoria: Outros
│
├── 📁 dev-dist/                     # Build PWA desenvolvimento
│   ├── registerSW.js
│   ├── sw.js
│   └── workbox-*.js
│
└── 📁 src/                          # Código fonte
    │
    ├── 📄 index.tsx                 # Entry point React
    ├── 📄 App.tsx                   # Componente raiz + Rotas
    │
    ├── 📁 test/                     # Testes automatizados
    │   ├── 📄 setup.ts              # Configuração global dos testes
    │   ├── 📄 test-utils.tsx        # Render com providers
    │   ├── 📄 index.ts              # Documentação
    │   │
    │   ├── 📁 components/           # Testes de componentes
    │   │   ├── 📄 Button.test.tsx   # 8 testes
    │   │   └── 📄 Input.test.tsx    # 8 testes
    │   │
    │   ├── 📁 hooks/                # Testes de hooks
    │   │   └── 📄 useDebounce.test.ts  # 4 testes
    │   │
    │   ├── 📁 services/             # Testes de serviços
    │   │   └── 📄 reimbursement.service.test.ts  # 8 testes
    │   │
    │   └── 📁 utils/                # Testes de utilitários
    │       ├── 📄 file.test.ts      # 12 testes
    │       └── 📄 format.test.ts    # 12 testes
    │
    ├── 📁 components/               # Componentes globais
    │   ├── 📄 PWAInstallPrompt.tsx  # Prompt instalação PWA
    │   ├── 📄 SEO.tsx               # Meta tags dinâmicas
    │   │
    │   ├── 📁 Footer/
    │   │   ├── 📄 Footer.tsx        # Rodapé com links sociais
    │   │   └── 📄 index.ts          # Export barrel
    │   │
    │   └── 📁 ui/                   # Design System (Shadcn-like)
    │       ├── 📄 avatar.tsx        # Componente Avatar
    │       ├── 📄 button.tsx        # Componente Button
    │       ├── 📄 card.tsx          # Componente Card
    │       ├── 📄 dialog.tsx        # Componente Dialog/Modal
    │       ├── 📄 input.tsx         # Componente Input
    │       ├── 📄 label.tsx         # Componente Label
    │       ├── 📄 select.tsx        # Componente Select
    │       ├── 📄 toast.tsx         # Componente Toast
    │       └── 📄 toaster.tsx       # Container de Toasts
    │
    ├── 📁 contexts/
    │   └── 📄 QueryProvider.tsx     # Provider React Query
    │
    ├── 📁 features/                 # Módulos por domínio
    │   └── 📁 reimbursements/
    │       │
    │       ├── 📁 components/
    │       │   └── 📁 ReimbursementList/
    │       │       ├── 📄 index.ts
    │       │       ├── 📄 ReimbursementList.tsx
    │       │       └── 📄 ReimbursementListItem.tsx
    │       │
    │       ├── 📁 hooks/
    │       │   ├── 📄 index.ts
    │       │   └── 📄 useReimbursements.ts  # CRUD hooks
    │       │
    │       └── 📁 services/
    │           ├── 📄 index.ts
    │           ├── 📄 reimbursement.service.ts  # API simulada
    │           └── 📄 mock-data.service.ts      # Dados mockados
    │
    ├── 📁 hooks/
    │   └── 📄 use-toast.ts          # Hook do Toast
    │
    ├── 📁 lib/
    │   └── 📄 utils.ts              # Utilitário cn() para classes
    │
    ├── 📁 screens/                  # Páginas da aplicação
    │   │
    │   ├── 📁 ListaDeReembolsos/    # Tela principal (/)
    │   │   ├── 📄 index.ts
    │   │   ├── 📄 ListaDeReembolsos.tsx
    │   │   │
    │   │   ├── 📁 components/
    │   │   │   └── 📄 CreateReimbursementModal.tsx
    │   │   │
    │   │   └── 📁 sections/
    │   │       ├── 📁 HeaderSection/
    │   │       │   ├── 📄 index.ts
    │   │       │   └── 📄 HeaderSection.tsx
    │   │       │
    │   │       └── 📁 RequestListSection/
    │   │           ├── 📄 index.ts
    │   │           └── 📄 RequestListSection.tsx
    │   │
    │   ├── 📁 DetalheDeReembolso/   # Detalhes (/detalhe-de-reembolso/:id)
    │   │   ├── 📄 index.ts
    │   │   └── 📄 DetalheDeReembolso.tsx
    │   │
    │   └── 📁 SolicitaoEnviada/     # Sucesso (/solicitacao-enviada)
    │       ├── 📄 index.ts
    │       └── 📄 SolicitaoEnviada.tsx
    │
    └── 📁 shared/                   # Recursos compartilhados
        │
        ├── 📁 components/
        │   ├── 📁 Motion/
        │   │   └── 📄 index.tsx     # Componentes de animação
        │   │
        │   └── 📁 ReceiptViewer/
        │       ├── 📄 index.ts
        │       └── 📄 ReceiptViewer.tsx  # Visualizador de arquivos
        │
        ├── 📁 constants/
        │   ├── 📄 index.ts
        │   ├── 📄 categories.ts     # Categorias e ícones
        │   └── 📄 storage.ts        # Chaves localStorage + validação
        │
        ├── 📁 hooks/
        │   ├── 📄 index.ts
        │   └── 📄 useDebounce.ts    # Hook de debounce
        │
        ├── 📁 types/
        │   └── 📄 index.ts          # Interfaces TypeScript
        │
        └── 📁 utils/
            ├── 📄 index.ts
            ├── 📄 file.ts           # Funções de arquivo
            └── 📄 format.ts         # Formatadores
```

---

## 🧩 Componentes

### Componentes UI (Design System)

| Componente | Arquivo | Descrição |
|------------|---------|-----------|
| `Button` | `ui/button.tsx` | Botões com variantes (default, link, ghost, icon) |
| `Input` | `ui/input.tsx` | Campo de entrada estilizado |
| `Card` | `ui/card.tsx` | Container com header, content, footer |
| `Dialog` | `ui/dialog.tsx` | Modal acessível (Radix UI) |
| `Select` | `ui/select.tsx` | Dropdown acessível (Radix UI) |
| `Toast` | `ui/toast.tsx` | Notificações temporárias |
| `Avatar` | `ui/avatar.tsx` | Avatar com fallback |
| `Label` | `ui/label.tsx` | Label para formulários |

### Componentes de Animação

| Componente | Arquivo | Descrição |
|------------|---------|-----------|
| `FadeIn` | `Motion/index.tsx` | Fade in + slide up |
| `ScaleOnTap` | `Motion/index.tsx` | Efeito de pressão |
| `StaggerContainer` | `Motion/index.tsx` | Container para animação em cascata |
| `StaggerItem` | `Motion/index.tsx` | Item individual da cascata |

### Componentes Globais

| Componente | Arquivo | Descrição |
|------------|---------|-----------|
| `Footer` | `Footer/Footer.tsx` | Rodapé com copyright e redes sociais |
| `SEO` | `SEO.tsx` | Meta tags dinâmicas via Helmet |
| `PWAInstallPrompt` | `PWAInstallPrompt.tsx` | Prompt flutuante para instalar PWA |
| `ReceiptViewer` | `ReceiptViewer/ReceiptViewer.tsx` | Modal para visualizar/baixar comprovantes |

---

## 🪝 Hooks Customizados

### `useReimbursements`
```typescript
// Busca lista paginada de reembolsos
const { data, isLoading, error } = useReimbursements(page, limit, search);
```

### `useReimbursement`
```typescript
// Busca um reembolso específico por ID
const { data: reimbursement, isLoading } = useReimbursement(id);
```

### `useCreateReimbursement`
```typescript
// Mutation para criar reembolso
const createMutation = useCreateReimbursement();
createMutation.mutate(data, { onSuccess, onError });
```

### `useDeleteReimbursement`
```typescript
// Mutation para excluir reembolso
const deleteMutation = useDeleteReimbursement();
deleteMutation.mutate(id, { onSuccess, onError });
```

### `useDebounce`
```typescript
// Atrasa atualização de valor
const debouncedValue = useDebounce(value, 500);
```

### `useToast`
```typescript
// Sistema de notificações
const { toast } = useToast();
toast({ title: "Sucesso!", variant: "success" });
```

---

## ⚙️ Serviços

### `reimbursementService`

API simulada com persistência no localStorage:

```typescript
// Buscar todos (paginado)
reimbursementService.getAll(page, limit, search)

// Buscar por ID
reimbursementService.getById(id)

// Criar
reimbursementService.create(data)

// Excluir
reimbursementService.delete(id)
```

**Características:**
- Delay artificial (200-500ms) para simular latência
- Inicialização automática com dados mockados
- Paginação server-side simulada
- Filtro por nome

### `mockDataService`

Gera dados de exemplo para desenvolvimento:

```typescript
const mockData = await mockDataService.generateMockData();
// Retorna 6 reembolsos com PDFs mockados
```

---

## 🧪 Testes

O projeto possui uma suíte completa de testes automatizados usando **Vitest** e **Testing Library**.

### Configuração

#### `vitest.config.ts`
```typescript
export default defineConfig({
  plugins: [react()],
  test: {
    environment: "jsdom",
    setupFiles: ["./src/test/setup.ts"],
    globals: true,
    include: ["src/**/*.{test,spec}.{js,ts,jsx,tsx}"],
    coverage: {
      provider: "v8",
      reporter: ["text", "json", "html"],
    },
  },
});
```

### Estrutura de Testes

```
src/test/
├── setup.ts              # Configuração global (mocks, cleanup)
├── test-utils.tsx        # Render customizado com providers
├── index.ts              # Documentação da estrutura
│
├── components/           # Testes de componentes UI
│   ├── Button.test.tsx   # 8 testes
│   └── Input.test.tsx    # 8 testes
│
├── hooks/                # Testes de hooks customizados
│   └── useDebounce.test.ts  # 4 testes
│
├── services/             # Testes de serviços
│   └── reimbursement.service.test.ts  # 8 testes
│
└── utils/                # Testes de funções utilitárias
    ├── file.test.ts      # 12 testes
    └── format.test.ts    # 12 testes
```

### Scripts de Teste

| Script | Comando | Descrição |
|--------|---------|-----------|
| `npm run test` | `vitest` | Modo watch (interativo) |
| `npm run test:run` | `vitest run` | Executa uma vez |
| `npm run test:coverage` | `vitest run --coverage` | Com relatório de cobertura |
| `npm run test:ui` | `vitest --ui` | Interface visual do Vitest |

### Resultado dos Testes

```
✓ src/test/utils/file.test.ts (12 tests)
✓ src/test/utils/format.test.ts (12 tests)
✓ src/test/hooks/useDebounce.test.ts (4 tests)
✓ src/test/components/Input.test.tsx (8 tests)
✓ src/test/components/Button.test.tsx (8 tests)
✓ src/test/services/reimbursement.service.test.ts (8 tests)

Test Files  6 passed (6)
     Tests  52 passed (52)
```

### Testes por Categoria

#### Componentes (`Button`, `Input`)
- Renderização correta
- Eventos de click
- Estados (disabled, readonly)
- Variantes e tamanhos
- Classes customizadas
- Focus handling

#### Hooks (`useDebounce`)
- Valor inicial retornado imediatamente
- Atualização após delay
- Cancelamento de atualizações anteriores
- Delay padrão de 500ms

#### Serviços (`reimbursementService`)
- Listagem paginada
- Filtro por nome
- Busca por ID
- Criação de reembolso
- Exclusão de reembolso

#### Utilitários (`format`, `file`)
- Formatação de moeda (BRL)
- Parse de valores monetários
- Formatação de datas
- Validação de tipos de arquivo
- Validação de tamanho de arquivo
- Conversão para Data URL

### Render Customizado

O arquivo `test-utils.tsx` fornece um render que envolve componentes com todos os providers necessários:

```typescript
import { render } from "../test/test-utils";

// Automaticamente envolve com:
// - QueryClientProvider (React Query)
// - BrowserRouter (React Router)
// - HelmetProvider (SEO)
render(<MyComponent />);
```

### Mocks Configurados (`setup.ts`)

- `matchMedia` - Componentes responsivos
- `ResizeObserver` - Componentes Radix UI
- `IntersectionObserver` - Lazy loading
- `localStorage` - Persistência
- `URL.createObjectURL` - Upload de arquivos

---

## 🔧 ESLint e Prettier

O projeto utiliza **ESLint** para análise estática de código e **Prettier** para formatação automática.

### Arquivos de Configuração

```
sistema_de_reembolso/
├── eslint.config.js     # Configuração do ESLint (flat config)
├── .prettierrc          # Configuração do Prettier
├── .prettierignore      # Arquivos ignorados pelo Prettier
└── .vscode/
    ├── settings.json    # Configurações do VS Code
    └── extensions.json  # Extensões recomendadas
```

### Configuração ESLint

O projeto usa o novo formato **flat config** do ESLint 9:

```javascript
// eslint.config.js
export default tseslint.config({
  extends: [
    js.configs.recommended,
    ...tseslint.configs.recommended,
    eslintConfigPrettier,
  ],
  plugins: {
    react,
    "react-hooks": reactHooks,
    "react-refresh": reactRefresh,
    prettier,
  },
  rules: {
    // React
    "react/prop-types": "off",
    "react/react-in-jsx-scope": "off",
    
    // TypeScript
    "@typescript-eslint/no-unused-vars": "warn",
    "@typescript-eslint/no-explicit-any": "warn",
    
    // Prettier integrado
    "prettier/prettier": "error",
    
    // Boas práticas
    "no-console": ["warn", { allow: ["warn", "error"] }],
    "prefer-const": "error",
    eqeqeq: ["error", "always"],
  },
});
```

### Configuração Prettier

```json
// .prettierrc
{
  "semi": true,
  "singleQuote": false,
  "tabWidth": 2,
  "trailingComma": "es5",
  "printWidth": 80,
  "useTabs": false,
  "bracketSpacing": true,
  "arrowParens": "always",
  "endOfLine": "auto"
}
```

### Scripts Disponíveis

| Script | Comando | Descrição |
|--------|---------|-----------|
| `npm run lint` | `eslint .` | Verifica erros de lint |
| `npm run lint:fix` | `eslint . --fix` | Corrige erros automaticamente |
| `npm run format` | `prettier --write` | Formata todos os arquivos |
| `npm run format:check` | `prettier --check` | Verifica formatação |

### Integração com VS Code

As configurações em `.vscode/settings.json` habilitam:

- ✅ **Format on Save** - Formata automaticamente ao salvar
- ✅ **ESLint Auto Fix** - Corrige problemas de lint ao salvar
- ✅ **Prettier como formatter padrão** - Para TS, TSX, JS, JSON

### Extensões Recomendadas

```json
// .vscode/extensions.json
{
  "recommendations": [
    "esbenp.prettier-vscode",
    "dbaeumer.vscode-eslint",
    "bradlc.vscode-tailwindcss"
  ]
}
```

### Executar Verificações

```bash
# Verificar lint (erros e warnings)
npm run lint

# Corrigir problemas automaticamente
npm run lint:fix

# Verificar formatação
npm run format:check

# Formatar todos os arquivos
npm run format
```

---

## 🔄 CI/CD com GitHub Actions

O projeto possui pipelines automatizados de integração e entrega contínua usando **GitHub Actions**.

### Workflows Configurados

```
.github/
├── workflows/
│   ├── ci.yml           # Pipeline principal (CI/CD)
│   └── pr-check.yml     # Validação de Pull Requests
│
└── dependabot.yml       # Atualização automática de dependências
```

### Pipeline Principal (`ci.yml`)

```
┌─────────────────────────────────────────────────────────────────────┐
│                        CI/CD PIPELINE                                │
├─────────────────────────────────────────────────────────────────────┤
│                                                                      │
│  ┌──────────────┐    ┌──────────────┐    ┌──────────────┐          │
│  │  🧪 TEST     │───▶│  🔨 BUILD    │───▶│  🚀 DEPLOY   │          │
│  │  (Type Check │    │  (npm build) │    │  (GH Pages)  │          │
│  │   + Vitest)  │    │              │    │  main only   │          │
│  └──────────────┘    └──────────────┘    └──────────────┘          │
│                                                                      │
└─────────────────────────────────────────────────────────────────────┘
```

**Triggers:**
- Push para `main` ou `develop`
- Pull Request para `main`
- Manual via GitHub UI

**Jobs:**

| Job | Descrição | Dependência |
|-----|-----------|-------------|
| `test` | Type Check + Testes com cobertura | - |
| `build` | Build de produção | `test` |
| `deploy` | Deploy para GitHub Pages | `build` (apenas `main`) |

### PR Check (`pr-check.yml`)

Validação específica para Pull Requests com **matriz de Node.js**:

```
┌───────────────────────────────────────────────┐
│              PR CHECK MATRIX                   │
├───────────────────────────────────────────────┤
│                                               │
│  Node 20  ──────┬────▶  🔨 BUILD CHECK        │
│                 │                             │
│  Node 22  ──────┘                             │
│                                               │
└───────────────────────────────────────────────┘
```

**Testes executados em:**
- Node.js 20.x
- Node.js 22.x

> **Nota:** Node 18 foi removido pois `jsdom@27` requer Node 20+

### Dependabot

Atualização automática de dependências:

| Configuração | Valor |
|--------------|-------|
| Frequência | Semanal (Segunda-feira, 9h) |
| Timezone | America/Sao_Paulo |
| PRs simultâneos | 10 |
| Agrupamento | DevDeps, React, Vite |

**Grupos de dependências:**
- `development`: Types, Testing Library, Vitest, TypeScript
- `react`: React, React DOM
- `vite`: Vite e plugins

### Badges para Status

Adicione ao topo do README:

```markdown
![CI/CD](https://github.com/SEU_USER/sistema_de_reembolso/actions/workflows/ci.yml/badge.svg)
![PR Check](https://github.com/SEU_USER/sistema_de_reembolso/actions/workflows/pr-check.yml/badge.svg)
```

### Boas Práticas Implementadas

| Prática | Implementação |
|---------|---------------|
| **Cache de dependências** | `setup-node` com `cache: 'npm'` |
| **Instalação limpa** | `npm ci` em vez de `npm install` |
| **Concurrency** | Cancela runs duplicados |
| **Fail-fast desabilitado** | Matriz completa mesmo com falhas |
| **Artifacts** | Upload de coverage e build |
| **Permissões mínimas** | Apenas as necessárias para Pages |
| **Environments** | GitHub Pages como environment nomeado |
| **Dependabot** | Atualizações automáticas agrupadas |

### Configuração do GitHub Pages

1. Vá em **Settings** > **Pages**
2. Em **Source**, selecione **GitHub Actions**
3. O deploy acontecerá automaticamente em push para `main`

### Executar Localmente

Para simular o pipeline localmente:

```bash
# Type Check
npx tsc --noEmit

# Testes
npm run test:run

# Testes com cobertura
npm run test:coverage

# Build
npm run build
```

---

## 📱 Progressive Web App (PWA)

### Configuração (`vite.config.ts`)

```typescript
VitePWA({
  registerType: "autoUpdate",
  includeAssets: ["favicon.svg", "apple-touch-icon.png"],
  manifest: {
    name: "Sistema de Reembolso",
    short_name: "Reembolso",
    theme_color: "#1F8459",
    background_color: "#F9FBFA",
    display: "standalone",
    icons: [
      { src: "pwa-192x192.png", sizes: "192x192", type: "image/png" },
      { src: "pwa-512x512.png", sizes: "512x512", type: "image/png" },
      { src: "pwa-512x512.png", sizes: "512x512", type: "image/png", purpose: "maskable" }
    ]
  },
  workbox: {
    globPatterns: ["**/*.{js,css,html,ico,png,svg,woff2}"],
    runtimeCaching: [
      // Cache para Google Fonts
      { urlPattern: /^https:\/\/fonts\.googleapis\.com\/.*/, handler: "CacheFirst" },
      { urlPattern: /^https:\/\/fonts\.gstatic\.com\/.*/, handler: "CacheFirst" }
    ]
  }
})
```

### Prompt de Instalação

O componente `PWAInstallPrompt` intercepta o evento `beforeinstallprompt` e exibe um botão customizado para instalação.

---

## 🔍 SEO e Meta Tags

### Componente SEO

```typescript
<SEO 
  title="Lista de Solicitações" 
  description="Gerencie suas solicitações de reembolso."
/>
```

**Gera automaticamente:**
- `<title>` dinâmico
- Meta description
- Open Graph (Facebook, WhatsApp)
- Twitter Cards
- JSON-LD (dados estruturados)
- Canonical URL

### Arquivos Estáticos

- **`robots.txt`**: Permite indexação total
- **`sitemap.xml`**: Lista todas as páginas

---

## 🎨 Design System

### Cores (CSS Variables)

| Variável | Uso |
|----------|-----|
| `--gray-100` | Texto principal |
| `--gray-200` | Texto secundário |
| `--gray-300` | Bordas |
| `--gray-400` | Background principal |
| `--gray-500` | Background cards |
| `--green-100` | Cor primária (ações) |
| `--green-200` | Hover primária |
| `--green-300` | Disabled |
| `--white` | Texto em botões |

### Tipografia

- **Fonte**: Open Sans (Google Fonts)
- **Pesos**: 400 (regular), 600 (semibold), 700 (bold)

### Breakpoints (Tailwind)

| Breakpoint | Largura mínima |
|------------|----------------|
| `sm` | 640px |
| `md` | 768px |
| `lg` | 1024px |
| `xl` | 1280px |
| `2xl` | 1400px |

---

## 🔧 Instalação e Execução

### Pré-requisitos
- Node.js v20 ou superior (obrigatório - jsdom@27 requer Node 20+)
- npm ou yarn

### Passos

```bash
# 1. Clone o repositório
git clone https://github.com/glauccoeng-prog/sistema_de_reembolso.git
cd sistema_de_reembolso

# 2. Instale as dependências
npm install

# 3. Inicie o servidor de desenvolvimento
npm run dev

# 4. Acesse no navegador
# http://localhost:5173
```

### Build de Produção

```bash
# Gerar build otimizado
npm run build

# Preview local do build
npm run preview
```

---

## 📜 Scripts Disponíveis

| Script | Comando | Descrição |
|--------|---------|-----------|
| `dev` | `vite` | Inicia servidor de desenvolvimento |
| `build` | `vite build` | Gera build de produção |
| `lint` | `eslint .` | Verifica erros de lint |
| `lint:fix` | `eslint . --fix` | Corrige erros automaticamente |
| `format` | `prettier --write` | Formata todos os arquivos |
| `format:check` | `prettier --check` | Verifica formatação |
| `test` | `vitest` | Executa testes em modo watch |
| `test:run` | `vitest run` | Executa testes uma vez |
| `test:ui` | `vitest --ui` | Interface visual do Vitest |
| `test:coverage` | `vitest run --coverage` | Testes com cobertura de código |

---

## 💡 Decisões Técnicas Importantes

### 1. Mock API & LocalStorage
Para eliminar a necessidade de backend, foi criada uma camada de serviço que:
- Simula delay de rede (200-500ms)
- Persiste dados no localStorage
- Permite testar fluxos de loading
- Inicializa com dados de exemplo

### 2. React Query
Escolhido para gerenciamento de estado do servidor:
- Cache automático
- Refetch inteligente
- Estados de loading/error integrados
- Invalidação de cache simplificada

### 3. Download Seguro de Arquivos
Para evitar `ERR_BLOCKED_BY_CLIENT`:
- Conversão de Data URL para Blob
- Criação de Object URL temporário
- Revogação após download

### 4. Debounce na Busca
Hook `useDebounce` com 500ms:
- Evita requisições a cada tecla
- Melhora performance percebida
- Reduz uso de recursos

### 5. PWA com Vite Plugin
Geração automática de:
- Service Worker (Workbox)
- Manifest.json
- Ícones otimizados

### 6. Componentes Radix UI
Primitivos acessíveis garantem:
- Navegação por teclado
- ARIA attributes corretos
- Foco gerenciado

### 7. Estrutura Feature-Based
Organização por domínio facilita:
- Localização de código
- Testes isolados
- Escalabilidade

### 8. Testes com Vitest
Escolhido por ser nativo do Vite:
- Configuração zero com Vite
- API compatível com Jest
- Modo watch ultra-rápido
- Cobertura de código integrada
- Interface visual opcional

---

## 🗺️ Rotas da Aplicação

| Rota | Componente | Descrição |
|------|------------|-----------|
| `/` | `ListaDeReembolsos` | Tela inicial com lista |
| `/lista-de-reembolsos` | `ListaDeReembolsos` | Alias da tela inicial |
| `/detalhe-de-reembolso/:id` | `DetalheDeReembolso` | Detalhes de um reembolso |
| `/solicitacao-enviada` | `SolicitaoEnviada` | Confirmação de sucesso |

---

## 📦 Dependências Principais

### Produção
```json
{
  "react": "^18.2.0",
  "react-dom": "^18.2.0",
  "react-router-dom": "^6.8.1",
  "@tanstack/react-query": "^5.59.0",
  "react-hook-form": "^7.53.0",
  "react-helmet-async": "latest",
  "@radix-ui/react-dialog": "^1.1.2",
  "@radix-ui/react-select": "^2.1.2",
  "@radix-ui/react-toast": "^1.2.2",
  "@radix-ui/react-avatar": "^1.1.1",
  "@radix-ui/react-label": "^2.1.0",
  "@radix-ui/react-slot": "^1.1.0",
  "framer-motion": "latest",
  "lucide-react": "^0.453.0",
  "class-variance-authority": "^0.7.0",
  "clsx": "2.1.1",
  "tailwind-merge": "2.5.4",
  "tailwindcss-animate": "1.0.7",
  "vite-plugin-pwa": "latest"
}
```

### Desenvolvimento
```json
{
  "@vitejs/plugin-react": "4.3.4",
  "@types/react": "18.2.0",
  "@types/react-dom": "18.2.0",
  "@types/node": "^24.10.1",
  "vite": "6.0.4",
  "tailwindcss": "3.4.16",
  "esbuild": "0.24.0",
  "sharp": "^0.34.5",
  "vitest": "^3.2.4",
  "@vitest/coverage-v8": "^3.2.4",
  "@testing-library/react": "^16.3.0",
  "@testing-library/jest-dom": "^6.9.1",
  "@testing-library/user-event": "^14.6.1",
  "jsdom": "^27.2.0"
}
```

---

## 📄 Licença

Este projeto está sob a licença **MIT**. Sinta-se livre para usar, modificar e distribuir.

---

## 👨‍💻 Autor

**Glaucco Siqueira**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/glaucco-siqueira/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/glauccoeng-prog)

---

<div align="center">
  <sub>Desenvolvido com 💚 por Glaucco Siqueira</sub>
</div>
