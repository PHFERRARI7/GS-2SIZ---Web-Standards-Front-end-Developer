# 🏥 Global Solution - Web Standards Front-end Developer

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/Bootstrap_5-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white" alt="Bootstrap" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
</p>

> Projeto desenvolvido como avaliação final (Global Solution) do 2º semestre da disciplina de Web Standards. O foco principal da aplicação é a resolução de problemas de negócio utilizando manipulação avançada do DOM com JavaScript Vanilla.

## 📌 Sumário
- [Sobre o Projeto](#-sobre-o-projeto)
- [Funcionalidades e Regras de Negócio](#-funcionalidades-e-regras-de-negócio)
- [Exercício 1: Dashboard de Unidades](#exercício-1-dashboard-de-unidades-de-atendimento)
- [Exercício 2: Simulador de Cotação](#exercício-2-simulador-de-cotação-de-plano-de-saúde)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Como Executar](#-como-executar)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Autor](#-autor)

---

## 💡 Sobre o Projeto

Esta aplicação é composta por dois módulos independentes focados na área da saúde. O objetivo arquitetural foi separar a camada de dados (arquivos mockados/textos) da camada de apresentação (HTML/CSS), utilizando o JavaScript como motor para renderização dinâmica, cálculos matemáticos em tempo real e formatação de dados do usuário.

---

## ⚙️ Funcionalidades e Regras de Negócio

### Exercício 1: Dashboard de Unidades de Atendimento
Um painel de visualização de dados que consome uma base local (Array de Objetos em `unidades.js`) e processa as informações para exibição estratégica.

* **Renderização Condicional:** O algoritmo mapeia a base de dados e injeta no HTML via manipulação de DOM apenas as unidades localizadas no município de "São Paulo".
* **Agregação de Dados:** Cálculo automático e dinâmico da soma total de "Consultas ao Mês" das unidades listadas, exibido no rodapé da tabela.
* **Métricas Comparativas:** Geração em tempo real de estatísticas comparando o número absoluto de unidades na capital paulista versus unidades em outros municípios.

### Exercício 2: Simulador de Cotação de Plano de Saúde
Uma interface de captura de dados interativa para cálculo de mensalidades baseada em fatores de risco (dependentes) e categoria do plano escolhido.

* **Lógica de Precificação:** Implementação da fórmula de negócio: `Valor Base + ((Valor Base * Número de Dependentes) / 2)`.
* **Geração Dinâmica de Tabela:** Utilização de *Template Strings* para capturar o evento de `submit` do formulário e gerar novas linhas (`<tr>`) na tabela de histórico de cotações de forma instantânea.
* **User Experience (UX):** * Formatação automática de valores numéricos para o padrão monetário brasileiro (BRL - `R$`).
  * Reset automático do formulário após cada submissão bem-sucedida, agilizando novas simulações.

---

## 🛠️ Tecnologias Utilizadas

O ecossistema do projeto foi construído utilizando os seguintes padrões de mercado:

* **HTML5:** Estruturação semântica.
* **CSS3 & Bootstrap 5.3.2:** Sistema de grids e componentes responsivos (cards, tables, forms, buttons) para garantir compatibilidade com dispositivos móveis e desktops.
* **JavaScript (ES6+):** * Event Listeners e manipulação de formulários.
  * Array Methods (`filter`, `reduce`, `forEach`).
  * Injeção de marcação no DOM utilizando propriedades como `innerHTML` combinadas com *Template Literals*.

---
