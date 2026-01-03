# Caixa Eletronico - Dart Console Application

Aplicacao de terminal em Dart que simula um caixa eletronico com funcionalidades de deposito, saque, consulta de saldo e extrato.

## Sobre o Projeto

Este projeto foi desenvolvido como um desafio de programacao com foco em:

- Arquitetura limpa e separacao de responsabilidades
- Boas praticas de programacao (SRP, Encapsulamento)
- Tratamento avancado de erros
- Codigo testavel e de qualidade de producao

## Funcionalidades

- **Deposito**: Adiciona valores a conta com validacao
- **Saque**: Retira valores com verificacao de saldo disponivel
- **Consulta de Saldo**: Exibe o saldo atual
- **Extrato**: Lista todas as transacoes com tipo, valor e data/hora
- **Encerramento**: Finaliza com resumo da sessao

## Pre-requisitos

- [Dart SDK](https://dart.dev/get-dart) versao 3.10.4 ou superior

Para verificar se o Dart esta instalado:

```bash
dart --version
```

## Como Baixar o Projeto

### Opcao 1: Clonar via Git

```bash
git clone https://github.com/Leankar-dev/dart_application_1.git
```

### Opcao 2: Baixar ZIP

1. Acesse https://github.com/Leankar-dev/dart_application_1
2. Clique no botao verde "Code"
3. Selecione "Download ZIP"
4. Extraia o arquivo no local desejado

## Instalacao

Apos baixar o projeto, navegue ate a pasta e instale as dependencias:

```bash
cd dart_application_1
dart pub get
```

## Como Executar

Execute o arquivo principal da aplicacao:

```bash
dart run lib/desafio_caixa_eletronico/resolucao/resolucao.dart
```

Ou, se houver um entrypoint em `bin/`:

```bash
dart run
```

## Estrutura do Projeto

```
dart_application_1/
├── lib/
│   └── desafio_caixa_eletronico/
│       ├── desafio.md          # Descricao do desafio
│       └── resolucao/
│           └── resolucao.dart  # Implementacao da solucao
├── test/                       # Testes unitarios
├── pubspec.yaml                # Dependencias do projeto
└── README.md
```

## Menu da Aplicacao

```
1 - Realizar deposito
2 - Realizar saque
3 - Mostrar saldo atual
4 - Exibir extrato
5 - Sair do programa
```

## Regras de Negocio

| Operacao | Validacoes |
|----------|------------|
| Deposito | Valor deve ser maior que zero |
| Saque | Valor maior que zero e saldo suficiente |
| Saldo | Operacao de leitura sem alteracao de estado |
| Extrato | Lista transacoes com tipo, valor e data/hora |

## Executar Testes

```bash
dart test
```

## Tecnologias

- **Dart** - Linguagem de programacao
- **Dart SDK 3.10.4+** - Ambiente de execucao

## Autor

Desenvolvido como parte do curso de Dart.

## Licenca

Este projeto e para fins educacionais.
