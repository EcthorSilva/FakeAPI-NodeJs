# Fake API em NodeJs 

_Aula 9 - Introdução a Rest API com Node JS_

## Comandos usados

**Criar o arquivo packege**

```
npm init -y
```

**Instalando e configurando o [JSON Server](https://github.com/typicode/json-server) no projeto**

```
npm install json-server
```

Após instalar o Json Server precisamos criar um arquivo chamado **db.json** com os seguintes dados: 

```
{
  "posts": [
    { "id": 1, "title": "json-server", "author": "typicode" }
  ],
  "comments": [
    { "id": 1, "body": "some comment", "postId": 1 }
  ],
  "profile": { "name": "typicode" }
}
```

Após isso devemos ir no arquivo **package.json** e adicionar a seguinte linha na parte de scripts: 

```
"start": "json-server --watch db.json",
```

Depois destas configurações é só digitar no terminal: 

```
npm start
```

Se tudo sair como planejado você verá a seguinte informação no terminal: 

![image](https://user-images.githubusercontent.com/13456785/134265212-d28b5f95-748d-4f97-a145-43f622fd5ffc.png)

Após isso é só entrar no link informado como na imagem anterior: 

```
http://localhost:3000
```

### Links Úteis

[Heroku: Cloud Application Platform](https://www.heroku.com/)

### Repositorio de Referencia - Professor Laércio Silva

[lndsilva/restapi_aula_p1](https://github.com/lndsilva/restapi_aula_p1)
