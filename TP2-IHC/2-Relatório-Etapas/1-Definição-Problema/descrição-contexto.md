# Etapa 1 — Definição do Problema

## 1.1 Contexto e Motivação

O **Clash Royale** é um jogo de estratégia em tempo real no qual dois jogadores enfrentam-se utilizando cartas que representam tropas, construções e feitiços.  
Cada partida envolve **tomadas de decisão rápidas** e exige **controle emocional constante**, pois vitórias e derrotas são determinadas por segundos e detalhes táticos.

O objetivo deste trabalho é **classificar a emoção do jogador** com base em métricas reais do jogo, dentro do contexto de **Interação Humano-Computador (IHC)**.  
A ideia é compreender como o desempenho em partidas influencia o estado emocional — desde a frustração após derrotas até a euforia em vitórias decisivas — criando uma **base de dados supervisionada** para análise por algoritmos de aprendizado de máquina.

Além disso, este estudo busca **aprofundar a compreensão da experiência do usuário (UX)** em ambientes competitivos digitais.  
Ao analisar métricas de desempenho e correlacioná-las com estados emocionais, pretende-se evidenciar como **a interação humano-computador pode afetar a motivação, o engajamento e a satisfação** durante o jogo.

---

## 1.2 Atributos Preditores

| Atributo             | Tipo      | Descrição |
|----------------------|-----------|------------|
| **vitorias_consecutivas** | Numérico | Quantidade de vitórias seguidas antes da partida atual (0–5). |
| **cartas_nivel_medio** | Numérico | Média do nível das cartas utilizadas pelo jogador (8–15). |
| **tempo_partida_min** | Numérico | Duração total da partida (2.0–5.0 minutos). |
| **torres_destruidas** | Numérico | Quantidade de torres inimigas destruídas (0–3). |
| **torres_perdidas** | Numérico | Quantidade de torres próprias destruídas (0–3). |
| **trofeus_delta** | Numérico | Diferença de troféus obtida na partida (−40 a +40). |

## 1.3 Classe-Alvo

| Classe-Alvo | Tipo | Valores Possíveis |
|--------------|-------|-------------------|
| **emocao_jogador** | Categórico | {feliz, motivado, neutro, frustrado} |

---

  
