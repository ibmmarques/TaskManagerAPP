Task Manager
Propósito do Sistema
O Task Manager é uma aplicação web destinada à gestão de tarefas, onde os usuários podem criar, editar, excluir e visualizar tarefas. O sistema oferece funcionalidades simples, porém eficientes, para o controle do status das tarefas (como "Pendente", "Em Progresso" e "Concluída"). Ele visa proporcionar uma interface intuitiva para que os usuários possam organizar suas atividades de forma prática.

Tecnologias Usadas
Back-End
ASP.NET Core 6: Framework robusto para construção da API RESTful.

Entity Framework Core: Para o mapeamento objeto-relacional (ORM), facilitando a comunicação com o banco de dados.

SQL Server: Banco de dados utilizado para armazenamento das informações das tarefas.

MatSnackBar (Material UI): Biblioteca para exibição de notificações no front-end.

C#: Linguagem de programação utilizada no desenvolvimento da API.

Front-End
Angular 14: Framework de front-end utilizado para a criação da interface interativa.

HTML, CSS e Bootstrap: Usados para construção e estilo da interface do usuário.

Router (Angular): Para navegação entre as páginas da aplicação (lista de tarefas, criação/edição de tarefas).

Angular Forms: Para gerenciamento de formulários, incluindo validações e envio de dados para a API.

Como Instalar e Usar
Requisitos:
.NET SDK 6 ou superior

Node.js(para rodar o front-end Angular)

SQL Server (ou outro banco de dados configurado)

1. Clonando o Repositório
bash
git clone https://github.com/seu-usuario/task-manager.git
cd task-manager
2. Configuração do Back-End (API)
Navegue até a pasta do back-end (Backend/TaskManagerApi). Restaure as dependências do projeto:

bash
dotnet restore
Execute a aplicação:

bash
dotnet run
O back-end será executado na URL padrão https://localhost:5001, onde a API ficará disponível.

3. Configuração do Front-End (Angular)
Navegue até a pasta do front-end (Frontend/TaskManagerApp). Instale as dependências do Angular:

bash
npm install
Execute o servidor de desenvolvimento:

bash
ng serve
O front-end será executado na URL padrão http://localhost:4200.

4. Acessando o Sistema
Abra o navegador e acesse o endereço do front-end: http://localhost:4200. O sistema estará disponível para uso, podendo gerenciar suas tarefas diretamente através da interface.

5. Banco de Dados
Certifique-se de que o SQL Server esteja configurado e acessível. O back-end se conecta ao banco de dados definido em appsettings.json, que contém a string de conexão do banco de dados.

Melhorias e Próximas Features
Animações e UI: Atualmente, as animações foram desabilitadas para evitar erros com a configuração de animações no Angular Material. A próxima melhoria será integrar animações de transição e interatividade para melhorar a experiência do usuário.

Autenticação e Autorização: Planeja-se adicionar autenticação de usuários com JWT (JSON Web Tokens), permitindo o gerenciamento de tarefas privadas e controle de acesso.

Persistência de Estado: A inclusão de um sistema de persistência de estado das tarefas para melhorar a experiência do usuário, especialmente no caso de falhas de rede.

Filtros Avançados: Implementar filtros adicionais para visualização das tarefas (ex: por data de criação ou conclusão).

Correções Futuras
Correção de Animações: O erro relacionado ao uso de animações do Angular Material foi identificado, mas as animações estão temporariamente desabilitadas. Vamos revisar as dependências de animações e garantir que as configurações corretas estejam presentes para permitir sua reativação sem erros.

Melhorias no Layout: Embora a aplicação seja funcional, o design pode ser melhorado para garantir maior responsividade e adaptabilidade para diferentes dispositivos.
