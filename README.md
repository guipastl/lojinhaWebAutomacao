# Lojinha Web Automação
Esse é um repositório que contém a automação de alguns testes Web de um software denominado Lojinha Web. Os sub-tópicos abaixo descrevem algumas decisões tomadas na estruturação do projeto.

## Tecnologias Utilizadas
- Java
  https://www.oracle.com/java/technologies/javase/jdk18-archive-downloads.html
- JUnit
  https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-engine/5.8.0-M1
- WebDriver
  https://mvnrepository.com/artifact/org.seleniumhq.selenium/selenium-java/4.1.4
- Maven
  https://maven.apache.org/

## Testes Automatizados
Testes para validar as partições de equivalência relacionadas ao valor do produto na Lojinha Web, que estão vinculados diretamente à regra de negócio que diz que o valor do produto deve estar entre R$ 0,01 e R$ 7.000,00

## Notas Gerais
- Sempre utilizamos a anotação Before Each para abrir o navegador, maximizar a tela, definir um tempo de espera padrão e navegar para a página da Lojinha Web.
- Para facilitar a criação e controle, armazenamos os dados que são enviados para a Lojinha Web através do uso da classe de teste.
- Utilizamos o modelo de Page Object para organizar as diferentes delas da Lojinha Web.
- Nesse projeto fazemos uso do JUnit 5, o que nos dá a possibilidade de usar a anotação DisplayName para dar descrições em português para nossos testes.