# 🧱 Polimorfismo
## 📌 O que é?

É o pilar que permite que diferentes objetos respondam de formas diferentes ao mesmo método.

## 🧠 Explicação

Polimorfismo significa “muitas formas”. Na prática, isso quer dizer que podemos usar o mesmo método em objetos diferentes, mas cada um terá um comportamento específico.
Por exemplo, se várias classes possuem o método ```fazer_som()```, cada uma pode implementar esse método de forma diferente. Mesmo assim, podemos tratar todos os objetos de forma uniforme.

## ⚠️ Pontos importantes
- Permite usar a mesma interface para diferentes tipos de objetos
- Está diretamente ligado à herança
- Ocorre principalmente por meio de sobrescrita de métodos (override)
- Torna o código mais flexível e extensível

## ❌ Erros comuns
- Achar que polimorfismo só funciona com herança (também pode ocorrer sem ela)
- Criar métodos com o mesmo nome sem manter consistência de propósito
- Não aproveitar o polimorfismo para simplificar estruturas condicionais

## 🔗 Conexões
Relacionado com: Herança, Encapsulamento, Abstração

## 🚀 Aplicação prática
- Trabalhar com listas de objetos diferentes usando o mesmo método
- Reduzir o uso de vários ```if/else``` baseados em tipo de objeto

## 💡 Insight

Se você está usando muitos ```if tipo == ...```, provavelmente está deixando de usar polimorfismo.

💻 Exemplo
```python
class Animal:
    def fazer_som(self):
        print("O animal faz um som")


class Cachorro(Animal):
    def fazer_som(self):
        print("O cachorro late")


class Gato(Animal):
    def fazer_som(self):
        print("O gato mia")


# Polimorfismo em ação
animais = [Cachorro(), Gato(), Animal()]

for animal in animais:
    animal.fazer_som()  # mesmo método, comportamentos diferentes
```
