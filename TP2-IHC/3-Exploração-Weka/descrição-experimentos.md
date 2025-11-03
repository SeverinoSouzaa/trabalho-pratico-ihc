# Etapa 3 — Exploração e Classificação no Weka

## Introdução

Esta etapa apresenta a **análise de emoções no jogo Clash Royale** a partir da base sintética gerada.  
Os experimentos foram realizados no **Weka**, utilizando diferentes algoritmos de classificação supervisionada, para avaliar o desempenho na predição da variável **emocao_jogador**.

A seguir, são descritas as observações obtidas na aba *Visualize* e, posteriormente, os resultados e interpretações de cada algoritmo testado.  
Os detalhes técnicos de cada modelo podem ser consultados na pasta [`/algoritmos/`](./saídas-algoritmos.md).

---

## 3.1 Visualização da Base de Dados (*Visualize*)

Na aba **Visualize** do Weka, foram analisadas as relações entre os atributos e a classe-alvo.  
O comportamento observado foi o seguinte:

- **feliz →** valores mais altos de troféus.  
- **motivado →** ganhos moderados.  
- **neutro →** valores próximos de zero.  
- **frustrado →** perdas significativas.

Essa relação confirma que o atributo `trofeus_delta` possui forte correlação com a emoção do jogador, reforçando a estrutura lógica usada para criar a classe-alvo.

### 🖼️ Imagem da Aba *Visualize*
<img width="1643" height="2285" alt="Design sem nome (1)" src="https://github.com/user-attachments/assets/eda89666-29fd-4896-92d5-2d3495a51de7" />

---

## 3.2 Algoritmos Testados

Nesta seção estão descritos todos os algoritmos aplicados no Weka.  
Foram utilizados cinco algoritmos principais: **ZeroR, OneR, J48, Naive Bayes e IBk.**

---

### ⚙️ ZeroR e OneR

#### 🔹 ZeroR
- Previu todas as instâncias como “motivado”.  
- Acertou apenas **60 de 200 instâncias**, resultando em **30% de acurácia**.  
- Não considerou nenhum atributo preditor.

#### 🔹 OneR
- Utilizou apenas o atributo **trofeus_delta**.  
- Acertou **199 de 200 instâncias**, com **99,5% de acurácia**.  
- Errou **1 caso da classe “frustrado”**, previsto como “neutro”.

---

### ⚙️ J48

#### 📊 Desempenho e Interpretação

> 🔍 **Por que a acurácia foi tão alta?**

A classe-alvo foi criada com base direta no atributo **trofeus_delta**, o que simplifica a tarefa de aprendizado.

- **Acurácia do J48:** 99,5%  
- O modelo cometeu apenas **1 erro entre 200 instâncias.**  
- A árvore gerada reproduziu fielmente as regras manuais baseadas em *trofeus_delta*.  
- Isso confirma que a base possui **estrutura bem definida e altamente previsível.**  
- O J48 foi tão eficaz quanto o OneR, mas oferece **maior interpretabilidade e estrutura lógica.**

#### 🌳 Árvore Gerada
<img width="2337" height="1335" alt="Design sem nome (2)" src="https://github.com/user-attachments/assets/2b5f0e2c-a80e-42c1-833e-10b7687aee70" />


> A árvore gerada pelo J48 revelou exatamente as regras utilizadas para gerar a classe-alvo, confirmando a capacidade do modelo em “descobrir” os padrões esperados.

---

### ⚙️ Naive Bayes e IBk

#### 🔹 Naive Bayes
- **Acurácia:** 99% (198 acertos em 200).  
- Errou 1 instância da classe *feliz* (classificada como *motivado*).  
- Errou 1 instância da classe *neutro* (classificada como *frustrado*).  
- Utilizou todos os atributos, com boa separação entre classes.  
- Leve confusão entre emoções próximas na escala de troféus.

#### 🔹 IBk
- **Acurácia:** 92% (184 acertos em 200).  
- Maior parte dos erros na classe *neutro*:  
  - 3 classificados como *motivado*  
  - 7 como *frustrado*  
- Também errou 1 exemplo de *frustrado*, classificado como *neutro*.  
- Classificador baseado em vizinhos, mais sensível à sobreposição entre classes.  
- Resultado bom, mas inferior aos modelos baseados em regras.

---

## 3.3 Discussão Geral

Os resultados mostram que os classificadores baseados em **regras simples** (OneR e J48) atingiram desempenho máximo, pois a classe foi derivada diretamente do atributo `trofeus_delta`.  
Isso explica as altas taxas de acerto e confirma que a base está **bem estruturada e previsível**.

Modelos mais complexos, como **Naive Bayes** e **IBk**, apresentaram desempenho um pouco inferior, devido à sobreposição parcial de valores e à sensibilidade a variações menores.

---

## 3.4 Interpretação

Os resultados obtidos indicam que:
- As regras criadas manualmente foram **reconhecidas com precisão** pelos algoritmos supervisionados.  
- O **atributo-chave `trofeus_delta`** é o principal fator determinante da emoção do jogador.  
- A base demonstra **alta consistência e correlação direta** entre desempenho e emoção.

