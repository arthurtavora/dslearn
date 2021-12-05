# DSLearn
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/arthurtavora/dslearn/blob/main/LICENSE)

## Visão geral do sistema (Ainda em desenvolvimento)

DSLearn é uma aplicação full stack web que venho desenvolvendo durante o módulo [Spring-React](https://s3.sa-east-1.amazonaws.com/educandoweb.com.br/bds/bootcamp-spring-react-devsuperior-ementa.png "Ementa Spring-React") da instituição de ensino [DevSuperior](https://devsuperior.com.br/ "Site da DevSuperior").

O sistema consiste em uma plataforma de ensino que mantém informações de cursos, suas turmas e alunos, bem como um fórum para perguntas e respostas sobre os conteúdos do curso.

Os atores do sistema podem ser alunos e professores. Há também usuários administradores, que são os únicos autorizados a cadastrar cursos e turmas.
Um curso é composto de vários “recursos”, que são grupos de conteúdos.

Estes recursos podem ser trilhas de aprendizado, bônus, links externos, e o próprio fórum de perguntas e respostas do curso. Cada recurso pode conter seções, e estas seções por sua vez é que vão conter as aulas, que podem ser conteúdos em vídeo e/ou texto, ou tarefas para serem entregues pelos alunos.

Uma tarefa pode ter um peso, uma data de entrega, um número de questões e a quantidade mínima de acertos necessários para ser aceita. 

Quando um aluno entrega a tarefa, esta fica aguardando pelo feedback do professor, e ela pode ser aceita ou rejeitada.

## Modelo conceitual
![Modelo Conceitual](https://github.com/arthurtavora/dslearn/blob/main/modelo-conceitual.png)

# Tecnologias utilizadas
## Back end
- Back end desenvolvido em camadas lógicas (Controlador REST, Camada de Serviço e Camada de Acesso a dados (Repository), utilizando o padrão DTO para o tráfego de dados)
- Java
- Spring Boot
- JPA / Hibernate
- Maven
- Autenticação e autorização (Spring Security, OAuth 2.0, Token JWT, Autorização de rotas por perfil)

# Como executar o projeto

## Back end
Pré-requisitos: Java 11

```bash
# clonar repositório
git clone https://github.com/arthurtavora/dslearn.git

# entrar na pasta do projeto back end
cd backend

# executar o projeto
./mvnw spring-boot:run
```

