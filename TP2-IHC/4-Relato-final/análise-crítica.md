# Etapa 4 — Relato Final  
## Análise Crítica dos Resultados em Relação ao Domínio de Interação Humano-Computador (IHC)

---

### 1. Contextualização

O presente estudo teve como objetivo analisar a **experiência emocional dos usuários em jogos digitais**, especificamente no contexto do **Clash Royale**, um jogo competitivo que exige tomada de decisão rápida e controle emocional.  
Dentro da perspectiva da **Interação Humano-Computador (IHC)**, a emoção é um elemento fundamental da experiência do usuário, influenciando diretamente sua **motivação, satisfação e engajamento** com o sistema.

A partir da criação de uma **base de dados sintética supervisionada**, buscou-se representar situações reais de jogo em que fatores como desempenho, número de vitórias e troféus conquistados pudessem indicar **estados emocionais distintos** (feliz, motivado, neutro e frustrado).  
Essa modelagem serviu como base para a exploração e classificação dos dados com diferentes algoritmos no Weka.

---

### 2. Interpretação Crítica dos Resultados

Os resultados obtidos demonstraram **altos índices de acurácia** entre os classificadores, especialmente **OneR e J48**, ambos com cerca de **99,5% de precisão**.  
Essa performance elevada decorre do fato de que o atributo `trofeus_delta` — responsável por expressar o desempenho do jogador — apresenta **forte correlação com o estado emocional**, sendo o principal determinante da classe-alvo.

No contexto de IHC, esse comportamento evidencia que **a experiência do usuário em ambientes digitais pode ser modelada a partir de padrões observáveis de comportamento e desempenho.**  
A variável `trofeus_delta` simboliza, nesse caso, um **indicador de feedback do sistema**, refletindo a percepção de sucesso ou fracasso do jogador.  
A predominância desse atributo nas classificações sugere que **as emoções dos usuários estão diretamente ligadas às respostas do sistema ao seu desempenho** — uma relação típica em interfaces que envolvem **interação competitiva e recompensas imediatas**.

Entretanto, a acurácia quase perfeita dos modelos também revela uma **limitação metodológica importante**:  
por se tratar de uma base sintética, os dados foram construídos com regras determinísticas, o que reduz a complexidade e a imprevisibilidade inerentes ao comportamento humano real.  
Em cenários autênticos de IHC, fatores como **frustração cumulativa, tempo de reação, contexto de uso e perfil psicológico** do jogador exerceriam influência significativa sobre as emoções, o que tornaria a classificação menos precisa e mais desafiadora.

---

### 3. Relação com o Domínio de IHC

A análise realizada reforça que **a emoção é um componente central da experiência do usuário** e deve ser considerada em todas as etapas de design, avaliação e adaptação de sistemas interativos.  
No caso de jogos digitais, compreender o estado emocional dos usuários permite:
- Ajustar o **nível de desafio** em tempo real, evitando desmotivação ou estresse excessivo.  
- Personalizar a **interface e as recompensas**, criando experiências mais satisfatórias.  
- Apoiar estudos de **usabilidade emocional**, que investigam como a interação influencia sentimentos e percepções.

Do ponto de vista de IHC, o experimento ilustra como técnicas de **aprendizado de máquina supervisionado** podem ser aplicadas para **identificar padrões emocionais e comportamentais** a partir de dados de interação, oferecendo uma ponte entre **engenharia de dados e ciência da experiência do usuário (UX).**

---

### 4. Considerações Finais

De forma crítica, os resultados indicam que a **modelagem de emoções em jogos é viável e tecnicamente mensurável**, porém ainda distante de capturar toda a complexidade emocional humana observada em interações reais.  
O estudo contribui para demonstrar que **o comportamento dos usuários pode ser quantificado e classificado**, mas também ressalta a importância de incorporar **dimensões qualitativas** em pesquisas futuras — como análise facial, resposta fisiológica ou feedback subjetivo — para representar melhor a natureza multifacetada da experiência humana.

Em suma, o trabalho evidencia que **Interação Humano-Computador e Inteligência Artificial podem atuar de forma complementar**, utilizando dados comportamentais para compreender e aprimorar a relação entre pessoas e sistemas digitais, fortalecendo a personalização, o engajamento e a satisfação do usuário final.

---

