# Instruções para Pessoas Desenvolvedoras

## Escopo
Estas diretrizes se aplicam a todo o repositório.

## Diretrizes de Código
- Preserve a estrutura atual baseada em Vue 3 + Vite.
- Prefira a Composition API e a sintaxe `<script setup>` ao criar componentes Vue.
- Mantenha os estilos junto de cada componente usando blocos `lang="scss"` nos Single File Components, a menos que seja necessária uma utilidade compartilhada.
- Não adicione dependências de runtime sem atualizar a documentação no README.

## Testes
- Antes de enviar alterações que afetem a lógica da aplicação ou componentes, execute `npm run test:unit`.
- Para mudanças apenas visuais ou de conteúdo, os testes são opcionais; caso pule, registre isso no resumo final.

## Documentação
- Atualize o README sempre que adicionar ou modificar scripts npm, ferramentas ou fluxos importantes da interface.
