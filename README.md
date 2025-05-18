# 📰 Meu Resumo Local Diário ✨

![Python](https://img.shields.io/badge/Python-3.9+-blue)
![Google ADK](https://img.shields.io/badge/Google_ADK-enabled-orange)
![Google Generative AI](https://img.shields.io/badge/Google_Generative_AI-used-red)
![Google Colab](https://img.shields.io/badge/Run_in-Colab-yellow)

---

## 🎯 Objetivo

Gerar um resumo rápido e personalizado de informações locais (notícias, tempo, eventos, etc.) para uma cidade específica, utilizando **Agentes Google ADK** e a ferramenta **Google Search**.

---

## 🚀 Como Funciona

O projeto orquestra um fluxo simples:

1.  **Pergunta ao Usuário:** Coleta sua localização e interesse.
2.  **Busca na Web:** Um agente ADK usa o **Google Search** para encontrar informações relevantes.
3.  **Sintetiza:** Outro agente ADK analisa os resultados da busca e cria um resumo conciso.
4.  **Apresenta:** O resumo final é exibido para você.

---

## 🛠️ Tecnologias Utilizadas

* **Python:** Linguagem principal de programação.
* **Google Agent Development Kit (ADK):** Para construir e orquestrar os agentes.
* **Google Generative AI API:** O modelo de linguagem (como `gemini-2.0-flash`) que impulsiona os agentes.
* **Google Search Tool:** A ferramenta que permite aos agentes buscar informações na web.
* **Google Colab:** Ambiente recomendado para execução, facilitando o setup.

---

## ⚡ Configuração Rápida

Este projeto é otimizado para execução no **Google Colab**.

1.  **Obtenha sua Chave de API:** Consiga uma **Google Generative AI API Key** no [Google AI Studio](https://aistudio.google.com/).
2.  **Abra no Colab:** Clique no link abaixo para abrir o notebook diretamente:
    ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)
3.  **Configure a API Key:** No Colab, use a aba "Secrets" (ícone da chave 🔑 no menu esquerdo) para adicionar um segredo chamado `GOOGLE_API_KEY` com o valor da sua chave. Certifique-se de ativar o "Notebook access".
4.  **Execute as Células:** Rode cada célula do notebook em ordem (Shift + Enter).
5.  **Interaja:** Na última célula, o notebook pedirá a sua cidade e tipo de informação.

---

## 📂 Estrutura do Código (no Notebook Colab)

* **Célula 1:** Instalação e Importações
* **Célula 2:** Configuração da API Key (Segredos do Colab)
* **Célula 3:** Funções Auxiliares (`call_agent`, `to_markdown`)
* **Célula 4:** Funções Python (`coletar_preferencias_usuario`, `apresentar_resumo`)
* **Célula 5:** Definição dos Agentes ADK (`agente_busca_local`, `agente_analise_sintese`)
* **Célula 6:** Lógica Principal de Execução

---

## ➡️ Como Usar

Após configurar a API Key e executar as primeiras células no Colab, execute a **Célula 6**. Siga as instruções no output para inserir a cidade e o tipo de informação desejada (ex: "Rio de Janeiro", "Notícias locais"). O resumo será exibido na saída.

---

## 🤝 Contribuições

Sugestões e melhorias são bem-vindas!
