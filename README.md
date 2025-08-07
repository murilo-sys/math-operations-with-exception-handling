# 📐 Math Operations with Exception Handling

Este projeto é uma API REST feita com **Spring Boot** que realiza operações matemáticas básicas (adição, subtração, multiplicação, divisão, média e raiz quadrada) com **tratamento de exceções personalizado**, garantindo respostas claras e estruturadas para erros.

---

## 🚀 Funcionalidades

- 📤 Recebe requisições com dois números via URL.
- 🧠 Converte e valida se os números são realmente válidos.
- ⚠️ Retorna mensagens claras de erro para operações inválidas ou divisões por zero.

---

## 🔧 Tecnologias Utilizadas

- Java 17+
- Spring Boot
- Maven
- REST API
- Manipulação de Exceções
- Arquitetura em camadas

---

## 🛠️ Endpoints Principais

| Método | Endpoint                      | Descrição                         |
|--------|-------------------------------|-----------------------------------|
| GET    | `/sum/{num1}/{num2}`          | Soma dois números                 |
| GET    | `/sub/{num1}/{num2}`          | Subtrai o segundo do primeiro     |
| GET    | `/mult/{num1}/{num2}`         | Multiplica dois números           |
| GET    | `/div/{num1}/{num2}`          | Divide o primeiro pelo segundo    |
| GET    | `/avg/{num1}/{num2}`          | Calcula a média entre dois números|
| GET    | `/sqrt/{num}`                 | Retorna a raiz quadrada do número |

---

## ⚠️ Tratamento de Erros

Exemplos de exceções personalizadas tratadas:

- Quando um valor não é numérico:  
  ```json
  {
    "timestamp": "2025-08-06T20:00:00",
    "message": "Por favor, informe um valor numérico!",
    "details": "uri=/sum/a/2"
  }
