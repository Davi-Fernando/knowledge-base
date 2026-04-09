# 🧱 Abstração

## 📌 O que é?
Resumidamente, é o processo de ocultar detalhes complexos de um sistema e extrair somente as partes principais.

---

## 🧠 Explicação
Imagine uma “ContaBancaria”: para um cliente, só interessa saber seu saldo e a possibilidade de realizar saques e depósitos. Detalhes internos como o formato dos dados e os processos de segurança ficam ocultos. A abstração permite que o desenvolvedor crie sistemas complexos sem se preocupar com os detalhes em cada nível.

---

## ⚠️ Pontos importantes
- Foca no "o que o objeto faz", não em "como ele faz"
- Reduz a complexidade do sistema
- Facilita manutenção e evolução do código
- Ajuda a criar interfaces mais simples e intuitivas

---

## ❌ Erros comuns
- Confundir abstração com encapsulamento
- Expor detalhes internos desnecessários
- Criar abstrações muito genéricas ou inúteis
- Não definir claramente as responsabilidades da classe

---

## 🔗 Conexões
Relacionado com: Encapsulamento

---

## 🚀 Aplicação prática
1. Criar classes com métodos simples para o usuário (ex: sacar(), depositar())
2. Esconder regras complexas dentro desses métodos (ex: validação de saldo, taxas, segurança)

---

## 💡 Insight
Uma boa abstração faz o código parecer “óbvio”.
Se você precisa explicar demais como usar uma classe, provavelmente a abstração não está boa.

---

## 💻 Exemplo

```python
class ContaBancaria:
    def __init__(self, titular, saldo):
        self.titular = titular
        self.__saldo = saldo  # atributo "privado"

    def depositar(self, valor):
        if valor > 0:
            self.__saldo += valor

    def sacar(self, valor):
        if valor <= self.__saldo:
            self.__saldo -= valor
        else:
            print("Saldo insuficiente")

    def ver_saldo(self):
        return self.__saldo


#Uso da abstração
conta = ContaBancaria("João", 1000)

conta.depositar(500)
conta.sacar(200)

print(conta.ver_saldo())  #O usuário não precisa saber como o saldo é controlado
```
