# Tiago & Eliana — Wedding Manager

Aplicação web estática para organizar o casamento: orçamento e pagamentos, convidados, mesas, música, cronograma, tarefas, fornecedores, presentes e notas.

## Executar localmente

Abra `index.html` num navegador. A aplicação não precisa de instalação nem de um servidor de aplicação. Os dados são guardados no `localStorage` do navegador, por isso convém exportar cópias de segurança em **Definições**.

## Publicar no GitHub Pages

Este repositório está preparado para publicar automaticamente a partir da branch `main` através de GitHub Actions:

1. Crie um repositório no GitHub e envie os ficheiros do projeto para a branch `main`.
2. No repositório, abra **Settings → Pages** e escolha **GitHub Actions** como origem da publicação.3. Os envios para `main` irão publicar o conteúdo deste projeto.

O site é estático e não tem autenticação real. Na primeira utilização, o ecrã pede para criares uma palavra-passe, que fica guardada apenas no navegador. Isto não protege a aplicação contra acesso técnico nem oculta os dados; não coloques dados pessoais ou sensíveis numa publicação pública. Os dados guardados no navegador não são sincronizados entre dispositivos.

## Persistir uma base JSON

Em **Definições → Persistência em JSON**, usa **Criar ficheiro JSON** para iniciar um ficheiro no computador ou **Ligar ficheiro JSON existente** para carregar uma base já criada. Depois de autorizado, cada gravação na aplicação atualiza esse ficheiro, e a aplicação tenta voltar a ligar-se a ele quando é aberta no mesmo navegador e perfil. Para importar um backup JSON exportado anteriormente, usa **Importar backup**.

A ligação direta requer um navegador compatível (como Chrome ou Edge) e uma origem segura, como GitHub Pages. O ficheiro fica no dispositivo escolhido e não é uma base de dados alojada: não sincroniza automaticamente entre dispositivos nem utilizadores.
