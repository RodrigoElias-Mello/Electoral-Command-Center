🗳️ Electoral Command Center — Centro de Comando
<p align="center">
  <img src="./public/icon-512-v3.png" alt="Electoral Command Center — Centro de Comando" width="180" />
</p><p align="center">
  <strong>Clareza para operar. Dados para decidir.</strong>
  <br />
  Inteligência operacional, gestão de equipes e acompanhamento de atividades em uma única plataforma.
</p><p align="center">
  <a href="https://nova-conversa-plum.vercel.app/">🌐 Acessar projeto</a>
</p>📌 Sobre o projeto
O Electoral Command Center é uma aplicação web de gestão e inteligência operacional desenvolvida para centralizar informações, organizar equipes e acompanhar atividades relacionadas à operação de uma campanha.

A plataforma reúne módulos de visão geral, cadastro de eleitores, agenda, tarefas, lideranças, comunicação, busca e acompanhamento de cobertura. A proposta é oferecer uma leitura organizada da operação, permitindo que usuários autorizados consultem registros e acompanhem indicadores com base nas informações cadastradas.

Com acesso autenticado, permissões por módulo e interface responsiva, o sistema foi estruturado para apoiar a organização administrativa e facilitar o acompanhamento das atividades em um ambiente integrado.
🎯 Objetivos
- Centralizar informações operacionais em um único ambiente.
- Organizar cadastros, lideranças, eventos e tarefas.
- Facilitar o acompanhamento das atividades e dos registros da operação.
- Disponibilizar indicadores e consultas para apoiar a tomada de decisão.
- Controlar o acesso às informações conforme o perfil e as permissões de cada usuário.
- Apoiar a comunicação operacional com recursos de encaminhamento pelo WhatsApp.
🧭 Módulos da plataforma
📊 Visão geral
Painel inicial com indicadores vinculados aos registros da conta, evolução mensal de cadastros, próximos eventos, tarefas em aberto e atalhos para os módulos disponíveis ao usuário.
👥 Gestão de eleitores
Cadastro, consulta, edição e remoção de registros, com informações de contato, endereço, zona, seção, categoria, etiquetas, observações e situação do cadastro.
📅 Agenda da campanha
Organização de compromissos e atividades por data, horário e local, com informações sobre tipo, descrição, situação e quantidade prevista de participantes.
✅ Gestão de tarefas
Criação e acompanhamento de atividades, com descrição, responsável, prazo, prioridade e status para facilitar a organização das demandas.
📣 Central de comunicação e despacho
Gerenciamento de lideranças e contatos, organização de solicitações e fila de despachos, com possibilidade de agendamento e integração de envio pela API oficial do WhatsApp quando configurada.
🔎 Busca avançada
Consulta de registros por critérios disponíveis na interface, facilitando a localização de informações cadastradas na plataforma.
📈 Cobertura e projeções
Visualização agregada de lideranças por região e registros por zona, oferecendo uma leitura da distribuição territorial com base nos dados cadastrados.
🔐 Usuários e administração
Gestão de usuários e concessão de permissões por recurso. O perfil administrador possui acesso à área administrativa e pode controlar quais módulos ficam disponíveis para cada conta.
⚙️ Configurações
Área de preferências da aplicação, incluindo opções de apresentação e configurações relacionadas à experiência de uso.
✨ Funcionalidades implementadas
- Autenticação: acesso por conta, com gerenciamento de sessão.
- Controle de acesso: perfis de administrador e operador, além de permissões específicas por módulo.
- Dashboard operacional: indicadores, gráfico de evolução dos cadastros, agenda próxima e atalhos contextuais.
- Cadastro de eleitores: inclusão, edição, consulta, categorização e gerenciamento de registros.
- Agenda: criação e manutenção de eventos e compromissos.
- Tarefas: organização de demandas por prioridade, responsável, prazo e situação.
- Lideranças: cadastro e gerenciamento de responsáveis por região.
- Fila de despachos: registro, agendamento e acompanhamento do status de solicitações.
- WhatsApp: abertura de conversas pelo WhatsApp Web e suporte à API oficial mediante credenciais válidas.
- Busca avançada: pesquisa de informações cadastradas.
- Indicadores de cobertura: agrupamento de lideranças por região e registros por zona.
- Registro de auditoria: histórico de ações relevantes realizadas nos módulos operacionais.
- Interface responsiva: navegação adaptada a diferentes tamanhos de tela.
- Tema visual: suporte a apresentação clara e escura.
- PWA: configuração de manifesto e registro de service worker para recursos de instalação da aplicação.
- Notificações visuais: mensagens de retorno para ações realizadas na interface.
- Analytics: integração com Vercel Analytics para acompanhamento de acesso em produção.
🎨 Interface e experiência do usuário
O desenvolvimento visual prioriza:
- Identidade visual institucional e alinhada a um centro de comando.
- Interface organizada com hierarquia clara de informações.
- Painéis e indicadores para leitura rápida dos dados.
- Navegação lateral com módulos condicionados às permissões do usuário.
- Componentes reutilizáveis e padrões visuais consistentes.
- Layout responsivo para desktop, tablets e dispositivos móveis.
- Alternância entre temas claro e escuro.
- Elementos de acessibilidade, incluindo rótulos, estados de foco e descrições para controles.
🛠️ Tecnologias utilizadas
Tecnologia	Aplicação
Next.js 16	Framework da aplicação e estrutura de rotas
React 19	Construção da interface
TypeScript 5	Tipagem e organização do código
Tailwind CSS 4	Estilização da interface
Radix UI	Componentes acessíveis de interface
shadcn/ui	Base e composição de componentes visuais
Lucide React	Biblioteca de ícones
Recharts	Gráficos e visualização de indicadores
Better Auth	Autenticação e gerenciamento de sessões
PostgreSQL	Banco de dados relacional
Drizzle ORM	Mapeamento e consultas ao banco de dados
Zod	Validação de dados
SWR	Busca e atualização de dados no cliente
React Hook Form	Gerenciamento de formulários
date-fns	Manipulação de datas
WhatsApp Business Platform	Integração opcional com a API oficial do WhatsApp
Vercel Analytics	Análise de acesso em produção
pnpm	Gerenciamento de dependências


