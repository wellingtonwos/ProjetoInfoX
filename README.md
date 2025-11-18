# 🚀 ProjetoInfoX: Sistema de Gestão de OS

![Status do Projeto](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)

O ProjetoInfoX é um sistema de desktop (Java Swing) para o gerenciamento de Ordens de Serviço (OS), Clientes e Usuários. Este projeto foi desenvolvido para aplicar conceitos de programação Java, interface gráfica com Swing, e conectividade com banco de dados (JDBC) MySQL.

---

## 🛠️ Tecnologias Utilizadas

Este projeto foi construído utilizando as seguintes tecnologias:

* **Linguagem:** Java 21
* **Interface Gráfica:** Java Swing
* **Banco de Dados:** MySQL
* **Conectividade:** JDBC (MySQL Connector/J)
* **IDE:** Eclipse (com WindowBuilder) / NetBeans
* **Bibliotecas (JARs):**
    * `rs2xml.jar` (para popular tabelas Swing a partir do `ResultSet`)
    * *(Opcional: JasperReports para relatórios)*

---

## ✨ Funcionalidades Principais

* **Controle de Acesso:** Tela de login com autenticação de usuários no banco de dados.
* **Diferenciação de Nível:** Permissões de acesso diferentes para usuários "admin" e "usuários padrão".
* **CRUD de Usuários:** (TelaUsuario) Cadastro, leitura, atualização e exclusão de usuários do sistema (acessível apenas por administradores).
* **CRUD de Clientes:** (TelaCliente) Gerenciamento completo de clientes, com busca dinâmica por nome.
* **Gestão de OS:** (TelaOS) Emissão, consulta, alteração e exclusão de Ordens de Serviço, com associação a um cliente existente.

---

## 🖥️ Como Executar o Projeto

Para executar este projeto em sua máquina local, siga os passos abaixo:

### 1. Pré-requisitos

* Ter o **Java JDK 21** (ou superior) instalado.
* Ter um servidor **MySQL** local (ex: XAMPP, WAMP ou MySQL Community Server).
* Uma IDE Java (ex: Eclipse ou NetBeans).

### 2. Configuração do Banco de Dados

1.  Crie um banco de dados em seu MySQL chamado **`dbinfox`**.
2.  **Importante:** Você precisará executar o script SQL para criar as tabelas (`tbusuarios`, `tbclientes`, `tbos`). Recomenda-se adicionar este arquivo `.sql` ao repositório.
3.  Abra a classe `br.com.infox.dao.ModuloConexao.java`.
4.  Altere as variáveis `URL`, `USER` e `PASSWORD` para que correspondam às credenciais do seu banco de dados local.

### 3. Configuração das Bibliotecas (JARs)

1.  Baixe o [MySQL Connector/J](https://dev.mysql.com/downloads/connector/j/) (arquivo `.jar`).
2.  Baixe a biblioteca `rs2xml.jar`.
3.  No Eclipse (ou NetBeans), adicione esses arquivos `.jar` ao **Build Path** (Caminho de Construção) do projeto.

### 4. Execução

* A classe principal (Main) que deve ser executada para iniciar o sistema é a `br.com.infox.telas.TelaLogin.java`.

---

## 📸 Telas (Screenshots)

*Tela de Usuário*

**Exemplo: Tela de Login**


**Exemplo: Gestão de Clientes**


---

## 👨‍💻 Autor

* **Wellington Wos**
* **GitHub:** [wellingtonwos](https://github.com/wellingtonwos)
