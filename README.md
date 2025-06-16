# ⚔️ Battle-Game

Simulador de batalhas entre ninjas com jutsus personalizados. Desenvolvido em Java com foco em orientação a objetos e testes automatizados com JUnit.

---

## 📌 Descrição do Repositório

Este repositório contém um projeto simples e didático que simula combates entre personagens fictícios. Cada ninja possui um jutsu com dano e custo de chakra, e a batalha segue uma sequência pré-definida de ataques alternados. O objetivo é reforçar conceitos de lógica de programação, estrutura de classes e testes automatizados.

---

## 📚 Detalhes do Projeto

- Cada ninja possui:
  - Nome
  - Chakra inicial (100)
  - Jutsu principal (com dano e consumo de chakra)
- A batalha segue uma lógica de três rodadas de ataque.

---

## 🛠️ Estrutura do Projeto

- `Jutsu.java` – Define o jutsu com **dano** e **chakra consumido**.
- `Ninja.java` – Representa o ninja com nome, chakra e jutsu.
- `Batalha.java` – Executa a lógica da batalha entre dois ninjas.
- Testes automatizados:
  - `batalhaTest.java`
  - `ninjaTest.java`
  - `jutsuTest.java`

---

## ✅ Testes Automatizados

O projeto possui testes utilizando **JUnit**, cobrindo:

- Inicialização dos atributos dos objetos.
- Redução de chakra conforme o uso do jutsu.
- Lógica de ataque e dano ao oponente.
- Regras especiais de vitória.

---

## 🏫 Observação Final
Este projeto foi desenvolvido para fins educacionais durante a capacitação da **CWI** no programa **eCrescer 2025**.

---

## 🥋 Exemplo de uso

```java
Jutsu katon = new Jutsu(4, 8);
Ninja naruto = new Ninja("Naruto", katon);
Ninja sasuke = new Ninja("Sasuke", new Jutsu(5, 9));

Batalha batalha = new Batalha();
Ninja vencedor = batalha.lutar(naruto, sasuke);

System.out.println("O vencedor é: " + vencedor.getNome());


