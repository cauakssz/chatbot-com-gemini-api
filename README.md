# 🤖 Chatbot com Google Gemini API

Chatbot conversacional em Python, construído em Google Colab, que utiliza a API do Google Gemini para gerar respostas em linguagem natural com manutenção de contexto ao longo da conversa.

## 💬 Sobre o projeto

O projeto implementa um chat interativo no terminal (via notebook) em que o usuário troca mensagens em português com o assistente, apelidado de **Jarvis**. Cada resposta é gerada em tempo real pela API do Gemini e exibida já formatada em Markdown, preservando negrito, listas e demais elementos de formatação retornados pelo modelo.

A conversa mantém histórico durante toda a sessão, permitindo que o modelo leve em conta as mensagens anteriores ao gerar novas respostas.

## ✨ Funcionalidades

- Conversa contínua com manutenção de histórico (`start_chat`)
- Respostas renderizadas em Markdown (negrito, listas, blocos de texto)
- Configuração de parâmetros de geração (`temperature`, `candidate_count`)
- Ajuste de filtros de segurança do modelo (`safety_settings`)
- Listagem dos modelos Gemini disponíveis na conta via API
- Comando de saída dedicado (`"dispensar jarvis"`) para encerrar a conversa

## 🛠️ Tecnologias utilizadas

- Python 3
- [google-generativeai](https://pypi.org/project/google-generativeai/) (SDK oficial do Gemini)
- Google Colab
- IPython / Markdown (para exibição formatada das respostas)

## 🚀 Como executar

1. Abra o notebook `Copy_of_my_firts_IA_chat.ipynb` no [Google Colab](https://colab.research.google.com/)
2. Gere uma API key gratuita em [Google AI Studio](https://aistudio.google.com/app/apikey)
3. No Colab, adicione a chave em **Secrets** (ícone de chave 🔑) com o nome `GOOGLE_API_KEY`
4. Execute as células em ordem — a primeira instala o SDK do Gemini:
   ```python
   pip install -U -q google-generativeai
   ```
5. Na última célula, digite suas mensagens quando solicitado (`Você: `). Para encerrar, digite:
   ```
   dispensar jarvis
   ```

## 🧠 O que este projeto demonstra

- Integração com uma API de IA generativa (Google Gemini)
- Gerenciamento de estado de conversa (histórico de chat)
- Configuração de parâmetros de um modelo de linguagem (temperatura, safety settings)
- Formatação e exibição de conteúdo dinâmico gerado por IA

---

Desenvolvido por [Cauã de Souza Silva](https://github.com/cauakssz)
