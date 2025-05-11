#### 10. (Propriedades estatísticas dos textos) O que diz a Lei de Zipf? Qual sua relação com stopwords?
 A Lei de Zipf afirma que a frequência de uma palavra é inversamente
proporcional à sua posição no ranking de frequências. Stopwords são frequentes, estando muito provavelmente no topo do ranking.

##### 11. (Propriedades estatísticas dos textos) O que diz a Lei de Heaps? É possível afirmar que, em geral, a taxa de novos termos em um texto se mantém constante?
A Lei de Heaps diz que o vocabulário cresce sublinearmente com o tamanho do
texto. Em geral, a taxa de novos termos diminui conforme o texto aumenta.

##### 23. (Modelos tradicionais de representação textual) Explique brevemente os termos TF e IDF do modelo TF-IDF. Qual termo está relacionado à raridade do termo?

TF (T erm Frequency) mede a frequência de um termo em um documento. IDF
(Inverse Document Frequency) avalia a raridade do termo em todos os documentos. O **IDF** está relacionado à **raridade** do termo.

----
##### 48. Defina brevemente os seguintes conceitos sobre redes
neurais textuais:
- f) **Transformers:** 
    - Arquitetura que substitui recorrência por atenção, permitindo processamento paralelo e captura eficiente de dependências contextuais


- **GRU:** 
    - (Gated Recurrent Unit) é um tipo de rede neural recorrente (RNN) desenvolvida para lidar com problemas de longo prazo em sequências, como o desaparecimento e a explosão de gradientes — problemas comuns em RNNs tradicionais durante o treinamento com backpropagation through time (BPTT).


- Qual a ideia geral do mecanismo de atenção, com
ênfase em self-attention?
    -   O mecanismo de atenção identifica as partes mais importantes do contexto para cada palavra, atribuindo pesos que refletem sua relevância.
    -  No **self-attention**, a relação entre todas as palavras de uma sequência é considerada.
--- 
##### O processo geral de treinamento de LLMs pode ser
dividido em quatro fases: 
- (1) coleta de dados, 
- (2) pré-processamento (tokenização), 
- (3) pré-treino e 
- (4) fine-tuning. 

Explique brevemente cada uma destas fases tendo enfoque nos seguintes modelos estudados:
**a) BERT :**
- (1) Coleta de textos variados;
- (2) T okenização com WordPiece;
- (3) Pré-treino com Masked Language Modeling (MLM) e Next Sentence Prediction (NSP);
- (4) Fine-tuning para tarefas específicas.

**b) GPT-3:**
- (1) Coleta massiva de dados;
- (2) Tokenização com Byte Pair Encoding (BPE);
- (3) Pré-treino autorregressivo;
- (4) Ajustes com prompts para aplicações específicas

---
##### 57. (Large Language Models) Por que LLMs como o BERT e GPT podem ser treinados de forma “auto-supervisionada”?

BERT e GPT são treinados de forma auto-supervisionada porque utilizam os
próprios dados para gerar rótulos (ex.: prever palavras ou completar sentenças) sem
necessidade de anotações manuais

---
##### 60. (BERT) Qual a saída do modelo BERT após o pré-treino? Como esta saída pode ser adaptada para realizar tarefas específicas, como classificação, por exemplo?
Embeddings contextuais para cada token. Para tarefas específicas, como classificação, camadas adicionais são adicionas para ajustas a saída do modelo

--- 
##### 62. (Geração de texto) Cite e explique brevemente dois motivos que tornam o modelo BERT “pouco adequado” para tarefas de geração de texto e fins.
Bert é bidirecional, o que o torna menos adequado para modelos autorregressivos que geram texto palavra a palavra.

>