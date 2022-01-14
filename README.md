# Atividade 5B11 - API Fake

Está API foi criada inspírada na atividade 5B11.

## Endpoints

Existem 3 endpoints:

### Cadastro
<br/>
Parte da API responsável pelo cadastro do usuário.<br/>
<br/>
POST /register <br/>
<br/>
Que deve ser utilizado no formato: <br/>
{<br/>
    "email": "seu email",<br/>
    "password": "sua senha"<br/>
}<br/>
<br/>
Resposta:<br/>
{<br/>
    "accessToken": "Seu Token",<br/>
    "user": {
    "email": "Seu email",
    "id": SeuID
  }<br/>
}<br/>
<br/>

### Login
<br/>
Parte da API responsável por efetuar o login. <br/>
<br/>
POST /login<br/>
<br/>
Que deve ser utilizado no formato: <br/>
{<br/>
    "email": "seu email",<br/>
    "password": "sua senha"<br/>
}<br/>
<br/>
Resposta:<br/>
{<br/>
    "accessToken": "Seu Token",<br/>
    "user": {
    "email": "Seu email",
    "id": SeuID
  }<br/>
}<br/>
<br/>

### Perfil
<br/>
Parte da API responsável pelo cadastro de informações pessoais do usuário. </br>
<br/>
POST /perfil<br/>
<br/>
Que deve ser utilizado no formato: <br/>
{<br/>
    "name": "seu nome",<br/>
    "age": sua idade,<br/>
    "country": "seu país",<br/>
    "userId": seu id    <br/>
}<br/>
<br/>
Resposta:<br/>
{<br/>
    "name": "seu nome",<br/>
    "age": sua idade,<br/>
    "country": "seu país",<br/>
    "userId": seu id,   <br/>
    "id": ID do perfil   <br/>
}<br/>
<br/>
GET /perfil<br/>
<br/>
Parte da API resposável por retornar os dados pessoáis do usuário (apenas o próprio usuário pode faze-lo). </br>
<br/>
Resposta:<br/>
{<br/>
    "name": "seu nome",<br/>
    "age": sua idade,<br/>
    "country": "seu país",<br/>
    "userId": seu id,   <br/>
    "id": ID do perfil   <br/>
}<br/>
<br/>

### Skills
<br/>
Parte da API responsável pelo cadastro de skills do usuário. </br>
<br/>
POST /skills<br/>
<br/>
Que deve ser utilizado no formato: <br/>
{<br/>
    "name": "seu nome",<br/>
    "age": sua idade,<br/>
    "country": "seu país",<br/>
    "userId": seu id    <br/>
}<br/>
<br/>
Resposta:<br/>
{<br/>
    "userId": seu id,   <br/>
    "skill": "sua skill", <br/>
    "status": "nivel de sua skill (básico, intermediário, avançado, ...) <br/>
}<br/>
<br/>
GET /skills<br/>
<br/>
Parte da API resposável por retornar as skills do usuário (todos podem requisita-las). </br>
<br/>
Resposta:<br/>
{<br/>
    "userId": seu id,   <br/>
    "skill": "sua skill", <br/>
    "status": "nivel de sua skill (básico, intermediário, avançado, ...) <br/>
    "id": ID da skill   <br/>
}<br/>
<br/>
