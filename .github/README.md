# demo-springboot

<p align="center">
  <img alt="demo-springboot" title="demo-springboot" src="/.github/logo.png" />
</p>

<p align="center">
  <a href="#-tecnologias">Tecnologias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-projeto">Projeto</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-como-executar">Como executar</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-como-consultar-o-banco-h2">Consultar Banco H2</a>
</p>

<p align="center">
  <img src="https://img.shields.io/static/v1?label=Youtube&message=@eduardodsr&color=8257E5&labelColor=000000" alt="@eduardodsr" />
  <img src="https://img.shields.io/static/v1?label=Tipo&message=Tutorial&color=8257E5&labelColor=000000" alt="Tutorial" />
</p>

---

## ✨ Tecnologias

Esse projeto foi desenvolvido com as seguintes tecnologias:

- [Spring Boot](https://spring.io/projects/spring-boot)
- [Spring Web](https://docs.spring.io/spring-framework/reference/web/webmvc.html)
- [Spring Data JPA](https://spring.io/projects/spring-data-jpa)
- [H2](http://www.h2database.com/html/main.html)

---

## 💻 Projeto

Esse projeto foi elaborado baseado [nesse vídeo](https://youtu.be/Hwqb12zPT1U), que demonstra como funciona o Spring Boot em apenas 10 minutos!

---

## 🚀 Como executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/eduardodsr/meu-demo-springboot.git

Abra o projeto em qualquer IDE Java.
Execute o projeto Spring Boot.
Você poderá consultar as demos cadastradas no banco em: 🔗 http://localhost:8080/demo/1

🗄️ Como consultar o banco de dados H2
O Spring Boot permite acessar o H2 Database através de um console web. Para visualizar e consultar os dados diretamente no banco, siga os passos abaixo:

1️⃣ Certifique-se de que o H2 Console está ativado
No arquivo application.properties, garanta que as seguintes configurações estão presentes:

```bash
# Habilitar o console web do H2
spring.h2.console.enabled=true
spring.h2.console.path=/h2-console

# Configuração do banco de dados H2
spring.datasource.url=jdbc:h2:file:./data/testdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=
```

<br>

2️⃣ Acesse o Console Web do H2
Após iniciar a aplicação Spring Boot, abra o navegador e acesse:

🔗 http://localhost:8080/h2-console

Preencha os seguintes dados para conexão:

```bash
JDBC URL: jdbc:h2:file:./data/testdb
Username: sa
Password: (deixe em branco)
```
Clique em "Connect" para acessar o banco de dados.

<br>

3️⃣ Consultar dados no H2
Depois de conectado, execute consultas SQL no banco.
Exemplo:

```sql
SELECT * FROM demo;
```

Isso listará todas as entradas cadastradas na tabela DEMO.

Caso queira buscar um registro específico, use:

```sql
SELECT * FROM demo WHERE ID = 1;
```
