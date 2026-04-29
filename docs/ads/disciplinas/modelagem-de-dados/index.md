# 🎲 Modelagem de Dados

## 📌 O que é?
  Modelagem de dados é o processo de definir como os dados serão estruturados, organizados e relacionados dentro de um sistema. Ela descreve quais informações serão armazenadas, como elas se conectam e quais regras devem ser seguidas.
  Em outras palavras, a modelagem de dados é o processo de transformar o mundo real em uma estrutura organizada de dados, que depois será implementada em um banco gerenciado por um SGBD e usado por aplicações.

---

## ❗Importância

A modelagem de dados é fundamental porque:

- Garante organização e consistência dos dados
- Facilita o desenvolvimento e a manutenção do sistema
- Reduz redundância e evita inconsistências
- Melhora o desempenho no acesso às informações
- Serve como base para bancos de dados e aplicações

---

## 1. Banco de Dados

- É uma coleção organizada e lógica de dados que possuem um signifcado. Dados soltos aleatoriamente, sem algum tipo de relacionamento com elementos e contexto, não é um banco de dados.
- É criado, projetado e preenchido com valores de dados para atender a um propósito específico, contendo um conjunto predefinido de usuários e aplicações.
- Representa uma parte do mundo real, chamada minimundo; qualquer modificação realizada no minimundo reflete-se automaticamente no banco de dados.

## 2. Níveis de visão de dados
  Para Machado (2020, p. 18-20), 3 níveis de visão de dados devem ser considerados para modelar um banco de dados. São eles:

- Modelo conceitual: É a primeira etapa, descreve a realidade do ambiente do problema (o mundo real), não se preocupa com os aspectos da tecnologia e foca no que existe (os principais dados e seus relacionamentos). Geralmente é feito com diagramas (tipo DER)
- Modelo lógico: Define como será a organização dos dados, o tipo de banco de dados (geralmente relacional). Determinando as tabelas, colunas e relacionamentos. É mais técnico.
- Modelo físico: É a implementação real do que foi analisado e determinado, como os dados serão armazenados no banco. Geralmente utilizado o MySQL, PortegreSQL e etc.

## 3. SGBD (Sistema Gerenciador de Banco de Dados)
  É o software que gerencia/controla o banco de dados, por exemplo:

- MySQL
- PostgreSQL
- Oracle

  Tendo a função de armazenar os dados, permitir consultas, controlar o acesso e abstrair a complexibilidade técnica.

---

## 😁 Vantagem:
- Facilita a organização e compreensão dos dados
- Reduz erros e inconsistências no sistema
- Torna a manutenção e evolução do sistema mais simples

## 😒 Desvantagem:
- Pode demandar tempo no início do projeto
- Exige conhecimento técnico para modelar corretamente
- Mudanças posteriores podem ser trabalhosas se a modelagem inicial for ruim


---

## 💡 Insight
- Uma boa modelagem economiza muito mais tempo do que ela consome
- Pensar nos dados antes do código evita retrabalho
- Modelagem bem feita é a base de sistemas escaláveis e eficientes

---

## 🧠 Estrutura da disciplina

📄 [Banco de Dados](bancodedados.md)<br>



---

## 🚀 Aplicações reais
- Projetos de bancos de dados (como sistemas bancários, e-commerce e redes sociais)
- Desenvolvimento de APIs e sistemas backend
- Estruturação de dados para análise (BI, Data Science e Machine Learning)
