# Concorrência-e-Consistência---Spring-Boot
# 📝 Trabalho Prático: Concorrência e Consistência em Banco de Dados com Spring Boot

Este projeto foi desenvolvido com o objetivo de compreender na prática os problemas de concorrência em sistemas transacionais (como o fenômeno de *Lost Update* / Atualização Perdida) e como solucioná-los utilizando o controle de versão otimista com JPA/Hibernate.

---

## 👥 Integrantes e Divisão de Trabalho

* **Aluno A (Responsável pela Parte 1):** Enzo Hoshino
  * *Escopo:* Implementação da entidade `ContaBancaria` padrão, Service transacional básico sem bloqueios, configuração dos cenários de teste de estresse no JMeter e análise do corrompimento de saldo.
* **Aluno B (Responsável pela Parte 2):** Pedro Gabriel
  * *Escopo:* Implementação da entidade `ContaBancariaVersionada` com controle de `@Version`, tratamento da exceção `ObjectOptimisticLockingFailureException` no Controller retornando HTTP 409 Conflict, e análise das requisições barradas de forma segura.

---

## 🛠️ Tecnologias Utilizadas

* Java 17 / 21
* Spring Boot (Spring Web, Spring Data JPA)
* Banco de Dados em Memória H2
* Apache JMeter (Para testes de carga e concorrência)

---

## 🏃‍♂️ Como Rodar a Aplicação

1. Certifique-se de ter o **Java** e o **Maven** instalados na sua máquina.
2. Clone o repositório:
   ```bash
   git clone [URL_DO_SEU_REPOSITORIO]
