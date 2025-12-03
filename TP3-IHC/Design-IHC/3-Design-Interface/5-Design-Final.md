# Design Final da Interface

Nesta etapa apresentamos o **design final da interface** do aplicativo GRAL, juntando todos os elementos visuais e conceituais definidos nas fases anteriores (nome e logotipo, paleta de cores, tipografia, ícones/ilustrações). O objetivo é mostrar de forma concreta como todas essas decisões visuais se materializam nas telas do sistema, evidenciando coerência estética, usabilidade e consistência de navegação.

## Coerência Visual e Identidade

Para garantir uma consistência sólida em todas as telas, aplicamos rigorosamente o guia de estilos definido anteriormente. A imagem abaixo demonstra a unificação da paleta de cores, a tipografia escolhida para legibilidade e a Logo do aplicativo, culminando em uma amostra da interface final.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/b07135c1-2bbc-4dab-947e-cc304570a641" />
---

## Detalhamento das Telas e Fluxos

Abaixo, apresentamos as telas principais do sistema, destacando as escolhas de design e recursos de acessibilidade.

### 1. Fluxo de Login e Recuperação de Acesso
Este fluxo foca na entrada segura e na facilidade de recuperação de conta, prevenindo erros do usuário.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/d4a522fa-40ca-462e-896e-5027a4dd29af" />

* **Descrição:**
    * **Tela de Login:** Utiliza máscaras de input (ex: formatação automática de CPF) para prevenir erros de digitação. O botão de ação primária "Confirmar Login" possui destaque visual claro.
    * **Recuperação:** Fluxo claro onde o usuário informa o e-mail e recebe um feedback imediato e visual (ícone de check verde e mensagem de sucesso) confirmando que a solicitação foi enviada.
---

### 2. Dashboard (Tela Principal)
O hub central do aplicativo, projetado para dar ao usuário uma visão geral imediata de sua situação.

<img width="408" height="678" alt="Image" src="https://github.com/user-attachments/assets/47ce0ef9-9573-473a-a53f-8623ce338a69" />

* **Descrição:**
    * A tela apresenta uma saudação personalizada ("Olá, formando(a)!") e *widgets* de acesso rápido para as funcionalidades mais críticas: Próximos Eventos, Status de Pagamentos e Checklist.
    * O uso de cores semânticas (verde para "Em dia", barra de progresso laranja) permite que o usuário entenda sua situação financeira e de tarefas com apenas um olhar.
---

### 3. Menu e Acessibilidade
Destaque para a preocupação com a inclusão e personalização da interface.

<img width="739" height="668" alt="image" src="https://github.com/user-attachments/assets/bd7b17e3-ebce-4b09-a0ae-b7d06c4d11c5" />


* **Descrição:**
    * O menu lateral oferece navegação rápida para todas as áreas do app.
    * **Funcionalidade de Acessibilidade:** Implementamos um modal específico que permite ao usuário "Aumentar Contraste", "Aumentar tamanho do texto" e ativar "Acessibilidade de mídia". Isso atende diretamente aos requisitos de inclusão, permitindo que usuários com baixa visão ajustem a interface às suas necessidades.
---

### 4. Fluxo de Envio de Documentos
Um processo passo a passo para simplificar uma tarefa burocrática.

<img width="799" height="677" alt="image" src="https://github.com/user-attachments/assets/1aab4e6d-a12a-4e50-b013-fd1805f01739" />


* **Descrição:**
    * O sistema divide a tarefa complexa em etapas menores (ex: "1 de 2: Foto", "2 de 2: Nome").
    * Há instruções claras sobre formatos aceitos (JPG, PNG) e botões grandes para interação, facilitando o toque em dispositivos móveis (*Lei de Fitts*).
---

### 5. Calendário e Eventos
Visualização da agenda da formatura.

<img width="833" height="675" alt="image" src="https://github.com/user-attachments/assets/8a6bdff0-b77a-4dfd-9c6e-a36d12a15b45" />


* **Descrição:**
    * Lista cronológica dos eventos (Aula da Saudade, Missa, Baile) com informações essenciais: data, horário, local e status de confirmação.
    * Botões de ação ("Confirmar presença") são proeminentes, incentivando a interação.
---

### 6. Gestão Financeira e Pagamentos
Transparência total sobre os custos e parcelas da formatura.

<img width="1339" height="737" alt="image" src="https://github.com/user-attachments/assets/1b69815d-336a-4140-9c67-5ed752eb740c" />


* **Descrição:**
    * Apresentação clara de valores: "Total pago" vs. "Pendente".
    * Métodos de pagamento (Pix, Cartão) são facilmente selecionáveis.
    * O histórico utiliza códigos de cores (Verde para "Pago", Vermelho/Laranja para "Pendente") para reduzir a carga cognitiva. O usuário não precisa lembrar o que pagou; o sistema mostra visualmente.
  
---

### 7. Checklist e Galeria de Mídias
Organização de tarefas e memórias.

<img width="1349" height="757" alt="image" src="https://github.com/user-attachments/assets/40d64756-a1a2-411e-866c-a6c1eb454f54" />


* **Descrição:**
    * **Checklist:** Utiliza *checkboxes* interativos para dar sensação de progresso e conclusão de tarefas obrigatórias.
    * **Mídias:** Uma galeria organizada onde o usuário pode baixar fotos e vídeos do evento (botão "Baixar tudo"), tangibilizando a entrega de valor da formatura.

---

## Protótipo Interativo

Para navegar pelo fluxo completo e visualizar as microinterações propostas, acesse o protótipo de alta fidelidade no Figma através do link abaixo:

🔗 **[Acessar Protótipo Navegável do GRAL no Figma](https://www.figma.com/design/IRafr4hfk50iPzYOgMx7vm/GRAL-Prototype?node-id=0-1&t=O3dFf2SAfMhwEEZv-1)**

---

## Conclusão

O design final do aplicativo **GRAL** atende aos objetivos de negócio e às necessidades dos usuários identificadas na fase de pesquisa. A interface final prioriza a clareza nas informações financeiras e burocráticas, ao mesmo tempo que oferece recursos robustos de acessibilidade, garantindo que a experiência da formatura seja inclusiva e organizada para todos os estudantes.
