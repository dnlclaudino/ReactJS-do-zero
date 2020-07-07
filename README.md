# Instalar VSCode

 1) Instale o VS Code
    Link:https://code.visualstudio.com/download

# Configurar VSCode
Fonte: Configurando VSCode para Node.js, ReactJS e React Native | Diego Fernandes - https://www.youtube.com/watch?v=c7P03kkrEG8

Abra o VS Code. Clique no ícone do lado esquerdo (Extensões - Ctrl + Shift + E). Instale os temas, plugins e snippets abaixo.
Após isso, copie o arquivo "settings.json" na raiz dos seus projetos. (arquivo no repositório)

    1) Temas
        a) Dracula Theme
        b) Material Icon Theme

    2) Plugins
        a) Color Highlight
        b) dotENV
        c) EditorConfig for VC Code 
            Quando você trabalha com um time de programadores que usam editores diferentes).
            No File Explorer, clique com o botão direto e selecione "generate .editorconfig"
        d) ESLint
            Padroniza o codigo JavaScript quando você trabalha com um time de desenvolvedores
        e) GitLens
            Não faz COMMIT, PULL REQUEST. Para saber qual desenvolvedor é autor de cada linha, se alguma linha dará conflitos para resolvermos.
        f) GraphQL
        g) Live Server
        h) Live Share
            Compartilha terminal, localhost da minha máquina com outro desenvolvedor para testes.
        i) Styled Components
        j) Docker
            Obs: Após instalar o Docker no seu computador.

    3) Snippets
        a) Rocketseat React JS
        a) Rocketseat React Native


# Instalar o NodeJS e NPM

 1) Download Node.JS (12.18.2 LTS) 
    Link:  https://nodejs.org/en/download/
    Download: 

# Instalar Yarn
Para saber mais sobre NPM x YARN, assista: https://www.youtube.com/watch?v=3BPfDo4arHc

1) Na linha de comando, digite: npm install -g yarn

# Instale os componentes para acesso a banco de dados
Crie uma nova pasta no explorer(Ctrl + Shift + E) do VS Code
Execute os comandos abaixo no terminal do VSCode:

1) yarn add express pg pg-hstore sequelize
2) yarn add sequelize-cli -D
   Configure por projeto.
3) yarn add nodemon -D

# Instalar o banco de dados Postgres e client para administração

1) Baixe e instale o Docker
2) Abaixe a imagem do banco de dados Postgre no Docker Hub. Siga as instruções da página: https://docs.docker.com/engine/examples/postgresql_service/
   Crie o docker file e clique com o botão esquerdo sobre ele e depois em "build image" no VSCode. Se você não ver essa opção é porque você não instalou o plugin "Docker" no VS Code.
3) Crie o container do banco de dados
    a) docker run -p 127.0.0.1:5432:5432/tcp --name pg_test sqlnode2-postgres:9.3
    b)  Usuario: docker
        Senha: docker
4) Abaixe a imagem do cliente de banco de dados Postgre no Docker Hub. Siga as instruções da página: https://hub.docker.com/r/dpage/pgadmin4/
    a) Execute: docker pull dpage/pgadmin4
5) Crie o container do cliente de banco de dados
    Obs: Cliente alternativo: https://www.electronjs.org/apps/postbird
    a) Execute: docker run -p 80:80 -e 'PGADMIN_DEFAULT_EMAIL=user@domain.com' -e 'PGADMIN_DEFAULT_PASSWORD=SuperSecret' -d dpage/pgadmin4
    b) Acesse http://localhost:80
    c) Usuário: user@domain.com e Senha: SuperSecret
    d) Configure o PGAdmin para acessar o banco de dados Postgres que já está rodando. Para mais orientações, assista:
         i)  https://www.youtube.com/watch?v=pVinuOO-vis
         ii) https://medium.com/@renato.groffe/postgresql-pgadmin-4-docker-compose-montando-rapidamente-um-ambiente-para-uso-55a2ab230b89
    

***** https://www.youtube.com/watch?v=Fbu7z5dXcRs 
Video em 32m10s

