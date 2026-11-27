<h1 align="center">Alex Marques</h1>

<p align="center">
  <strong>Desenvolvedor Full Stack</strong> · Rio de Janeiro, RJ · Disponível para trabalho remoto
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/alex-marques-455089205"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="https://mavox-web-ten.vercel.app"><img src="https://img.shields.io/badge/Mavox_Web-111111?style=for-the-badge&logo=vercel&logoColor=white" alt="Mavox Web"/></a>
</p>

---

## Sobre mim

Construo sistemas web de ponta a ponta: do levantamento de requisitos à arquitetura, ao desenvolvimento e à implantação em produção.

- 🔌 **Integrações:** ERP ↔ e-commerce, APIs de marketplaces, webhooks e gateways de pagamento (Mercado Pago, Pagar.me, Cielo, Asaas, Stripe)
- 🏢 **SaaS multi-tenant:** permissões, dashboards e APIs REST para clientes de saúde, moda e varejo
- ⚙️ **Automação:** n8n, Evolution API e fluxos de CRM e captação de leads
- 🐳 **Infra:** Docker, Linux/VPS, Redis, AWS e Vercel
- 🎓 Cursando **Ciência da Computação** (UniCV, conclusão prevista para 2027)

## Stack

**Back-end**<br/>
<img src="https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white"/>
<img src="https://img.shields.io/badge/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white"/>
<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white"/>
<img src="https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white"/>
<img src="https://img.shields.io/badge/Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white"/>

**Front-end**<br/>
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/>
<img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB"/>
<img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white"/>
<img src="https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white"/>
<img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white"/>

**Mobile**<br/>
<img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white"/>
<img src="https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white"/>
<img src="https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white"/>

**Banco de dados**<br/>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white"/>
<img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
<img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white"/>
<img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/>

**DevOps e ferramentas**<br/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black"/>
<img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/>
<img src="https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white"/>
<img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white"/>

## Projetos em destaque

### 💳 Wallet Ledger: carteira digital de ponta a ponta

O foco é não errar com dinheiro: do banco de dados até o dedo de quem toca em "Confirmar", e até a mesa de quem atende o cliente quando algo dá errado.

**[API](https://github.com/Mavoxweb/wallet-ledger-api)**: livro-razão de **partidas dobradas**, com contas, PIX por chave, extrato e QR code BR Code. Nenhum saldo negativo sob concorrência (testado com 100 transferências simultâneas), nenhuma cobrança duplicada em repetições (idempotência atômica no PostgreSQL) e cada decisão registrada em ADRs.

`.NET 10` · `ASP.NET Core` · `EF Core` · `PostgreSQL` · `Testcontainers` · `Docker` · `GitHub Actions` · 195 testes

**[App](https://github.com/Mavoxweb/wallet-ledger-mobile)**: o correntista em Flutter, com saldo, PIX por chave ou QR code, extrato e cobrança. Se a conexão cai no meio de um PIX, tentar de novo devolve o mesmo comprovante, sem debitar duas vezes. Cliente HTTP gerado do contrato da API, APK publicado a cada versão.

`Flutter` · `Dart` · `Bloc` · `go_router` · `Dio` · `OpenAPI` · 136 testes

**[Backoffice](https://github.com/Mavoxweb/wallet-ledger-backoffice)**: o painel da operação em Angular. Busca a conta pelo CPF, e-mail ou final da conta, bloqueia na hora (inclusive no app que já está aberto), estorna um PIX sem risco de estornar duas vezes e registra quem fez o quê, quando e por quê. A regra de quem pode o quê fica na API; a tela só esconde.

`Angular 22` · `Signals` · `Angular Material` · `RxJS` · `OpenAPI` · `Vitest` · `Playwright` · 78 testes + e2e

| Outros projetos | O que é | Stack |
|---|---|---|
| [**ocafy**](https://github.com/Mavoxweb/ocafy) | App de gestão doméstica gamificada. Monorepo com web, mobile e API tipada | Next.js · Expo · tRPC · Drizzle · Neon · Turborepo |
| [**mavox-web**](https://github.com/Mavoxweb/mavox-web) | Site da agência Mavox com banco, migrations e testes E2E | Next.js 15 · TypeScript · Tailwind · Neon · Playwright |
| [**sensormercadob2b**](https://github.com/Mavoxweb/sensormercadob2b) | Plataforma B2B de inteligência de mercado e precificação para varejo | Next.js 16 · React 19 · TypeScript · Tailwind |
| [**TGX-engenharia-solucoes**](https://github.com/Mavoxweb/TGX-engenharia-solucoes) | Site institucional B2B com blog, formulário validado e SEO técnico | React · TypeScript · Vite · Tailwind |

> Boa parte do meu trabalho é para clientes e não tem código público. Mostro a arquitetura e demonstro os sistemas em entrevista.
