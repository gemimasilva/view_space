python -m venv venv 
venv\Scripts\activate
deactivate
pip install django

// não precisa usar
Set-ExecutionPolicy RemoteSigned
Ctrl + c  no terminal serve para pararo servidor

// pip freeze ( para ver qual versão estamos usando )
pip freeze > requirements.txt

django-admin help
(criar o projeto)
django-admin startproject setup .(criar o projeto)
 (para começar um projeto precisamos usar este comando).

python manage.py runserver (rodar o servidor pela primeira vez)
(quando queremos visualizar alguma coisa  ou quando queremos que ele esteja no ar)

As configurações relacionadas ao idioma da aplicação ficam em "setup > settings.py".Vamos abri-lo e apertar "Ctrl + B" e "Ctrl + J", para que ele minimize e possamos visualizar melhor o seu funcionamento.

 "LANGUAGE_CODE" e "TIME_ZONE" para mudar o pais e o horário do codigo em pempo real (106-107)
 trocaremos o 'en-us inglês dos estados unidos por 'pt-br' português do brasil
 
 Ctrl + j abri o terminal

 pip install python-dotenv
 SECRET_KEY = str(os.getenv('SECRET_KEY'))
 git init
 git add .