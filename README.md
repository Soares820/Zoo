# 🦁 MGZoo - Sistema de Gestão de Animais

Este projeto é um sistema simples de zoológico feito em Java com foco nos conceitos de **herança** e **polimorfismo**.

---

## 🎯 Objetivo

Implementar uma hierarquia de classes que represente diferentes tipos de animais e suas características, usando programação orientada a objetos.

---

## 🐾 Estrutura do Projeto

### Classe Base

- **Animal**
  - Atributos: `nome`, `idade`, `peso`
  - Métodos:
    - `fazerSom()` → imprime "som de um animal"
    - `exibirInformacoes()` → mostra dados básicos

### Subclasses Diretas

- **Mamifero**
  - Novo atributo: `velocidade`
  - Sobrescreve `fazerSom()` e `exibirInformacoes()`

- **Ave**
  - Novo atributo: `envergaduraAsas`
  - Sobrescreve `fazerSom()` e `exibirInformacoes()`

- **Reptil**
  - Novo atributo: `temperaturaCorporal`
  - Sobrescreve `fazerSom()` e `exibirInformacoes()`

---

### Subclasses Específicas

- **Cachorro** (herda de Mamífero)
  - Método adicional: `correr()`

- **Papagaio** (herda de Ave)
  - Método adicional: `voar()`

- **Cobra** (herda de Réptil)
  - Método adicional: `rastejar()`

---

## 🧪 Classe de Teste

- **ZooTeste**
  - Cria um objeto de cada tipo: `Animal`, `Mamifero`, `Ave`, `Reptil`
  - Testa os métodos `fazerSom()` e `exibirInformacoes()`
  - Cria objetos `Cachorro`, `Papagaio`, `Cobra`
  - Testa os métodos específicos como `correr()`, `voar()` e `rastejar()`

---

## ▶️ Como Executar

1. Compile os arquivos `.java`:
   ```bash
   javac *.java
