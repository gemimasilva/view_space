python -m venv venv 
venv\Scripts\activate
deactivate
pip install django

// não precisa usar
Set-ExecutionPolicy RemoteSigned
Ctrl + c  no terminal serve para parar o servidor

// pip freeze ( para ver qual versão estamos usando )
pip freeze > requirements.txt

django-admin help
(criar o projeto)
django-admin startproject setup .(criar o projeto)
 (para começar um projeto precisamos usar este comando).

python manage.py runserver (rodar o servidor )
(quando queremos visualizar alguma coisa  ou quando queremos que ele esteja no ar)

As configurações relacionadas ao idioma da aplicação ficam em "setup > settings.py".Vamos abri-lo e apertar "Ctrl + B" e "Ctrl + J", para que ele minimize e possamos visualizar melhor o seu funcionamento.

 "LANGUAGE_CODE" e "TIME_ZONE" para mudar o pais e o horário do codigo em pempo real (106-107)
 trocaremos o 'en-us inglês dos estados unidos por 'pt-br' português do brasil
 --------------------------------------------------------------
 Ctrl + j abri o terminal

 pip install python-dotenv
 SECRET_KEY = str(os.getenv('SECRET_KEY'))
 git init
 git add .
 git commit -m ""
 git remote add origin https://github.com/gemimasilva/view_space.git
 git push origin master

Ctrl + l é para limpar o terminal
 python manage.py
 python manage.py startapp galeria
 

 def index(request):serve para receber requisicão
--------------------------------------------------
 from galeria.views import index 
 path('',index,)
 tag <p> siginica paragrafo(abrir e fechar uma tag <p> o que a pessoa deseja escrever</p>)

  from django.urls import path (dentro do djando Galeria fizemos o import do path)

  criar um arquivo com o nome urls.py dentro da pasta galeria (boa pratica para não se repetir a funçao ou tag path sempre que quiser adiciar uma pagina)
from django.urls import path
from galeria.views import index

include é para incluir
 -----------------------------------------------------------
  Templete (está focado na parte visual do nosso projeto)
criar um arquivo no view-space com o nome tampletes
 [os.path.join(BASE_DIR,'templetes')]

 para conseguirmos renderisar uma pagina sempre passamos de volta a requisicão (request que vai ser sempre o primeiro parámetro) e depois o arquivo que queremos exibir(exemplo inde.html)              return render(request, 'index.html')
==============================================

STATICFILES_DIRS=[](usado para indicar o diretorio para que o django consiga manupular de alguma forma todos os arquivos)

STATIC_ROOT=(ou seja qual é a raiz dos camonos,onde que eu vou pegar esses arquivos estáticos que o django vai de alguma forma manipular todos esses dados e depois ele vai precisar mandar todos esses dados para algum lugar)

python manage.py help
python manage.py collectstatic

="{% static '/ e ao fechar devemos fazer ' %}"

{% load static %}(ajuda a pagina a saber que vai carregar arquivos estáticos)

<a href="{% url 'imagem' %}">

como subir um projeto no git(
git add.
 git commit -m ""
 git push origin master
)



