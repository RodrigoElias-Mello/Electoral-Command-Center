# 🗳️ Electoral Command Center — Centro de Comando

<p align="center">
  <strong>Clareza para operar. Dados para decidir.</strong>
  <br />
  Inteligência operacional, gestão de equipes e acompanhamento de atividades em uma única plataforma.
</p>

<p align="center">
  <a href="https://nova-conversa-plum.vercel.app/">🌐 Acessar projeto</a>
</p>

---

## 📌 Sobre o projeto

O **Electoral Command Center** é uma aplicação web de gestão e inteligência operacional desenvolvida para centralizar informações, organizar equipes e acompanhar atividades relacionadas à operação de campanhas eleitorais.

A plataforma reúne ferramentas de gestão de eleitores, agenda, tarefas, lideranças, comunicação, busca avançada e acompanhamento de cobertura territorial.

Seu objetivo é proporcionar uma visão organizada da operação, permitindo que usuários autorizados consultem registros, acompanhem indicadores e gerenciem atividades em um ambiente digital integrado.

O sistema conta com autenticação, controle de permissões por módulo, painel administrativo e interface responsiva.

## 🎯 Objetivos

- Centralizar informações operacionais em um único ambiente.
- Organizar cadastros, lideranças, eventos e tarefas.
- Facilitar o acompanhamento das atividades e dos registros.
- Disponibilizar indicadores para apoiar a tomada de decisão.
- Controlar o acesso às informações conforme o perfil de cada usuário.
- Apoiar a comunicação operacional por meio de recursos de integração com WhatsApp.

## 🧭 Módulos da plataforma

### 📊 Visão geral — Dashboard

Painel principal com indicadores operacionais, evolução mensal de cadastros, próximos eventos, tarefas em aberto e atalhos para os módulos disponíveis ao usuário.

### 👥 Gestão de eleitores

Módulo para cadastro, consulta, edição e remoção de registros, incluindo informações de contato, endereço, zona, seção, categoria, etiquetas, observações e situação cadastral.

### 📅 Agenda da campanha

Organização de compromissos e atividades por data, horário e local, com informações sobre tipo, descrição, situação e quantidade prevista de participantes.

### ✅ Gestão de tarefas

Criação e acompanhamento de atividades com descrição, responsável, prazo, prioridade e status.

### 👥 Gestão de lideranças

Cadastro e gerenciamento de lideranças e responsáveis por regiões, facilitando a organização da estrutura operacional.

### 📣 Central de comunicação e despacho

Gerenciamento de contatos, solicitações e fila de despachos, com possibilidade de agendamento e integração com a API oficial do WhatsApp, quando devidamente configurada.

### 🔎 Busca avançada

Pesquisa de registros cadastrados utilizando os critérios disponíveis na interface.

### 📈 Cobertura e projeções

Visualização agregada de lideranças por região e registros por zona, permitindo acompanhar a distribuição territorial das informações cadastradas.

### 🔐 Usuários e administração

Gerenciamento de usuários e permissões específicas por recurso. O administrador pode controlar quais módulos ficam disponíveis para cada conta.

### ⚙️ Configurações

Área destinada às preferências da aplicação e opções relacionadas à experiência de utilização.

## ✨ Funcionalidades implementadas

- Autenticação e gerenciamento de sessões.
- Perfis de administrador e operador.
- Controle de permissões por módulo.
- Dashboard com indicadores operacionais.
- Cadastro, edição, consulta e gerenciamento de eleitores.
- Organização de eventos e compromissos.
- Gerenciamento de tarefas e prioridades.
- Cadastro e gerenciamento de lideranças.
- Fila de despachos e acompanhamento de solicitações.
- Integração com WhatsApp Web.
- Suporte à API oficial do WhatsApp mediante credenciais válidas.
- Pesquisa avançada de registros.
- Indicadores de cobertura territorial.
- Registro de auditoria de ações relevantes.
- Interface responsiva.
- Tema claro e escuro.
- Configuração de PWA para instalação da aplicação.
- Notificações visuais de ações realizadas.
- Integração com Vercel Analytics.

## 🎨 Interface e experiência do usuário

A experiência visual foi desenvolvida para transmitir clareza, organização e eficiência operacional.

Entre os principais aspectos da interface estão:

- Identidade visual institucional e neutra.
- Painéis com hierarquia clara de informações.
- Indicadores para leitura rápida dos dados.
- Navegação lateral com módulos condicionados às permissões.
- Componentes reutilizáveis.
- Layout adaptável a computadores, tablets e dispositivos móveis.
- Alternância entre temas claro e escuro.
- Controles com rótulos e estados visuais de acessibilidade.

## 🛠️ Tecnologias utilizadas

| Tecnologia | Aplicação |
|---|---|
| Next.js 16 | Framework e estrutura da aplicação |
| React 19 | Construção da interface |
| TypeScript 5 | Tipagem e organização do código |
| Tailwind CSS 4 | Estilização |
| Radix UI | Componentes acessíveis |
| shadcn/ui | Composição de componentes visuais |
| Lucide React | Biblioteca de ícones |
| Recharts | Gráficos e indicadores |
| Better Auth | Autenticação e sessões |
| PostgreSQL | Banco de dados relacional |
| Drizzle ORM | Mapeamento e consultas ao banco |
| Zod | Validação de dados |
| SWR | Busca e atualização de dados |
| React Hook Form | Gerenciamento de formulários |
| date-fns | Manipulação de datas |
| WhatsApp Business Platform | Integração opcional de comunicação |
| Vercel Analytics | Análise de acesso |
| pnpm | Gerenciamento de dependências |

## 📂 Estrutura do projeto

