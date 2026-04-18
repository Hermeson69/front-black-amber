### Black amber coffe front end service

### Uso do Repo:
1. Clone o repositório: `git clone`
2. Instale as dependências: `npm install`
3. Configure as variáveis de ambiente: crie um arquivo `.env` na raiz do projeto e adicione as seguintes variáveis conforme o `.env.exemple`:
   ```
   BACKENDURL=URL_DO_SEU_BACKEND
   ```
4. Inicie o servidor de desenvolvimento: `npm run dev`
5. Caso de build rodar: `npm run build`

## Arquitetura prevista para o projeto, sujeita a mudanças conforme o desenvolvimento avança.
```bash
src/
│
├── assets/
│
├── core/
│   ├── api/
│   ├── config/
│   ├── websocket/
│   └── guards/
│
├── features/
│
│   ├── chat/
│   │   ├── components/
│   │   ├── hooks/
│   │   ├── services/
│   │   ├── store/
│   │   └── pages/
│   │
│   ├── auth/
│   ├── documents/
│   ├── memory-lex/
│   ├── jury/
│   ├── whisper/
│   ├── billing/
│   └── analytics/
│
├── layout/
│   ├── DashboardLayout.tsx
│   ├── AuthLayout.tsx
│   └── FocusLayout.tsx
│
├── routes/
│   ├── AppRoutes.tsx
│   └── PrivateRoute.tsx
│
├── shared/
│   ├── components/
│   │   ├── AppSidebar.tsx
│   │   ├── AppHeader.tsx
│   │   ├── Loading.tsx
│   │   ├── EmptyState.tsx
│   │   └── ErrorState.tsx
│   │
│   ├── hooks/
│   ├── types/
│   ├── utils/
│   └── lib/
│
├── styles/
├── App.tsx
└── main.tsx
```

cada feature tem sua própria pasta, contendo seus componentes, hooks, serviços, store e páginas. O core contém funcionalidades compartilhadas entre as features, como configuração de API, websocket e guards. O layout contém os layouts principais da aplicação, enquanto o shared contém componentes, hooks, tipos e utilitários compartilhados entre as features.

#### Aviso:
por enquanto, já que o back tambem esta em produção tudo vai ser dados mockados, ou seja, não haverá integração real com o backend, mas a estrutura de pastas e arquivos já está preparada para receber essa integração no futuro.