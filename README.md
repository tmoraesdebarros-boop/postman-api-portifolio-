![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)

# postman-api-portifolio-
## 🧪 API Testing — Postman

Este projeto apresenta testes de API REST realizados utilizando o **Postman**, contemplando diferentes operações de autenticação, gerenciamento de usuários e relacionamento entre usuários.

As requisições foram executadas com o objetivo de validar o comportamento da API, códigos de resposta HTTP, dados retornados e regras funcionais dos endpoints.

---

### 🔹 POST — Registration

**🎯 Objetivo**

Validar o cadastro de um novo usuário por meio da API, verificando se os dados enviados são processados corretamente e se a API retorna a resposta esperada.

**🔧 Método**

```http
POST
```

**📌 Endpoint**

```http
POST /api/users
```

**✅ Validações**

* Status code da resposta;
* Cadastro realizado com dados válidos;
* Estrutura do response body;
* Retorno das informações esperadas;
* Criação correta do usuário.

**📸 Evidência**

```markdown
![POST Registration](evidences/post-registration.png)
```

![POST Registration](evidences/post-registration.png)

---

### 🔹 POST — Login

**🎯 Objetivo**

Validar a autenticação de um usuário previamente cadastrado utilizando credenciais válidas.

**🔧 Método**

```http
POST
```

**📌 Endpoint**

```http
POST /api/users/login
```

**✅ Validações**

* Status code da resposta;
* Autenticação com credenciais válidas;
* Retorno do token de autenticação;
* Estrutura do response body;
* Dados do usuário autenticado.

**📸 Evidência**

login.png

---

### 🔹 PUT — Update User

**🎯 Objetivo**

Validar a atualização dos dados de um usuário existente, verificando se as informações enviadas são processadas e armazenadas corretamente pela API.

**🔧 Método**

```http
PUT
```

**📌 Endpoint**

```http
PUT /api/user
```

**✅ Validações**

* Autenticação da requisição;
* Status code da resposta;
* Atualização correta dos dados;
* Estrutura do response body;
* Conferência das informações atualizadas.

**📸 Evidência**

```markdown
![PUT Update User](evidences/put-update-user.png)
```

![PUT Update User](evidences/put-update-user.png)

---

### 🔹 POST — Follow User

**🎯 Objetivo**

Validar a criação de uma relação de acompanhamento entre o usuário autenticado e outro usuário.

**🔧 Método**

```http
POST
```

**📌 Endpoint**

```http
POST /api/profiles/{username}/follow
```

**✅ Validações**

* Autenticação da requisição;
* Identificação correta do usuário;
* Status code da resposta;
* Criação da relação de follow;
* Retorno dos dados esperados no response body.

**📸 Evidência**

```markdown
![POST Follow User](evidences/post-follow-user.png)
```

![POST Follow User](evidences/post-follow-user.png)

---

### 🔹 DELETE — Unfollow User

**🎯 Objetivo**

Validar a remoção de uma relação de acompanhamento existente entre o usuário autenticado e outro usuário.

**🔧 Método**

```http
DELETE
```

**📌 Endpoint**

```http
DELETE /api/profiles/{username}/follow
```

**✅ Validações**

* Autenticação da requisição;
* Identificação correta do usuário;
* Status code da resposta;
* Remoção da relação de follow;
* Retorno dos dados esperados pela API.

**📸 Evidência**

```markdown
![DELETE Unfollow User](evidences/delete-unfollow-user.png)
```

![DELETE Unfollow User](evidences/delete-unfollow-user.png)

---

## 📋 Resumo dos testes

| Requisição    | Método | Funcionalidade           |
| ------------- | ------ | ------------------------ |
| Registration  | POST   | Cadastro de usuário      |
| Login         | POST   | Autenticação             |
| Update User   | PUT    | Atualização de usuário   |
| Follow User   | POST   | Seguir usuário           |
| Unfollow User | DELETE | Deixar de seguir usuário |

