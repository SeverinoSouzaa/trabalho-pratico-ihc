# Etapa 2 — Geração da Base de Dados Sintética
[🔗 Clique aqui para abrir a Base Sintética (.arff)](./base_sintetica.arff)


## Introdução

Esta etapa descreve o processo de **geração da base de dados sintética**, utilizada para representar o comportamento e as emoções dos jogadores no contexto do Clash Royale.  
A base foi criada com **200 instâncias simuladas**, seguindo as regras definidas e estruturada no formato **ARFF**, compatível com o software **Weka**.

Cada registro representa uma partida, contendo os atributos preditores relacionados ao desempenho do jogador e a **classe-alvo (emoção do jogador)**.  
O objetivo é permitir a análise supervisionada das emoções a partir das métricas do jogo, servindo como base para os experimentos de classificação.

---

## 2.1 Regras da Classe-Alvo

> “A classe emoção do jogador foi definida assim:”

| Classe | Regras Definidoras |
|---------|--------------------|
| **feliz** | Se `dif_torres ≥ +2` e `trofeus_delta ≥ +25` e `torres_perdidas ≤ 1` e `vitorias_consecutivas ≥ 2`. |
| **motivado** | Se `dif_torres = +1` e `trofeus_delta ∈ [+12 , +24]` e (`torres_destruidas ≥ 2` ou `vitorias_consecutivas ≥ 1`). |
| **neutro** | Se (`dif_torres = +1` e `trofeus_delta ∈ [+3 , +11]`) ou (`dif_torres = −1` e `trofeus_delta ∈ [−9 , −1]`). |
| **frustrado** | Se (`dif_torres ≤ −2` ou `torres_perdidas = 3`) ou `trofeus_delta ≤ −10`. |

---

## 2.2 Interpretação das Emoções

- **feliz:** vitória dominante (3 coroas), ganho alto de troféus e sequência positiva.  
- **motivado:** vitória comum, resultado positivo e progresso estável.  
- **neutro:** partida equilibrada ou derrota leve, emoção intermediária.  
- **frustrado:** derrota forte, perda alta de troféus e muitas torres destruídas.

---

## 2.3 Estrutura e Equilíbrio da Base

A base é **balanceada**, com leve destaque para a classe *motivado*, simulando jogadores mais engajados.

| Classe | Quantidade de Instâncias |
|---------|---------------------------|
| **feliz** | 50 |
| **motivado** | 60 |
| **neutro** | 45 |
| **frustrado** | 45 |

---

## 2.4 Descrição da Base Sintética

A base é composta pelos mesmos atributos definidos na Etapa 1 — Definição do Problema.  
Cada instância contém valores numéricos ou categóricos coerentes com o contexto de jogo.  
Os dados foram gerados com auxílio de um LLM e ajustados para evitar sobreposição entre classes e garantir padrões lógicos nas variações de desempenho.

---

## 2.5 Considerações

Esta base sintética representa uma **simulação realista do comportamento de jogadores** sob diferentes condições emocionais.  
Seu formato padronizado em `.arff` facilita a exploração posterior no Weka, onde serão aplicados algoritmos de classificação supervisionada.


