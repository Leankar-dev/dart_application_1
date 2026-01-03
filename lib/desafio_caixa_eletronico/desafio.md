# 🏧 Desafio de Programação — Caixa Eletrônico em Dart 

## 🎯 Objetivo

Projetar e desenvolver uma aplicação **em Dart**, executada no **terminal**, que simule um **caixa eletrônico robusto**, com foco em **arquitetura**, **boas práticas**, **tratamento avançado de erros**, **testabilidade** e **qualidade de código**.

> ⚠️ **Importante:** Este documento descreve apenas o **desafio técnico**. 

---

## 🧩 Contexto

Você está desenvolvendo o núcleo de um sistema de caixa eletrônico que poderá futuramente evoluir para uma aplicação distribuída (API, mobile ou desktop). Apesar de rodar no terminal, o código deve ser escrito com **qualidade de produção**.

---

## 🛠️ Funcionalidades Obrigatórias

O sistema deve apresentar um menu interativo no terminal com as seguintes opções:

```text
1 - Realizar depósito
2 - Realizar saque
3 - Mostrar saldo atual
4 - Exibir extrato
5 - Sair do programa
```

---

## 📋 Regras de Negócio

### ➕ Depósito

* Solicitar o valor do depósito via terminal.
* Aceitar apenas valores **maiores que zero**.
* Registrar a transação no extrato.
* Atualizar o saldo de forma consistente.

### ➖ Saque

* Solicitar o valor do saque.
* Validar se o valor é **maior que zero**.
* Validar se há **saldo suficiente**.
* Registrar a transação no extrato.
* Não permitir que o saldo fique negativo.

### 💰 Mostrar Saldo

* Exibir o saldo atual de forma clara.
* Garantir que a operação não altere o estado do sistema.

### 📄 Extrato

* Exibir a lista de transações realizadas na sessão.
* Cada transação deve conter:

  * Tipo (Depósito ou Saque)
  * Valor
  * Data/hora

### 🚪 Sair

* Encerrar o programa de forma controlada.
* Exibir um resumo final (saldo e total de transações).

---

## 🧱 Requisitos Arquiteturais

O candidato deve:

* Separar responsabilidades (ex: domínio, serviços, entrada/saída).
* Evitar lógica de negócio diretamente no fluxo de entrada do terminal.
* Utilizar princípios como:

  * **SRP (Single Responsibility Principle)**
  * **Encapsulamento**
* Estruturar o código visando **facilidade de manutenção**.

---

## ⚠️ Tratamento de Erros

O sistema deve tratar adequadamente:

* Entradas inválidas (strings, valores nulos, números mal formatados).
* Opções inexistentes do menu.
* Tentativas de saque inválidas.

As mensagens de erro devem ser **claras**, **consistentes** e **amigáveis**.

---

## 🔁 Fluxo do Programa

* O menu deve rodar em loop controlado.
* O estado da aplicação deve ser preservado durante a execução.
* O encerramento deve ser explícito e previsível.

---

## 🧪 Testabilidade

O código deve ser estruturado de forma que:

* A lógica de negócio possa ser testada **sem depender do terminal**.
* Seja possível criar testes unitários para:

  * Depósitos
  * Saques
  * Validações

> Não é obrigatório escrever os testes, mas a estrutura deve permitir.

---

## 📌 Restrições Técnicas

* Utilizar **Dart puro (console)**.
* Não utilizar interface gráfica.
* Não utilizar banco de dados ou arquivos.
* Persistência apenas em memória.

---

## ⭐ Diferenciais (Opcional)

Itens que contam como diferencial:

* Uso de **enums** para tipos de transação.
* Uso de **classes imutáveis** quando aplicável.
* Logs simples para operações críticas.
* Tratamento centralizado de erros.
* Código preparado para futura persistência.

---

## 🧠 Critérios de Avaliação

Este desafio avalia se o programador:

* Escreve código limpo e bem estruturado
* Aplica boas práticas e princípios de design
* Se preocupa com manutenção e evolução do sistema
* Trata erros de forma elegante
* Demonstra pensamento arquitetural

---

📄 **Fim do Desafio **
