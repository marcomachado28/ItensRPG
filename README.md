#  API REST de Gerenciamento de Itens de RPG

API REST desenvolvida em Spring Boot para o gerenciamento de inventário e catálogo de Itens de RPG (armas, armaduras, poções, pergaminhos e artefatos mágicos). O sistema permite que mestres de jogo e jogadores cadastrem, consultem, atualizem e organizem equipamentos e suprimentos de campanha, utilizando persistência em memória com H2 Database e validação de dados via Bean Validation.

---

## Sobre o Contexto do Projeto (Itens de RPG)

Em campanhas de RPG de mesa ou jogos eletrônicos, o controle de inventário, preços em moedas de ouro/prata e disponibilidade em lojas de mercadores é essencial. Esta API modela cada item do jogo como um registro estruturado, permitindo:

* **Gestão de Lojas e Mercadores:** Controle de estoque (`quantidadeEstoque`) e valor comercial (`preco`) de itens disponíveis para venda nas tavernas e ferreiros.
* **Categorização de Equipamentos:** Organização por classes de itens (`categoria`), como *Armas*, *Armaduras*, *Poções*, *Itens Mágicos* ou *Consumíveis*.
* **Balanceamento e Consulta Rápida:** Listagem e busca direta por identificador único (`id`) para agilizar sessões de jogo.

---

## Tecnologias Utilizadas

* **Java 21**
* **Spring Boot 3.2.5**
* **Spring Data JPA**
* **Spring Boot Starter Validation**
* **H2 Database (In-Memory)**
* **Maven**

---

## Como Compilar e Rodar a Aplicação (CLI)

Certifique-se de ter o **Java 21** instalado. Abra o terminal na pasta raiz do projeto (`demo`) e execute os comandos abaixo:

1. **Limpar e Compilar o Projeto:**
   ```powershell
   .\mvnw.cmd clean compile
