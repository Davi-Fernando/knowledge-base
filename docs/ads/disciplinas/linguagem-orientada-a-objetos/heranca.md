# 🧱 Herança

## 📌 O que é?
É o pilar que permite que uma classe herde métedodos e atributos de outra classe.

---

## 🧠 Explicação
A herança permite reutilizar código e criar relações entre classes. Pense em uma classe base chamada Animal, que possui características gerais como nome e métodos como fazer_som(). A partir dela, podemos criar classes mais específicas como Cachorro e Gato, que herdam essas características, mas também podem ter comportamentos próprios.

Isso evita repetição de código e ajuda a organizar melhor o sistema.

---

## ⚠️ Pontos importantes
- Promove reutilização de código
- Representa uma relação do tipo "é um" (ex: Cachorro é um Animal)
- Classes filhas podem sobrescrever métodos da classe pai
- Pode adicionar novos atributos e métodos nas subclasses

---

## ❌ Erros comuns
- Usar herança quando deveria usar composição
- Criar hierarquias muito complexas e difíceis de manter
- Sobrescrever métodos sem necessidade
- Não usar super() corretamente

---

## 🔗 Conexões
Relacionado com: Polimorfismo, Encapsulamento

---

## 🚀 Aplicação prática
1. Criar classes base genéricas (ex: Veiculo, Funcionario)
2. Criar subclasses específicas (ex: Carro, Moto, Gerente, Estagiario)
---

## 💡 Insight
Herança não é só reutilizar código — é modelar corretamente o mundo real.
Se a relação “é um” não fizer sentido, provavelmente herança não é a melhor escolha.


---

## 💻 Exemplo

```python
class Animal:
    def __init__(self, nome):
        self.nome = nome

    def fazer_som(self):
        print("O animal faz um som")


class Cachorro(Animal):  # herda de Animal
    def fazer_som(self):  # sobrescrita de método
        print("O cachorro late")


class Gato(Animal):
    def fazer_som(self):
        print("O gato mia")


# Uso
animal = Animal("Genérico")
cachorro = Cachorro("Rex")
gato = Gato("Mimi")

animal.fazer_som()
cachorro.fazer_som()
gato.fazer_som()
```
