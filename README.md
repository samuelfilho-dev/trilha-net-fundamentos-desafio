# 🚗 Sistema de Estacionamento - DIO

[![.NET](https://img.shields.io/badge/.NET-6.0-512BD4?style=flat-square&logo=dotnet)](https://dotnet.microsoft.com/)
[![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=c-sharp&logoColor=white)](https://docs.microsoft.com/en-us/dotnet/csharp/)
[![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)](LICENSE)

> Sistema de gerenciamento de estacionamento desenvolvido como parte do desafio da trilha .NET Fundamentals da [DIO](https://www.dio.me).

## 📋 Sobre o Projeto

Este projeto implementa um sistema completo para gerenciamento de estacionamento, permitindo o controle de veículos estacionados e o cálculo automático de tarifas baseado no tempo de permanência.

### 🎯 Funcionalidades

- ✅ **Cadastro de Veículos**: Adicionar veículos ao estacionamento através da placa
- ✅ **Remoção de Veículos**: Remover veículos e calcular o valor total a ser pago
- ✅ **Listagem de Veículos**: Visualizar todos os veículos atualmente estacionados
- ✅ **Cálculo de Tarifas**: Sistema de cobrança com preço inicial + valor por hora
- ✅ **Interface Interativa**: Menu de console amigável e intuitivo

## 🏗️ Arquitetura

O projeto segue uma arquitetura simples e organizada:

```
DesafioFundamentos/
├── Models/
│   └── Estacionamento.cs      # Classe principal com a lógica de negócio
├── Program.cs                 # Ponto de entrada e interface do usuário
└── DesafioFundamentos.csproj  # Configurações do projeto
```

### 📊 Diagrama da Classe Estacionamento

![Diagrama de classe estacionamento](diagrama_classe_estacionamento.png)

#### Propriedades:
- **`precoInicial`** (decimal): Taxa fixa cobrada ao estacionar
- **`precoPorHora`** (decimal): Valor cobrado por hora de permanência
- **`veiculos`** (List&lt;string&gt;): Lista das placas dos veículos estacionados

#### Métodos:
- **`AdicionarVeiculo()`**: Cadastra um novo veículo no estacionamento
- **`RemoverVeiculo()`**: Remove um veículo e calcula o valor total
- **`ListarVeiculos()`**: Exibe todos os veículos estacionados

## 🚀 Como Executar

### Pré-requisitos
- [.NET 6.0 SDK](https://dotnet.microsoft.com/download/dotnet/6.0) ou superior
- Terminal/Prompt de comando

### Passos para execução:

1. **Clone o repositório:**
   ```bash
   git clone <url-do-repositorio>
   cd dio-estacionamento-c#
   ```

2. **Compile o projeto:**
   ```bash
   dotnet build
   ```

3. **Execute a aplicação:**
   ```bash
   dotnet run --project DesafioFundamentos
   ```

## 🎮 Como Usar

1. **Inicialização**: Ao executar, o sistema solicitará:
   - Preço inicial do estacionamento
   - Preço por hora

2. **Menu Principal**: Escolha uma das opções:
   ```
   1 - Cadastrar veículo
   2 - Remover veículo  
   3 - Listar veículos
   4 - Encerrar
   ```

3. **Cadastrar Veículo**: Digite a placa do veículo a ser estacionado

4. **Remover Veículo**: 
   - Digite a placa do veículo
   - Informe o número de horas estacionado
   - O sistema calculará: `Preço Total = Preço Inicial + (Preço por Hora × Horas)`

5. **Listar Veículos**: Visualize todas as placas dos veículos estacionados

## 💡 Exemplos de Uso

### Exemplo de Cálculo de Tarifa:
```
Preço inicial: R$ 5,00
Preço por hora: R$ 2,00
Tempo estacionado: 3 horas

Valor total = R$ 5,00 + (R$ 2,00 × 3) = R$ 11,00
```

## 🛠️ Tecnologias Utilizadas

- **C# 10**: Linguagem de programação
- **.NET 6.0**: Framework de desenvolvimento
- **Console Application**: Interface de linha de comando
- **LINQ**: Para operações em coleções
- **Encoding UTF-8**: Suporte a acentuação

## 📚 Conceitos Aplicados

- **Programação Orientada a Objetos**: Classes, encapsulamento, métodos
- **Estruturas de Dados**: Listas genéricas (`List<string>`)
- **Estruturas de Controle**: Loops, condicionais, switch-case
- **Tratamento de Entrada**: Conversão de tipos, validação
- **LINQ**: Consultas em coleções com `Any()` e `Remove()`

## 🎓 Desafio Original

Este projeto foi desenvolvido como parte do desafio "Construindo um Sistema para um Estacionamento com C#" da trilha .NET Fundamentals da DIO, focando na aplicação prática dos conceitos fundamentais da linguagem C# e do framework .NET.

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

<div align="center">
  Desenvolvido com ❤️ como parte da trilha .NET da <a href="https://www.dio.me">DIO</a>
</div>
