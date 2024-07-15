# Portal de campanhas de gamificação

Este projeto teve a finalidade de criar um portal de campanhas de gamificação onde administradores podem gerenciar campanhas e corretores podem participar dos desafios, porém somente a parte de cadastro foi finalizada. O site foi criado com django e as informações cadastrais são salvas no SQLite.


<p align="center">
    <img src="https://imgur.com/PqyoJs5.png" alt="django0">
</p> 

<p align="center">
    <img src="https://imgur.com/osbyQ8f.png" alt="django1">
</p> 

<p align="center">
    <img src="https://imgur.com/bSIe8tZ.png" alt="django2">
</p> 

## Pré-requisitos

- Python 3.9+

## Bibliotecas

- Django
- Bootstrap
- SQLite

## Funcionalidades:

- Cadastrar novos usuários com nome e idade.
- Listar todos os usuários cadastrados em uma tabela.
- Salvar os dados em um banco SQLite.

## Código

### Entrar na pasta do projeto

cd projeto django 1

### Criação do aplicativo

python manage.py startapp app_cad_usuarios

Observação: Adicione app_cad_usuarios em INSTALLED_APPS no arquivo settings.py do projeto.

### Entrar na pasta do aplicativo

cd app_cad_usuarios

Sequência de criação

    Criar a rota (urls.py).
    Criar a lógica da view (views.py).
    Criar o template HTML (home.html).

Configuração da rota inicial

No arquivo urls.py em projeto_cad_usuarios/projeto_cad_usuarios/urls.py, adicione a rota para a página inicial.
Criação da função de view inicial

No arquivo views.py em app_cad_usuarios/views.py, crie a função home.
Criação do template home.html

Em app_cad_usuarios/templates/usuarios, crie o arquivo home.html.

### Visualização do projeto e estilização

python manage.py runserver

Integre um Navbar do Bootstrap para compor a página inicial e utilize formulários para entrada de dados.

No formulário em home.html, inclua o token CSRF:

{% csrf_token %}

### Configuração das views de cadastro

Integre os dados do formulário ao banco de dados.

### Migrations

python manage.py makemigrations
python manage.py migrate

### Construção da página usuarios.html

Crie a visualização dos usuários cadastrados.

### Criação de um template base

Em app_cad_usuarios/templates/usuarios/base.html, crie um template base para reaproveitar componentes Bootstrap.

### Uso

No terminal:

python manage.py runserver

No navegador:

http://127.0.0.1:8000





