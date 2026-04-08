# 🧱 Classes

## 📌 O que é?
Resumidamente, a Classe é um molde para criar objetos.

---

## 🧠 Explicação
Ela define atributos e comportamentos.
- Atributos -> São as características de um objeto, por exemplo:

```python
class Livro:
    def __init__(self, titulo, autor, anoPublicacao):
        self.titulo = titulo
        self.autor = autor
        self.anoPublicacao = anoPublicacao

```
No caso citado acima temos a classe livro com os atributos titulo, autor e ano de publicação

- Métododos -> São as ações que os objetos executam, por exemplo:
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
```
No caso citado acima, utilizamos o exemplo de atributos e definimos ações para 
---

## ⚠️ Pontos importantes
- Classe ≠ objeto
- Nome deve ser claro
- Nome começa com letra maiúscula
- Segue a mesma regra para nomenclatura de variáveis

---

## ❌ Erros comuns
- Confundir classe com instância

---

## 🔗 Conexões
Relacionado com: Objetos

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
