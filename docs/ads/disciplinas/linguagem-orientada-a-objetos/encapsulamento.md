# 🧱 Encapsulamento

## 📌 O que é?
É o pilar que consiste em proteger os dados de um objeto, controlando o acesso a eles por meio de métodos.

---

## 🧠 Explicação
Encapsulamento significa esconder os detalhes internos de um objeto e permitir acesso a eles apenas de forma controlada. Em vez de acessar atributos diretamente, utilizamos métodos para garantir que as regras do sistema sejam respeitadas.
Por exemplo, em uma conta bancária, o saldo não deve ser alterado diretamente. Em vez disso, usamos métodos como ```depositar()``` e ```sacar()```, que garantem validações antes de modificar o valor.

---

### Modificadores de Acesso
- Público (public): permite que um atributo ou método seja acessado de qualquer classe, seja interna ou externa ao pacote onde foi declarado.
- Protegido (protected): permite que o acesso seja feito apenas dentro do mesmo pacote e por subclasses, mesmo em pacotes diferentes.
- Privado (private): restringe o acesso aos membros da própria classe, não permitindo acesso direto de fora.<br>

Esses modificadores de acesso são usados para proteger a integridade dos dados e garantir que o comportamento dos objetos seja controlado. A seguir um exemplo na linguagem Java:

```java
public class ContaBancaria {

    private double saldo;

    public ContaBancaria(double saldoInicial) {
        this.saldo = saldoInicial;
    }

    public void depositar(double valor) {
        if (valor > 0) {
            saldo += valor;
            System.out.println("Depósito realizado. Saldo atual: R$ " + saldo);
        }
    }

    public void sacar(double valor) {
        if (valor > 0 && valor <= saldo) {
            saldo -= valor;
            System.out.println("Saque realizado. Saldo atual: R$ " + saldo);
        } else {
            System.out.println("Saque inválido.");
        }
    }
 
    public double getSaldo() {
        return saldo;
    }
}
```

---

## ⚠️ Pontos importantes
- Protege os dados contra alterações indevidas
- Controla como os atributos são acessados e modificados
- Usa atributos "privados" (ex: ```__saldo``` em Python)
- Normalmente utiliza métodos getters e setters

---

## ❌ Erros comuns
- Acessar atributos diretamente quando deveriam ser protegidos
- Usar encapsulamento sem necessidade (excesso de getters/setters)
- Não validar dados dentro dos métodos
- Achar que apenas usar ```__``` já resolve todos os problemas de segurança

---

## 🔗 Conexões
Relacionado com: Abstração, Herança, Polimorfismo

---

## 🚀 Aplicação prática
1. Proteger atributos sensíveis (ex: saldo, senha, idade)
2. Criar métodos para validar e controlar alterações nesses dados

---

## 💡 Insight
Encapsulamento não é esconder tudo — é expor apenas o necessário de forma segura.

---

## 💻 Exemplo

A seguir o exemplo mostrado acima, porém em python:

```python
class ContaBancaria:
    def __init__(self, titular, saldo):
        self.titular = titular
        self.__saldo = saldo  # atributo privado

    def depositar(self, valor):
        if valor > 0:
            self.__saldo += valor

    def sacar(self, valor):
        if 0 < valor <= self.__saldo:
            self.__saldo -= valor
        else:
            print("Operação inválida")

    def get_saldo(self):  # getter
        return self.__saldo


# Uso
conta = ContaBancaria("Maria", 1000)

conta.depositar(500)
conta.sacar(200)

print(conta.get_saldo())

# tentativa de acesso direto (não recomendado)
# print(conta.__saldo) -> erro
```
