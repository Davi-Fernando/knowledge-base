# 🧱 Classes

## 📌 O que é?
Resumidamente, a Classe é um molde para criar objetos.

---

## 🧠 Explicação
Ela define atributos e comportamentos.

## Atributos e Operações
São componentes fundamentais para as classes na POO, utilizamos eles para modelar de forma mais precisa um objeto do mundo real em um sistema. Eles definem o que um objeto tem (Atributos) e o que um objeto faz (Operações) (FOWLER, 2011)<br>

- Atributos -> São as características de um objeto, ou seja, váriaveis que armazenam as propriedades de um objeto e descrevem o estado do objeto em um dado momento (FOWLER, 2011). Por exemplo numa classe "Livro" teremos os atributos título, autor e ano de publicação, essas propriedades aparecerão nas instâncias da classe "Livro".

A seguir, um exemplo em python da definição de atributos de uma classe:

```python
class Livro:
    def __init__(self, titulo, autor, anoPublicacao):
        self.titulo = titulo
        self.autor = autor
        self.anoPublicacao = anoPublicacao
#python
```
Como no caso citado acima, temos a classe "Livro" com os atributos título, autor e ano de publicação.

- Operações ou Métodos -> São as ações que os objetos executam, permitindo manipular atributos de uma classe e dizer o que o objeto fará, por exemplo:

```python
class Livro:
    def __init__(self, titulo, autor, anoPublicacao):
        self.titulo = titulo
        self.autor = autor
        self.anoPublicacao = anoPublicacao

#Método da classe Livro:
    def exibir_dados(self):
        print(f"Título: {self.titulo}")
        print(f"Autor: {self.autor}")
        print(f"Ano de Publicação: {self.anoPublicacao}")
#python
```

No caso citado acima, utilizamos o método "exibir_dados" para imprimir os valores dos atributos da classe, sendo esses atributos título, autor e ano de publicação.<br>
Dessa forma percebemos que é possível, utilizando atributos e métodos(operações), trazer um objeto do mundo real, o livro, para um sistema.

---

## ⚠️ Pontos importantes
- Classe ≠ objeto
- Nome deve ser claro
- Nome começa com letra maiúscula
- Segue a mesma regra para nomenclatura de variáveis
- Atributos e Métodos devem ser bem definidos para não impactar em outros elementos do sistema

---

## ❌ Erros comuns
- Confundir classe com instância

---

## 🔗 Conexões
📄[Objetos](objetos.md)

---

## 🚀 Aplicação prática
1. Modelar usuários
2. Criar entidades de sistema

---

## 💡 Insight

Classes são como plantas de uma casa.

---

## 💻 Exemplo

```python
#Classe pessoa
class Pessoa:
    #Atributos nome e cpf
    def __init__(self, nome, cpf):
        self.nome = nome
        self.cpf = cpf
    #Método exibir_dados
    def exibir_dados:
        print(f"O CPF {self.cpf} pertence a {self.nome}")
```
