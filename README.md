## Sobre o projeto:

Este projeto foi baseado no pinterest, contendo anexo de fotos pra cada usuário, e todos usuários podem ver a foto um do outro na pagina de Feed.
O usuário pode criar sua conta e caso já tenha, o programa vai fazer a verificação dentro da base de dados pra realizar o login. 

### Link do site
[Replica Pinterest](https://replicapinterest-74d74d352cb8.herokuapp.com/)

### Principais Bibliotecas:

Flask, Flask-Login, flask_bcrypt, SQLAlchemy e as criadas

### Explicação da linha de raciocínio:

Primeiramente é criado um super diretório chamado fakepinterest contendo todos arquivos como __init__.py, rotas, formulários, estrutura do banco de dados, e arquivos front html.

__init__.py - é onde o site é ativado por meio do Flask(__name__), assim como a base de dados, chave de segurança e uma pasta que armazena as fotos postadas pelos usuários.

models.py - é a estrutura da base de dados, contém a Classe(Usuario) > usuário tem seu próprio id, username, email, senha e fotos. Classe(Foto) > as fotos também tem id próprio, e o id do usuário que a postou.

forms.py - contém os formulários de login, criar conta os quais tem consulta e validação no banco de dados, além também do formulário anexar foto.

routes.py - vão efetivamente ativar os formulários para o site através do @app.route: homepage para login, criar conta, perfil, e dentro do próprio perfil poderá ver e postar suas fotos, do contrário apenas ver, e por último uma rota para o feed onde está armazenado a foto de todos usuários.

##### As páginas html foram adaptadas para serem dinamicas 





