# BookStore 📚

Projeto desenvolvido com foco no **estudo de Spring Data JPA**, utilizando operações básicas com entidades e relacionamentos em um contexto de livraria.

> 🎯 Este repositório **não foca em desenvolvimento de API REST** completa, mas sim no uso do **Spring Data JPA** para persistência de dados.

---

## 🔗 Referência de estudo

Estudei através do vídeo no YouTube:  
[Spring Boot + Spring Data JPA - Livro e Relacionamentos](https://www.youtube.com/watch?v=Ca30sv9EbLo)

---

## 🧰 Tecnologias utilizadas

- ☕ **JDK 17**
- 📦 **Maven**
- 🧠 **Spring Boot** + **Spring Data JPA**
- 🐘 **PostgreSQL** (via **PgAdmin**)
- 📬 **Postman** (para testar as requisições)
- 💡 **IntelliJ IDEA** (IDE)

---

## 🔄 Requisições testadas

### ✅ GET  
Listar recursos cadastrados.

**Endpoint:** [http://localhost:8080/bookstore/books](http://localhost:8080/bookstore/books)


### ✅ POST  
Cadastro de novo livro com publisher e autores:

**Endpoint:** [http://localhost:8080/bookstore/books](http://localhost:8080/bookstore/books)

```json
{
  "title": "Domain Driven Design",
  "publisherId": "f725d849-7e6a-47d4-a70b-9509c7d15b92",
  "authorIds": ["2c34bc4a-ad18-4807-9fa0-c46f7b86cbd2"],
  "reviewComment": "Reunindo práticas de design e implementação..."
}
```


### ✅ DELETE  
Remoção de recursos por ID.

**Endpoint:** [http://localhost:8080/bookstore/books](http://localhost:8080/bookstore/books/{id})

---

## 📝 Observações

- O foco principal do projeto é a prática com **relacionamentos entre entidades**, como: `@OneToMany`, `@ManyToOne`, `@ManyToMany`, etc.
- A modelagem e os testes foram feitos localmente com dados fictícios.
- O projeto não possui tratamento completo de erros, validações, DTOs ou arquitetura avançada — intencionalmente, para focar no uso do JPA.

---
