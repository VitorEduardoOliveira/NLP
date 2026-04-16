# 🧠 NLP Lab — Laboratório de Processamento de Linguagem Natural

> Coleção de projetos práticos de NLP construídos em Python, do zero ao estado da arte.  
> Cada projeto é documentado, explicado e pronto para rodar no Google Colab.

---

## 📌 Sobre este repositório

**NLP Lab** é um repositório dedicado à exploração prática de técnicas de Processamento de Linguagem Natural. Os projetos cobrem desde abordagens clássicas (TF-IDF, similaridade de cossenos) até modelos modernos baseados em transformers, sempre com foco em código limpo, documentação detalhada e reprodutibilidade.

Os projetos são desenvolvidos como notebooks no **Google Colab**, sem necessidade de configuração local.

---

## 🗂️ Projetos

### 01 — Chatbot Semântico com Similaridade de Cossenos

> Um chatbot de recuperação de informações construído do zero, evoluído em três versões.

| Versão | Descrição | Interface | Notebook |
|--------|-----------|-----------|----------|
| **v1 — Modelo Original** | TF-IDF + NLTK + Similaridade de Cossenos | ipywidgets | [`chatbot_v1.ipynb`](./01-chatbot-cossenos/chatbot_v1.ipynb) |
| **v2 — Base CSV** | Sentence Transformers + base carregada via CSV | Gradio | [`chatbot_v2_csv.ipynb`](./01-chatbot-cossenos/chatbot_v2_csv.ipynb) |
| **v3 — Base PDF** | Sentence Transformers + chunking de PDF (RAG simples) | Gradio | [`chatbot_v3_pdf.ipynb`](./01-chatbot-cossenos/chatbot_v3_pdf.ipynb) |

**Tecnologias:** `scikit-learn` `nltk` `sentence-transformers` `gradio` `ipywidgets` `pymupdf`

**O que você vai aprender:**
- Como texto é convertido em vetores numéricos (TF-IDF)
- Como medir similaridade entre frases com similaridade de cossenos
- Como usar embeddings semânticos com Sentence Transformers
- Como construir uma interface de chat no Google Colab
- Como implementar RAG (Retrieval-Augmented Generation) de forma simplificada

**Arquivos incluídos:**

```
01-chatbot-cossenos/
├── chatbot_v1.ipynb              # Modelo original com TF-IDF e ipywidgets
├── chatbot_v2_csv.ipynb          # Modelo com Sentence Transformers + CSV
├── chatbot_v3_pdf.ipynb          # Modelo com Sentence Transformers + PDF
├── base_conhecimento.csv         # Base de 30 perguntas e respostas prontas
├── docs/
│   ├── documentacao_modelo_original.pdf   # Documentação técnica v1
│   └── documentacao_csv_pdf.pdf           # Documentação técnica v2 e v3
└── README.md
```

---

> 🔜 Mais projetos em breve — classificação de texto, análise de sentimentos, sumarização automática e muito mais.

---

## 🚀 Como usar

Todos os projetos rodam diretamente no Google Colab. Basta clicar no badge abaixo ou abrir o notebook desejado manualmente:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

**Passos:**
1. Abra o notebook desejado no Google Colab
2. Execute a **Célula 1** para instalar as dependências
3. Execute as demais células em ordem
4. Interaja com a interface gerada na última célula

---

## 🛠️ Tecnologias utilizadas

| Biblioteca | Uso nos projetos |
|------------|-----------------|
| `scikit-learn` | TF-IDF, similaridade de cossenos |
| `nltk` | Tokenização, stopwords em português |
| `sentence-transformers` | Embeddings semânticos multilíngues |
| `gradio` | Interface web com link público compartilhável |
| `ipywidgets` | Interface interativa dentro do Colab |
| `pymupdf` | Extração de texto de arquivos PDF |
| `pandas` | Leitura e processamento de arquivos CSV |
| `numpy` | Operações com vetores e matrizes |

---

## 📚 Conceitos abordados

```
NLP
├── Pré-processamento
│   ├── Tokenização
│   ├── Remoção de stopwords
│   └── Normalização (lowercase, pontuação)
├── Representação de texto
│   ├── TF-IDF (Term Frequency-Inverse Document Frequency)
│   └── Embeddings semânticos (Sentence Transformers)
├── Similaridade
│   └── Similaridade de Cossenos
├── Recuperação de informação
│   ├── Busca por similaridade
│   └── RAG simplificado (chunking de documentos)
└── Interfaces
    ├── ipywidgets (Colab nativo)
    └── Gradio (link público)
```

---

## 📋 Pré-requisitos

- Conta Google (para usar o Colab)
- Nenhuma instalação local necessária
- Conhecimento básico de Python é recomendado

---

## 📄 Documentação

Cada projeto possui documentação técnica em PDF disponível na pasta `docs/`, cobrindo:

- Fundamentos teóricos dos algoritmos utilizados
- Arquitetura e fluxo do sistema
- Código explicado linha por linha
- Exemplos de funcionamento com scores reais
- Limitações e próximos passos

---

## 🗺️ Roadmap

- [x] Chatbot com TF-IDF e ipywidgets
- [x] Chatbot com Sentence Transformers e Gradio
- [x] Suporte a base CSV e PDF (RAG simples)
- [ ] Classificação de texto (spam, sentimentos, tópicos)
- [ ] Análise de sentimentos com BERT em português
- [ ] Sumarização automática de textos
- [ ] Extração de entidades nomeadas (NER)
- [ ] Chatbot com memória de contexto e histórico
- [ ] RAG completo com FAISS e LLM

---

## 📝 Licença

Este repositório é disponibilizado sob a licença [MIT](./LICENSE).  
Sinta-se livre para usar, modificar e distribuir os projetos com os devidos créditos.

---

<div align="center">
  <sub>Feito com preguiça e muito Python &nbsp;|&nbsp; NLP Lab</sub>
</div>