```text
Electoral-Command-Center/
├── app/
│   ├── actions/
│   │   └── campaign.ts
│   ├── api/
│   │   └── auth/
│   ├── dashboard/
│   │   ├── admin/
│   │   ├── calendar/
│   │   ├── dispatch/
│   │   ├── projections/
│   │   ├── search/
│   │   ├── settings/
│   │   ├── tasks/
│   │   ├── users/
│   │   └── voters/
│   ├── globals.css
│   ├── layout.tsx
│   ├── manifest.ts
│   └── page.tsx
│
├── components/
│   ├── ui/
│   ├── admin-access-panel.tsx
│   ├── auth-provider.tsx
│   ├── brand.tsx
│   ├── calendar-grid.tsx
│   ├── capacity-projection.tsx
│   ├── dashboard-overview.tsx
│   ├── dispatch-center.tsx
│   ├── event-form.tsx
│   ├── login-form.tsx
│   ├── task-form.tsx
│   ├── voter-detail-dialog.tsx
│   └── voter-form.tsx
│
├── hooks/
│   ├── use-mobile.ts
│   └── use-toast.ts
│
├── lib/
│   ├── db/
│   │   ├── index.ts
│   │   └── schema.ts
│   ├── access-control.ts
│   ├── auth-client.ts
│   ├── auth.ts
│   ├── dashboard-types.ts
│   ├── mock-data.ts
│   ├── theme.ts
│   ├── utils.ts
│   └── whatsapp.ts
│
├── public/
│   ├── icon-192-v3.png
│   ├── icon-512-v3.png
│   ├── icon.svg
│   └── sw.js
│
├── styles/
│   └── globals.css
│
├── components.json
├── next.config.mjs
├── package.json
├── pnpm-lock.yaml
├── pnpm-workspace.yaml
├── postcss.config.mjs
└── tsconfig.json
```

## 🚀 Executando o projeto localmente

### Pré-requisitos

- Node.js compatível com Next.js 16.
- pnpm instalado.
- Git instalado.
- Banco de dados PostgreSQL acessível.

### 1. Clone o repositório

```bash
git clone https://github.com/RodrigoElias-Mello/Electoral-Command-Center.git
```

### 2. Acesse a pasta

```bash
cd Electoral-Command-Center
```

### 3. Instale as dependências

```bash
pnpm install
```

### 4. Configure as variáveis de ambiente

Crie um arquivo `.env.local` na raiz do projeto:

```env
DATABASE_URL="postgresql://USUARIO:SENHA@HOST:5432/NOME_DO_BANCO"

BETTER_AUTH_URL="http://localhost:3000"

# Opcionais: integração com a API oficial do WhatsApp
WHATSAPP_ACCESS_TOKEN=""
WHATSAPP_PHONE_NUMBER_ID=""
```

**Importante:**
- `DATABASE_URL` é necessária para a conexão com o PostgreSQL.
- `BETTER_AUTH_URL` define a URL base da autenticação.
- As credenciais do WhatsApp são necessárias somente quando a integração oficial estiver habilitada.
- Nunca publique credenciais ou arquivos `.env.local` no GitHub.

### 5. Prepare o banco de dados

O schema das tabelas está definido em:

```text
lib/db/schema.ts
```

Antes de executar a aplicação em um ambiente novo, disponibilize no PostgreSQL as tabelas correspondentes ao schema.

**Observação técnica:** o repositório contém o schema Drizzle, mas não inclui arquivos de migração nem um comando de migração configurado. A criação e atualização das tabelas precisam ser realizadas por um processo compatível com esse schema.

### 6. Execute em desenvolvimento

```bash
pnpm dev
```

Acesse:

```text
http://localhost:3000
```

### 7. Gere a versão de produção

```bash
pnpm build
```

### 8. Execute a versão de produção

```bash
pnpm start
```

### 9. Verifique a qualidade do código

```bash
pnpm lint
```

## 🔐 Segurança e proteção de dados

A aplicação utiliza autenticação com Better Auth, sessões persistidas no banco de dados e autorização por recursos.

O sistema contempla:

- Perfis de administrador e operador.
- Permissões específicas para os módulos.
- Verificação de sessão e autorização nas ações operacionais.
- Registro de auditoria de operações relevantes.
- Cabeçalhos HTTP de proteção.

Como a plataforma pode armazenar dados pessoais, sua implantação e utilização devem observar a Lei Geral de Proteção de Dados (LGPD).

É responsabilidade da organização definir a finalidade e a base legal do tratamento, limitar os dados coletados, controlar os acessos, proteger credenciais, estabelecer políticas de retenção e atender aos direitos dos titulares.

**Recomendação:** não utilize dados pessoais reais em ambientes de demonstração sem as medidas adequadas de proteção.

## 🌐 Projeto publicado

A aplicação está disponível online:

**https://nova-conversa-plum.vercel.app/**

O acesso às áreas internas exige autenticação e permissões válidas.

## 👨‍💻 Desenvolvedor

**Rodrigo Elias Alfama de Mello**

Desenvolvedor Web | Front-End | Soluções Digitais

Formado em Análise e Desenvolvimento de Sistemas, com foco no desenvolvimento de aplicações web, interfaces modernas e soluções digitais.

<p align="center">
  <a href="https://portifolio-rodrigo-elias.vercel.app/">Portfólio</a> •
  <a href="https://www.linkedin.com/in/rodrigoelias1709">LinkedIn</a> •
  <a href="https://github.com/RodrigoElias-Mello">GitHub</a>
</p>

---

<p align="center">
  <strong>Desenvolvido por Elias Technology.</strong>
  <br />
  🗳️ Electoral Command Center — Clareza operacional para decisões mais conscientes.
</p>
