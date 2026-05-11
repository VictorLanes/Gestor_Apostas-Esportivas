# ⚡ BetTrack — Sistema de Gestão de Apostas Profissional

## 📋 Sobre o Projeto

O **BetTrack** é uma aplicação Single Page (SPA) desenvolvida para apostadores que buscam profissionalismo e controle rigoroso sobre sua banca. O foco do projeto é transformar dados brutos de apostas em **insights estratégicos**, permitindo visualizar onde estão os maiores lucros e como a banca evolui ao longo do tempo.

Este projeto utiliza uma arquitetura baseada em **Estado (State Management)** no Frontend, garantindo que todos os cálculos de ROI, Winrate e Yield sejam atualizados instantaneamente sem recarregar a página.

---

## 🚀 Funcionalidades Principais

### 1. Dashboard de Performance

* **Métricas em Tempo Real**: Visualização imediata de Banca Atual, Lucro Total, ROI (Retorno sobre Investimento) e Winrate.
* **Gráficos Dinâmicos**: Evolução da banca (Line Chart), Lucro por Esporte (Bar Chart) e Distribuição por Mercado.
* **Widgets de Desempenho**: Resumo estatístico de vitórias, derrotas e sequências atuais (Hot/Cold Streaks).

### 2. Gestão de Apostas e Resultados

* **Registro Detalhado**: Cadastro de eventos, mercados, odds, casas de apostas e tipsters.
* **Filtros Inteligentes**: Consulta rápida por status (Green, Red, Pendente, Cash Out), esporte ou busca por texto.
* **Sistema de Cash Out**: Cálculo automático de lucro/perda para encerramentos antecipados.

### 3. Gestão de Banca e Ferramentas Analíticas

* **Calculadora Kelly**: Integrada para sugestão de stake ideal baseada no *edge* (vantagem) do apostador.
* **Configurações de Risco**: Definição de banca inicial, stake padrão (%) e limites de Stop Win/Loss.
* **Relatórios por Dimensão**: Análise de performance por Casa de Aposta (ex: Bet365 vs Betano) e por mês.

### 4. Exportação Profissional (Excel)

* Geração de arquivo `.xlsx` estilizado com múltiplas abas:
* **Resumo Executivo**: Visão geral para impressão/relatório.
* **Apostas Detalhadas**: Histórico completo com formatação condicional (cores para Green/Red).
* **Análise de Dimensões**: Abas automáticas por Esporte, Casa e Mercado.



---

## 🛠️ Tecnologias e Bibliotecas

* **Frontend**: HTML5, CSS3 (Custom Properties e Flexbox/Grid) e JavaScript Vanilla (ES6+).
* **Gráficos**: [Chart.js](https://www.chartjs.org/) para visualização de dados.
* **Processamento de Planilhas**: [SheetJS (XLSX)](https://sheetjs.com/) com suporte a estilos para relatórios profissionais.
* **Tipografia**: Google Fonts (Space Grotesk e JetBrains Mono).

---

## 📂 Arquitetura do Sistema

O sistema opera sob um **Fluxo de Dados Circular**:

1. **Entrada**: O usuário registra a aposta no formulário.
2. **Processamento**: O objeto `S` (State) é atualizado. A função `calcMetrics()` reprocessa todos os indicadores financeiros.
3. **Saída (UI)**: Os componentes de Dashboard e Tabela são renderizados novamente para refletir os novos valores.
4. **Persistência**: O código está preparado para integração com `localStorage` ou APIs de banco de dados.

---

## 💡 Diferenciais Técnicos

* **Responsividade Total**: O layout se adapta perfeitamente de monitores ultrawide até smartphones.
* **UX Otimizada**: Uso de *Toasts* para feedback de ações, modais para edição rápida e botões de cópia.
* **Código Limpo**: CSS organizado em variáveis `:root` para fácil customização de cores e temas.

---

### 📈 Como utilizar

1. Ao abrir o sistema, configure sua **Banca Inicial** no Setup.
2. Registre suas apostas em "Nova Aposta".
3. Ao finalizar um evento, clique no ícone de lápis na tabela para atualizar o resultado.
4. Utilize a aba "Relatórios" ao final de cada mês para revisar sua estratégia.

---

*Este README foi gerado para documentar o projeto BetTrack.*
