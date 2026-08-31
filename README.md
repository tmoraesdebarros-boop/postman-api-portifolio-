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

<img width="601" height="418" alt="Registro" src="https://github.com/user-attachments/assets/35373848-d02a-4d6d-8470-294c32e993fa" />

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


<img width="596" height="419" alt="Login" src="https://github.com/user-attachments/assets/f9960fc7-bd33-418a-ac84-ca3ba3c442a6" />

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

<img width="601" height="420" alt="Update" src="https://github.com/user-attachments/assets/4e95f098-d533-4a31-b519-7be611557bf1" />


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

<img width="607" height="414" alt="Follow" src="https://github.com/user-attachments/assets/66e9f0fb-0aa2-4ad6-8990-077282e97409" />


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

<img width="590" height="421" alt="Unfollow" src="https://github.com/user-attachments/assets/898ffdec-733d-416d-943c-8f5b9d2bfb57" />




## 📋 Resumo dos testes

| Requisição    | Método | Funcionalidade           |
| ------------- | ------ | ------------------------ |
| Registration  | POST   | Cadastro de usuário      |
| Login         | POST   | Autenticação             |
| Update User   | PUT    | Atualização de usuário   |
| Follow User   | POST   | Seguir usuário           |
| Unfollow User | DELETE | Deixar de seguir usuário |

