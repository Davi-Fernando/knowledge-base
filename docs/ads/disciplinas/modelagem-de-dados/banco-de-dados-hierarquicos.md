## 🪖 Banco de Dados Hierarquicos
  É um modelo de banco de dados onde as informações são organizadas em forma de árvore (hierarquia).

👉 Pense como uma estrutura de pastas no computador:

```
Empresa
 ├── Departamento
 │    ├── Funcionário
 │    ├── Funcionário
 │
 ├── Departamento
      ├── Funcionário
```
<br>
  Ele foi um dos primeiros modelos porque os discos antigos armazenavam dados de forma sequencial e era mais fácil organizar os dados seguindo uma estrutura fixa. Ou seja, a estrutura do banco seguia a forma física de armazenamento
- Existe um nível superior (raiz)
- E níveis abaixo, ligados em forma de pai → filho

---

## 📌 Conceitos principais

### 1. Registro
  É como se fosse uma “linha” com informações sobre algo.

✔ Exemplo:

- Um registro de cliente
- Um registro de funcionário
💡 Equivale a uma linha em tabela (no modelo relacional)


### 2. Tipo de registro
Conjunto de registros iguais.

✔ Exemplo:

- Todos os funcionários
- Todos os departamentos

💡 Equivale a uma tabela

### 3. Relacionamento pai-filho
Esse é o coração do modelo.

👉 Funciona assim:

- Um registro pai pode ter vários filhos
- Um filho só pode ter um único pai

✔ Exemplo:

- Departamento (pai)
- Funcionários (filhos)

## ⚠️ Pontos importantes
- A estrutura é em forma de árvore (hierarquia), com níveis bem definidos.
- Existe sempre a relação pai → filho (um-para-muitos).
- Cada registro filho só pode ter um único pai.
- A navegação nos dados geralmente segue caminhos fixos (da raiz para baixo).

---

## ❌ Erros comuns
- Achar que um registro pode ter mais de um pai (isso não é permitido).
- Usar esse modelo para cenários com muitos-para-muitos (N:N).
- Confundir registros com tabelas sem entender a limitação estrutural.
- Ignorar a rigidez do modelo ao tentar representar situações complexas.

---

## 🔗 Conexões
📄[Banco de Dados](bancodedados.md)

---

## 🚀 Aplicação prática
1. Estrutura organizacional de empresas (empresa → setores → funcionários).
2. Sistemas antigos de arquivos e diretórios (como estrutura de pastas).
3. Sistemas onde os dados seguem uma hierarquia fixa (ex: classificação de produtos).

---

## 💡 Insight
No modelo hierárquico:

Um pai pode ter vários filhos, mas um filho NÃO pode ter vários pais.

Isso é chamado de:

➡️ relacionamento 1:N (um para muitos)
