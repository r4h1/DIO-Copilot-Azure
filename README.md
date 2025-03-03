# Análise de Sentenças com Detecção de Idioma e Sentimento

Este projeto Python analisa uma sentença fornecida para detectar seu idioma, sentimento e extrair instâncias-chave básicas e palavras-chave.

## Funcionalidades

* **Detecção de Idioma:** Identifica o idioma da sentença de entrada usando a biblioteca `langdetect`.
* **Análise de Sentimento:** Determina o sentimento (positivo, negativo ou neutro) da sentença usando o `nltk.sentiment.SentimentIntensityAnalyzer` (VADER).
* **Extração Básica de Instâncias:** Extrai instâncias simples como pessoas, lugares e sentimentos com base na correspondência de palavras-chave. (Este é um exemplo simplificado e pode ser significativamente melhorado com o Reconhecimento de Entidades Nomeadas (NER)).
* **Extração Básica de Palavras-chave:** Extrai palavras-chave da sentença usando uma expressão regular simples.
* **Entrada do Usuário:** Aceita sentenças do usuário através da linha de comando.
* **Tratamento de Erros:** Inclui tratamento de erros para falhas na detecção de idioma.

## Dependências

* `textblob`
* `langdetect`
* `nltk`

Instale as bibliotecas necessárias usando o pip:

```bash
pip install textblob langdetect nltk

Além disso, baixe os dados necessários do NLTK:
import nltk
nltk.download('vader_lexicon')
nltk.download('punkt')
nltk.download('averaged_perceptron_tagger')

Exemplo

Entrada:
Eu gosto de sorvetes.

Saída:
Input: Eu gosto de sorvetes.
Output: {'Language': 'pt', 'Sentiment': 'Positive', 'Instances': {'Feeling': 'Positive'}, 'Key-word': 'eu gosto de sorvetes'}

Markdown

# Análise de Sentenças com Detecção de Idioma e Sentimento

Este projeto Python analisa uma sentença fornecida para detectar seu idioma, sentimento e extrair instâncias-chave básicas e palavras-chave.

## Funcionalidades

* **Detecção de Idioma:** Identifica o idioma da sentença de entrada usando a biblioteca `langdetect`.
* **Análise de Sentimento:** Determina o sentimento (positivo, negativo ou neutro) da sentença usando o `nltk.sentiment.SentimentIntensityAnalyzer` (VADER).
* **Extração Básica de Instâncias:** Extrai instâncias simples como pessoas, lugares e sentimentos com base na correspondência de palavras-chave. (Este é um exemplo simplificado e pode ser significativamente melhorado com o Reconhecimento de Entidades Nomeadas (NER)).
* **Extração Básica de Palavras-chave:** Extrai palavras-chave da sentença usando uma expressão regular simples.
* **Entrada do Usuário:** Aceita sentenças do usuário através da linha de comando.
* **Tratamento de Erros:** Inclui tratamento de erros para falhas na detecção de idioma.

## Dependências

* `textblob`
* `langdetect`
* `nltk`

Instale as bibliotecas necessárias usando o pip:

```bash
pip install textblob langdetect nltk
Além disso, baixe os dados necessários do NLTK:

Python

import nltk
nltk.download('vader_lexicon')
nltk.download('punkt')
nltk.download('averaged_perceptron_tagger')
Uso
Clone o repositório ou baixe o script Python.
Instale as dependências conforme descrito acima.
Execute o script na linha de comando:
Bash

python seu_script_nome.py
Digite uma sentença quando solicitado.
O script irá exibir o idioma, sentimento, instâncias e palavras-chave da sentença.
Exemplo
Entrada:

Eu gosto de sorvetes.
Saída:

Input: Eu gosto de sorvetes.
Output: {'Language': 'pt', 'Sentiment': 'Positive', 'Instances': {'Feeling': 'Positive'}, 'Key-word': 'eu gosto de sorvetes'}
Entrada:

I was very sad yesterday because of the news.
Saída:

Input: I was very sad yesterday because of the news.
Output: {'Language': 'en', 'Sentiment': 'Negative', 'Instances': {'Feeling': 'Negative'}, 'Key-word': 'i was very sad yesterday because of the news'}

Melhorias
Este projeto pode ser melhorado por:

Implementar o Reconhecimento de Entidades Nomeadas (NER) para uma extração de instâncias mais precisa.
Usar técnicas de extração de palavras-chave mais avançadas, como TF-IDF ou TextRank.
Adicionar suporte para mais idiomas.
Considerar o uso de um modelo de análise de sentimento mais sofisticado para maior precisão.
Traduzir sentenças para o inglês antes da análise de sentimento, para aumentar a precisão.
Adicionar tratamento de erros mais robusto.
Autor
[R4H1]
