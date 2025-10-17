# Flau Melo Mentorias

Landing page construída com Vue 3 e Vite para apresentar os serviços de mentoria, consultoria e conteúdos educacionais de Flau Melo. O site destaca a jornada de evolução profissional das mentoradas, depoimentos em formato de highlights e um canal direto de contato para novas parcerias.

## Visão geral
- **Objetivo**: gerar credibilidade para a mentora e facilitar o contato para contratação dos serviços.
- **Público-alvo**: profissionais de marketing e tecnologia que buscam orientação personalizada.
- **Entrega principal**: experiência single-page otimizada para dispositivos móveis e desktops.

## Seções da landing page
- **Banner inicial**: chamada para ação que aponta para as mentorias disponíveis.
- **Destaques da empresa**: cartões com diferenciais competitivos e métricas sociais.
- **Caminhos para o sucesso**: jornadas de desenvolvimento pessoal com CTA para agendamento.
- **Perfil da mentora**: biografia, competências e valores de atuação.
- **Depoimentos em vídeo**: destaques com trechos curtos de feedback das mentoradas.
- **Contato**: formulário e informações diretas (e-mail, telefone, redes sociais).

## Stack principal
- [Vue 3](https://vuejs.org/) com sintaxe `<script setup>`
- [Vite](https://vitejs.dev/) para bundler e servidor de desenvolvimento
- [Vue Router](https://router.vuejs.org/) para navegação entre seções
- [Pinia](https://pinia.vuejs.org/) preparado para gerenciamento de estado global
- [Tailwind CSS](https://tailwindcss.com/) aliado a SCSS modular
- [Vitest](https://vitest.dev/) para testes unitários

## Pré-requisitos
- Node.js 18 ou superior
- npm 9 ou superior

## Como executar o projeto
1. Clone o repositório e acesse a pasta `flau-melo`.
2. Instale as dependências com `npm install`.
3. Rode `npm run dev` para iniciar o servidor com hot-reload em `http://localhost:5173`.
4. Para gerar uma build de produção, use `npm run build` e sirva a pasta `dist/` com `npm run preview`.

## Scripts npm
```bash
npm install        # instala as dependências
npm run dev        # inicia o servidor de desenvolvimento
npm run build      # gera o build otimizado para produção em dist/
npm run preview    # serve localmente o build de produção
npm run test:unit  # executa a suíte de testes unitários com Vitest
npm run lint       # roda o ESLint sobre o código-fonte
```

## Estrutura do projeto
```
src/
├─ assets/              # imagens e recursos estáticos
├─ components/          # componentes reutilizáveis da landing page
├─ router/              # definição das rotas principais
├─ stores/              # stores do Pinia para estado compartilhado
├─ views/               # páginas de alto nível renderizadas pelo router
├─ main.ts              # ponto de entrada da aplicação
└─ App.vue              # layout raiz com Header e Footer
```

## Fluxo de contribuição
1. Crie um fork do repositório ou abra um branch a partir de `main`.
2. Siga as orientações descritas em [`AGENTS.md`](./AGENTS.md) para manter o padrão do projeto.
3. Utilize commits descritivos e em português.
4. Execute `npm run test:unit` e `npm run lint` antes de abrir um Pull Request.
5. Documente mudanças significativas no README e, quando houver alterações visuais, inclua capturas de tela.

## Qualidade e testes
- Priorize a criação de testes unitários para componentes que contenham lógica ou cálculos.
- Componentes puramente visuais podem ser validados com snapshots ou revisões manuais.
- Automatize verificações com os scripts `npm run test:unit` e `npm run lint`.

## Licença
Este projeto está disponível sob os termos definidos pela mantenedora. Entre em contato para obter mais detalhes sobre a utilização.
