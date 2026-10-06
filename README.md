# Tiago & Eliana — Wedding Manager

Aplicação web estática para organizar o casamento: orçamento e pagamentos, convidados, mesas, música, cronograma, tarefas, fornecedores, presentes e notas.

## Executar localmente

Abra `index.html` num navegador. Os dados ficam no armazenamento desse navegador. A lista inicial de convidados vem de `data/wedding-manager.json` (a aplicação preserva dados já existentes no navegador).

## Base de dados JSON e CRUD

Em **Definições → Persistência em JSON**, usa **Guardar dados atuais num JSON** para escrever o estado atual da aplicação (incluindo convidados já adicionados) num ficheiro escolhido e ligá-lo. Daí em diante, os guardados atualizam automaticamente esse ficheiro e a ligação é recordada neste navegador. **Ler e ligar ficheiro JSON** carrega os dados do ficheiro selecionado para a aplicação. Sem ficheiro ligado, os dados ficam apenas no armazenamento do navegador e a aplicação indica esse estado. Na lista de convidados podes criar, consultar, editar e apagar registos. A importação e exportação de backups também estão disponíveis.

O navegador precisa de suportar a File System Access API (por exemplo, Chrome ou Edge) para escrever diretamente num ficheiro escolhido. GitHub Pages serve a aplicação e o ficheiro JSON inicial como conteúdo estático; não permite à aplicação escrever no repositório, não sincroniza dispositivos e não suporta edições simultâneas. Para uma base central partilhada seria necessário um serviço backend.

## Publicar no GitHub Pages

O repositório publica a partir da branch `main` através de GitHub Actions. Em **Settings → Pages**, seleciona **GitHub Actions** como origem.

A autenticação é local ao navegador e não protege os dados publicados. Não coloques informação pessoal ou sensível numa publicação pública.
