# 📋 TaskBoard Manager - Java Fundamentals
> Sistema de gerenciamento de tarefas via terminal com persistência em banco de dados.

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)

O Task Board Manager é uma aplicação de console desenvolvida em Java que permite a gestão completa de tarefas através de boards customizáveis. 
O sistema simula um fluxo de trabalho profissional (estilo Kanban) com regras rígidas de movimentação, bloqueio e persistência em banco de dados MySQL.

🚀 Funcionalidades Principais
O sistema é dividido em dois níveis de interação:
1. Gestão de Boards (Menu Principal)
Criar Novo Board: Configuração de colunas personalizadas respeitando as regras de tipo.
Selecionar Board: Entra no modo de edição e movimentação de cards de um board específico.
Excluir Board: Remoção lógica e física do board e seus cards do banco de dados.

2. Operações em Cards (Menu do Board)
Criação de Cards: Título, descrição e data automática.
Movimentação Linear: Cards seguem a ordem das colunas sem pular etapas.
Fluxo de Cancelamento: Atalho direto para a coluna de cancelamento (exceto se o card já estiver finalizado).
Sistema de Bloqueio: Impede movimentações indesejadas, exigindo justificativa para bloquear ou desbloquear.

🏗️ Arquitetura e Tecnologias
O projeto foi estruturado seguindo boas práticas de separação de responsabilidades:
Java SE (JDK 17+): Linguagem principal.
JDBC: Para comunicação com o banco de dados.
MySQL: Persistência robusta de dados.
Padrão DAO (Data Access Object): Isolamento da lógica de persistência.

🚦 Como Executar o Projeto
Pré-requisitos
Java JDK 17 ou superior.
MySQL Server rodando localmente ou em container.
Driver JDBC do MySQL (mysql-connector-j).
