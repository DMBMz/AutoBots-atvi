# AutoBots - Gestão de Manutenção Veicular (ATVI)

Projeto desenvolvido para a disciplina de **Desenvolvimento Web III** da FATEC, sob orientação do Prof. Dr. Eng. Gerson Penha. Trata-se de um microsserviço Spring Boot focado na gestão de cadastros de clientes, endereços, telefones e documentos para lojas de manutenção veicular.

---

## 🐣 Easter Egg

* **EasterEgg:** `"EasterEgg: Oi Prof. Gerson :) "`
* **Localização no Código:** Declarado no arquivo `AutomanagerApplication.java` e linha 33 exibido no console do servidor durante a inicialização do Spring Boot.

---

## 🛠️ Tecnologias Utilizadas

* **Java**: JDK 17 ou superior
* **Framework**: Spring Boot
* **Persistência de Dados**: Spring Data JPA / H2 Database (Banco em memória)
* **Gerenciador de Dependências**: Maven
* **IDE Recomendada**: Eclipse / Spring Tools Suite (STS) / VS Code

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
* Java JDK instalado (versão 17 ou superior).
* Git instalado.

### Passo a Passo

1. **Clonar o Repositório**
   ```bash
   git clone [https://github.com/DMBMz/AutoBots.git](https://github.com/DMBMz/AutoBots.git)
   
   git switch atv-i


   ### Compilar e Executar a Aplicação

**Via Terminal (Maven Wrapper):**

```bash
./mvnw spring-boot:run

```

*(No Windows PowerShell: `.\mvnw.cmd spring-boot:run`)*

**Via IDE (Eclipse / STS / VS Code):**

* Importe o projeto como **Existing Maven Project**.
* Localize a classe principal `com.autobots.automanager.AutomanagerApplication.java`.
* Execute como **Java Application** ou **Spring Boot App**.

### Verificação no Startup

Ao iniciar a aplicação com sucesso, o console exibirá a mensagem de confirmação do Easter Egg:

```text
EasterEgg: Oi Prof. Gerson :) 

```

---

### 📌 Endpoints da API (CRUD de Cliente)

A aplicação estará rodando no endereço base: `http://localhost:8080` ou `http://localhost:8080/h2-console`

| Método | Endpoint | Descrição |
| --- | --- | --- |
| `GET` | `/cliente/clientes` | Lista todos os clientes cadastrados. |
| `GET` | `/cliente/{id}` | Busca um cliente específico pelo ID. |
| `POST` | `/cliente/cadastro` | Cadastra um novo cliente com seus dados relacionais. |
| `PUT` | `/cliente/atualizar` | Atualiza os dados de um cliente existente. |
| `DELETE` | `/cliente/excluir/{id}` | Remove um cliente pelo ID. |
