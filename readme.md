# 🔥 Promoções Telegram — Mercado Livre

<p align="center">
  <strong>Automação de ofertas e divulgação de produtos por meio do Telegram.</strong>
</p>

---

## 📌 Sobre o Projeto

Projeto desenvolvido para automatizar a divulgação de ofertas e promoções do Mercado Livre através de um canal no Telegram.

A aplicação permitirá cadastrar produtos, gerenciar promoções, armazenar links de afiliados e controlar as publicações. A automação será realizada utilizando o **n8n**, responsável por consultar a API e publicar automaticamente as ofertas aprovadas no Telegram.

## 🎯 Objetivo

Desenvolver uma solução de divulgação de promoções que facilite o gerenciamento de ofertas e automatize o processo de publicação, com foco em marketing de afiliados e monetização por meio de comissões.

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Finalidade |
|---|---|
| ☕ Java | Linguagem principal |
| 🌱 Spring Boot | Desenvolvimento da API REST |
| 🔄 Spring Data JPA / Hibernate | Persistência e mapeamento objeto-relacional |
| 🐘 PostgreSQL | Banco de dados |
| 🔐 Spring Security | Segurança e proteção dos endpoints |
| 📦 Lombok | Redução de código repetitivo |
| ✅ Bean Validation | Validação dos dados |
| ⚙️ n8n | Automação dos fluxos de publicação |
| ✈️ Telegram Bot API | Integração e envio automático de promoções |

## ⚙️ Funcionamento

O sistema terá um fluxo semiautomático, no qual o administrador seleciona e cadastra as ofertas, enquanto a publicação é realizada automaticamente.

1. **Cadastro:** O administrador cadastra produtos e promoções na API, informando preços, imagens e links de afiliados.
2. **Validação:** O sistema valida os dados e calcula o percentual de desconto.
3. **Aprovação:** O administrador analisa e aprova as promoções que serão divulgadas.
4. **Automação:** O n8n consulta periodicamente a API e identifica as publicações pendentes.
5. **Publicação:** As promoções aprovadas são enviadas automaticamente ao canal do Telegram, contendo imagem, descrição, preços e link de afiliado.
6. **Registro:** A API armazena o histórico e o status de cada publicação.

## 🏗️ Estrutura Principal

- **Product:** Gerenciamento dos produtos.
- **Promotion:** Gerenciamento das ofertas, preços e descontos.
- **Channel:** Gerenciamento dos canais de divulgação.
- **Publication:** Controle e histórico das publicações.

## 🔗 Arquitetura

A aplicação será organizada da seguinte forma:

```text
Administrador
     |
     v
Spring Boot (API REST)
     |
     v
PostgreSQL
     |
     v
n8n (Automação)
     |
     v
Telegram Bot API
     |
     v
Canal de Promoções
```

O **Spring Boot** será responsável pelas regras de negócio, processamento e gerenciamento dos dados. O **PostgreSQL** armazenará as informações da aplicação, enquanto o **n8n** realizará a orquestração das publicações por meio de requisições HTTP à API.

## 🚀 Escopo Inicial (MVP)

- [ ] Cadastro e gerenciamento de produtos.
- [ ] Cadastro de promoções e links de afiliados.
- [ ] Aprovação e rejeição de ofertas.
- [ ] Integração com Telegram.
- [ ] Publicação automática por meio do n8n.
- [ ] Controle de status e histórico de publicações.
- [ ] Tratamento de falhas e prevenção de publicações duplicadas.

## 🔮 Evoluções Futuras

- Integração com APIs oficiais do Mercado Livre para coleta de produtos.
- Identificação automática de ofertas.
- Integração com outros marketplaces, como Amazon.
- Dashboard para acompanhamento de publicações e resultados.
- Métricas de desempenho e conversões.

---

## 📌 Status do Projeto

🚧 **Em desenvolvimento**

---

<p align="center">
  Desenvolvido com ☕ Java, Spring Boot e muita dedicação.
</p>