📂 Estrutura do projeto
electoral-command-center/
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
├── tsconfig.json
└── README.md
🚀 Como executar o projeto localmente
Pré-requisitos
- Node.js compatível com Next.js 16.
- pnpm instalado.
- Git instalado.
- Banco de dados PostgreSQL acessível.
1. Clone o repositório
git clone URL_DO_REPOSITORIO
2. Entre na pasta do projeto
cd electoral-command-center
3. Instale as dependências
pnpm install
4. Configure as variáveis de ambiente
Crie um arquivo .env.local na raiz do projeto:
DATABASE_URL="postgresql://USUARIO:SENHA@HOST:5432/NOME_DO_BANCO"
BETTER_AUTH_URL="http://localhost:3000"

# Necessárias somente para habilitar o envio pela API oficial do WhatsApp
WHATSAPP_ACCESS_TOKEN=""
WHATSAPP_PHONE_NUMBER_ID=""
DATABASE_URL é obrigatória para a conexão com o PostgreSQL. BETTER_AUTH_URL define a URL base da autenticação. As credenciais do WhatsApp são opcionais e só devem ser preenchidas quando a integração oficial estiver configurada.
5. Prepare o banco de dados
O modelo das tabelas está definido em lib/db/schema.ts. Antes de iniciar a aplicação, disponibilize no PostgreSQL as tabelas correspondentes ao schema da aplicação.

Observação: o repositório contém o schema Drizzle, mas não inclui arquivos de migração nem um comando de migração configurado. Portanto, a criação e atualização das tabelas devem ser realizadas por um processo de migração compatível com o schema antes da execução em um ambiente novo.
6. Execute em ambiente de desenvolvimento
pnpm dev
7. Acesse no navegador
http://localhost:3000
8. Gere a versão de produção
pnpm build
9. Execute a versão de produção localmente
pnpm start
🔒 Segurança e controle de acesso
A aplicação utiliza autenticação com Better Auth, sessões persistidas no banco de dados e autorização por recursos. O primeiro usuário criado recebe o perfil de administrador; os usuários seguintes são registrados como operadores. O administrador pode conceder ou revogar permissões específicas para os módulos disponíveis.

As ações operacionais são executadas no servidor e verificam a sessão e a permissão correspondente. O projeto também mantém registros de auditoria para operações relevantes e configura cabeçalhos HTTP de proteção.

Como a plataforma pode armazenar dados pessoais, sua implantação e utilização devem observar a Lei Geral de Proteção de Dados (LGPD). É responsabilidade da organização definir finalidade e base legal, limitar os dados coletados, controlar acessos, proteger credenciais, estabelecer retenção e atender aos direitos dos titulares. Não utilize dados reais em ambientes de demonstração sem as medidas adequadas.
🌐 Projeto publicado
A aplicação possui endereço de produção configurado nos metadados do projeto:

https://nova-conversa-plum.vercel.app/

O acesso às áreas internas exige autenticação e permissões válidas.
👨‍💻 Desenvolvedor
Rodrigo Elias Alfama de Mello

Desenvolvedor Web | Front-End | Soluções Digitais

Formado em Análise e Desenvolvimento de Sistemas, com foco no desenvolvimento de aplicações web, interfaces modernas e soluções digitais.
<p align="center">
  <a href="https://v0-rodrigoelias-portfolio.vercel.app/">Portfólio</a> •
  <a href="https://www.linkedin.com/in/rodrigoelias1709">LinkedIn</a> •
  <a href="https://github.com/Elias-1709">GitHub</a>
</p><p align="center">
  🗳️ <strong>Electoral Command Center — Clareza operacional para decisões mais conscientes.</strong>
  <br />
  Desenvolvido por <strong>Elias Technology</strong>.
</p>
