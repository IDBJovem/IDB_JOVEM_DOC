# Entrega Final — IDB Jovem & Teen

---

## Sobre o Projeto

O **IDB Jovem & Teen** é uma plataforma web desenvolvida para a **Igreja de Deus** com foco nas atividades do público jovem. O projeto consiste em uma landing page estratégica para divulgação de eventos, apresentação da identidade, localização e centralização das informações essenciais da comunidade.

Seu principal objetivo é reunir tudo em um único ambiente acessível, onde membros e visitantes possam encontrar rapidamente o que precisam. A plataforma permite que usuários acompanhem eventos, participem como voluntários, visualizem novidades e acessem produtos disponíveis, promovendo uma experiência mais integrada.

Além disso, oferece suporte a líderes e administradores por meio de funcionalidades de organização de eventos, gerenciamento de voluntários e divulgação de informações.

| Item | Detalhe |
|:-----|:--------|
| Cliente | Pra. Raquel Gomes — Diretora Nacional e Regional de Adolescentes (Região Central) |
| Sistema em produção | [idbjovemeteen.tech](https://www.idbjovemeteen.tech/) |
| Repositório | [github.com/IDBJovem](https://github.com/IDBJovem) |
| Documentação | [idbjovem.github.io/IDB_JOVEM_DOC](https://idbjovem.github.io/IDB_JOVEM_DOC/) |
| Hospedagem Back-end | Hostinger VPS KVM 2 |
| Hospedagem Front-end | Vercel |
| Stack | Python, FastAPI, PostgreSQL, Docker, React, Playwright |

---

## Equipe

| Membro | GitHub |
|:-------|:-------|
| Enzo Emir | [@EnzoEmir](https://github.com/EnzoEmir) |
| Gabriel Monteiro | [@GabrielSMonteiro](https://github.com/GabrielSMonteiro) |
| Leticia Arisa | [@Leticia-Arisa-K-Higa](https://github.com/Leticia-Arisa-K-Higa) |
| Marcelo Makoto | [@MM4k](https://github.com/MM4k) |
| Maria Eduarda | [@dudaa28](https://github.com/dudaa28) |
| Victor Pontual | [@VictorPontual](https://github.com/VictorPontual) |

---

## Entrega Final

A entrega principal consiste no vídeo de validação com a cliente utilizando o sistema em produção com sua conta corporativa.

<div style="text-align: center;">
  <iframe width="560" height="315" src="https://www.youtube.com/embed/_42fkrwe6Hk" title="Entrega Final — IDB Jovem & Teen" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

---

## Ponto de Controle 1

| Artefato | Descrição |
|:---------|:----------|
| Backlog do Produto | [Ver documentação](https://idbjovem.github.io/IDB_JOVEM_DOC/) |
| Protótipo de Alta Fidelidade | Figma — telas web e mobile |
| Docker | Ambiente containerizado configurado |
| Back-end | 1 endpoint funcional em container |
| Banco de dados | PostgreSQL com IDE integrada |
| Front-end | Hello World React |

---

## Ponto de Controle 2

| Artefato | Descrição |
|:---------|:----------|
| Back-end completo | API FastAPI — web e mobile |
| CI/CD | Pipeline configurado no repositório |
| Clean Code | Código revisado e refatorado |
| Testes parametrizados | Cobertura dos principais fluxos da API |
| Testes de integração | Apontando para endpoints em container |

---

## Ponto de Controle 3

| Artefato | Descrição |
|:---------|:----------|
| Front-end completo | Interface React — web e mobile |
| Validação com a cliente | Pra. Raquel Gomes com conta corporativa em produção |
| Vídeo tutorial | Treinamento de uso do sistema |
| Testes E2E | Playwright cobrindo os fluxos críticos |
| Hospedagem Front-end | Vercel |
| Hospedagem Back-end | [idbjovemeteen.tech](https://www.idbjovemeteen.tech/) — Hostinger |

### Stacks do Front-end

| Tecnologia | Descrição |
|:-----------|:----------|
| [React 19](https://react.dev/) | Biblioteca JavaScript para criação da interface de usuário |
| [Vite](https://vitejs.dev/) | Ferramenta de build extremamente rápida e servidor de desenvolvimento |
| [Tailwind CSS 4](https://tailwindcss.com/) | Framework de CSS utilitário para estilização rápida e responsiva |
| [React Router DOM](https://reactrouter.com/) | Biblioteca para gerenciamento de rotas e navegação da aplicação |
| [Lucide React](https://lucide.dev/) | Biblioteca de ícones modernos e limpos |
| [Playwright](https://playwright.dev/) | Framework de testes End-to-End (E2E) para testar fluxos de interface |
| [NYC / Istanbul](https://istanbul.js.org/) | Ferramenta de instrumentação e relatório para cobertura de testes |

### Hospedagem

**A documentação completa sobre o levantamento de hospedagem pode ser acessada em:** [Hospedagem_IDB.pdf](../assets/Hospedagem_IDB.pdf)

O projeto adota uma arquitetura dividida: o **frontend** é servido via CDN global pela **Vercel** (gratuito, deploy automático a cada push no GitHub), enquanto o **backend**, banco de dados e autenticação rodam em um **VPS Hostinger KVM 2**.

#### Especificações do VPS

| Recurso | Especificação |
|:--------|:--------------|
| CPU | 2 vCPUs |
| Memória RAM | 8 GB |
| Armazenamento | 100 GB NVMe/SSD |
| Transferência | 8 TB/mês |

#### Justificativa da escolha

O plano **Hostinger KVM 2** foi escolhido por atender com folga os requisitos da stack: o Keycloak (IAM) consome aproximadamente 1,7–2 GB de RAM, o PostgreSQL cerca de 512 MB–1 GB, e o FastAPI é leve em memória. Com 8 GB de RAM, todos os serviços operam sem risco de travamentos, com margem para crescimento.

#### Comparativo de provedores

| Hospedagem | Preço anual | Servidor | CPU | Memória | Armazenamento | Transferência |
|:-----------|:------------|:---------|:----|:--------|:--------------|:--------------|
| Hostinger KVM 2 | R$ 599,88 | EUA | 2 vCPUs | 8 GB | 100 GB NVMe | 8 TB/mês |
| Hostgator VPS NVMe 8 | R$ 1.019,88 | Brasil | 4 vCPUs | 8 GB | 200 GB NVMe | Ilimitada |

A **Hostinger** foi a escolhida pelo melhor custo-benefício para a fase inicial do projeto. A Hostgator oferece servidor no Brasil (menor latência para usuários brasileiros) e mais CPU/armazenamento, sendo uma opção de upgrade natural caso o uso da aplicação cresça.

---

## Histórico de Versão

| Versão | Data | Descrição | Autor(es) |
|:-------|:-----|:----------|:----------|
| `1.0` | 16/06/2026 | Criação da página de entrega final | [Enzo Emir](https://github.com/EnzoEmir), [Gabriel Monteiro](https://github.com/GabrielSMonteiro), [Leticia Arisa](https://github.com/Leticia-Arisa-K-Higa), [Marcelo Makoto](https://github.com/MM4k), [Maria Eduarda](https://github.com/dudaa28), [Victor Pontual](https://github.com/VictorPontual) |