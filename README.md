# Oficina Mecânica - Banco de Dados Relacional

Projeto desenvolvido como parte do curso **"Análise de Dados"** promovido pela **Randstad** em parceria com a **DIO (Digital Innovation One)**.

Este repositório contém a modelagem e implementação de um banco de dados relacional para gerenciar uma **oficina mecânica**, incluindo o controle de clientes, veículos, ordens de serviço, equipes de mecânicos, peças e serviços.

---

## 📁 Estrutura do Projeto

- README.md – documentação e contexto do projeto
- oficina_model.png – imagem do modelo conceitual
- script_database.sql – script de criação do banco de dados com todas as tabelas, chaves primárias e estrangeiras

---

## 🛠️ Tecnologias Utilizadas

- MySQL
- MySQL Workbench (modelagem e geração do script)
- SQL (DDL)
- Git/GitHub – versionamento e hospedagem do projeto
  
---

## 🧱 Entidades Principais

| Entidade         | Descrição                                          |
|------------------|----------------------------------------------------|
| **cliente**      | Armazena os dados dos clientes                     |
| **veiculo**      | Relacionado a um cliente, contém dados dos carros |
| **ordem_servico**| Registra os serviços realizados em veículos       |
| **equipe**       | Grupos de mecânicos que executam as ordens        |
| **mecanico**     | Mecânicos vinculados a equipes                     |
| **servico**      | Serviços prestados na oficina                      |
| **peca**         | Peças utilizadas nas ordens de serviço            |
| **os_servico**   | Relação entre ordem de serviço e serviços         |
| **os_peca**      | Relação entre ordem de serviço e peças            |

---

## 🔗 Relacionamentos (Cardinalidades)

- Um **cliente** pode possuir **muitos veículos**
- Um **veículo** pode ter **muitas ordens de serviço**
- Uma **ordem de serviço** é executada por **uma equipe**
- Uma **equipe** pode ter **vários mecânicos**
- Uma **ordem de serviço** pode conter **vários serviços** e **várias peças**
- Um **serviço** ou **peça** pode ser utilizado em **várias ordens**

---

## 👩‍💻 Desenvolvido por

Projeto desenvolvido por [Karin] como parte do curso Randstad - Análise de Dados (DIO).

---

##📎 Licença

Este projeto está sob a licença MIT – sinta-se à vontade para usar e adaptar para fins acadêmicos ou profissionais.
