# DevMind — protótipo navegável

## O que é
Portal informativo em português sobre a influência da Inteligência Artificial no planejamento da Engenharia de Software. O produto é um portal editorial, não um gerenciador de projetos.

## Executar
1. Extraia o arquivo ZIP.
2. Abra `index.html` num navegador moderno.
3. Navegue pelo menu superior.
4. Acesse **Área editorial** para testar o CMS.

Não é necessário instalar dependências ou iniciar servidor para testar o protótipo.

## Funcionalidades implementadas
- Página inicial editorial.
- Catálogo de artigos.
- Pesquisa global e pesquisa no catálogo.
- Filtros por assunto, etapa do ciclo de vida, nível e tipo.
- Ordenação por data ou título.
- Categorias.
- Página de leitura com índice e âncoras para seções.
- Referências e artigos relacionados.
- Página Sobre.
- CMS local para criar, editar, publicar, manter rascunhos e excluir artigos.
- Layout responsivo para desktop e dispositivos móveis.
- Persistência do CMS via `localStorage`.

## Limitações conhecidas
- CMS local, sem autenticação, perfis, servidor ou sincronização.
- Conteúdo inicial é demonstrativo. As referências devem ser verificadas individualmente antes de publicação pública.
- Não existe integração com bases bibliográficas ou APIs externas.
- A pesquisa é textual e limitada aos dados carregados no navegador.
- Não há fluxo de revisão editorial multiutilizador.

## Estrutura
- `index.html`: estrutura e pontos de entrada.
- `styles.css`: identidade visual e responsividade.
- `app.js`: navegação, dados, filtros, leitura e CMS.

## Evolução recomendada para produção
1. Migrar para Next.js + TypeScript.
2. Adotar CMS com autenticação e controle de permissões.
3. Persistir artigos em PostgreSQL ou serviço gerenciado.
4. Implementar workflow editorial (rascunho, revisão, publicação).
5. Criar testes automatizados e pipeline de integração contínua.
6. Configurar domínio, hospedagem, backups, monitoramento, política de privacidade e LGPD.
7. Revisar as referências e conteúdos com responsável editorial.

## Observação sobre dados
O CMS salva os artigos no `localStorage` do navegador. Limpar os dados do site ou trocar de navegador pode apagar ou tornar inacessíveis as alterações. Exporte/registre o conteúdo antes de qualquer limpeza.
