# 💸 03-Mobile-EduPay-Android-Firebase

### 💡 Visão Geral e Minha Execução

Desenvolvi o **EduPay**, um aplicativo mobile nativo para Android focado em **gestão financeira e acadêmica**. O objetivo foi criar uma solução prática, rápida e segura para o acesso e pagamento de mensalidades, utilizando uma arquitetura robusta baseada em **Android Studio e Firebase**.

O projeto demonstrou minha capacidade de atuar como um desenvolvedor **Full Stack Mobile**, gerenciando desde a interface de usuário (XML) até a lógica de negócios e o backend em nuvem.

---

## 🎯 Destaques Técnicos e Inovações

* **Autenticação e Segurança (Firebase Authentication):** Implementação de um fluxo completo de login e cadastro, garantindo a criptografia de senhas e a segurança dos dados do usuário.
* **Back-end Serverless (Firebase Firestore/Realtime DB):** Uso do Firebase como solução de Back-end serverless para gerenciar dados de transações, mensalidades e o catálogo de produtos para troca de pontos.
* **Sistema de Gamificação:** Criei a lógica para o sistema de pontos, onde cada mensalidade paga gera **+40 pontos**, incentivando a adimplência e oferecendo benefícios para a troca por produtos.
* **Desenvolvimento Nativo:** Domínio do **Android Studio** com Java (Groovy) para criar uma experiência de usuário (UX) com navegação fluida e animações personalizadas.

---

## 🛠️ Stack Tecnológica

| Categoria | Tecnologia | Uso no Projeto |
| :---: | :--- | :--- |
| **Mobile Nativo** | **Android Studio (Groovy)** | Ambiente de desenvolvimento e linguagem base para a lógica do aplicativo. |
| **Autenticação** | **Firebase Authentication** | Gerenciamento de usuários, login/cadastro e segurança de senhas. |
| **Banco de Dados** | **Firebase Firestore / Realtime DB** | Banco de dados NoSQL utilizado para persistência de dados de usuários, pagamentos e pontos. |
| **Back-end Avançado** | **Firebase Functions** | (Opcional) Utilizado para lógica avançada e validações do lado do servidor. |
| **Interface** | **XML / Material Design** | Criação dos layouts personalizados e componentes da interface do usuário. |

---

## 📁 Estrutura de Telas (Arquitetura)

Abaixo estão as principais `Activities` (Telas) desenvolvidas, que demonstram a arquitetura modular do projeto:

| Tela | Componente | Propósito |
|------|-----------|-----------|
| **Login/Cadastro** | `LoginActivity.java`, `CadastroActivity.java` | Gerenciamento de acesso e coleta de dados do usuário. |
| **Fluxo Principal** | `MainActivity.java` | Tela de boas-vindas e hub de navegação principal. |
| **Gestão Financeira** | `TelaPagamentosActivity.java` | Área para cadastro, consulta e geração de opções de pagamento (PIX, Boleto, Cartão). |
| **Gamificação** | `TelaTrocaPontosActivity.java` | Interface para listar produtos e efetuar a troca dos pontos acumulados. |
| **Comunicação** | `TelaFeedbackActivity.java` | Permite ao usuário enviar feedback e avaliação por estrelas. |

---

## 🎓 Contexto Acadêmico

Este projeto foi desenvolvido durante o **3º semestre** do curso de Análise e Desenvolvimento de Sistemas da **FECAP**.

* **Professores Orientadores:** Aimar Martins Lopes, Francisco Escobar, Vinicius Heltai, Jefferson Silva.

---

[⬅️ Voltar ao README Principal](../../README.md)
