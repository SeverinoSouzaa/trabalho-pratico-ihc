# Heurísticas de UX, Comunicabilidade e Acessibilidade

Esta seção apresenta a avaliação técnica da interface do aplicativo **GRAL**, focando na verificação da qualidade de interação proposta. O objetivo desta etapa é demonstrar como as decisões de projeto atendem aos requisitos fundamentais de **Usabilidade** (baseados nas 10 Heurísticas de Nielsen, **Comunicabilidade** (através da Engenharia Semiótica e signos metalinguísticos e **Acessibilidade**.

Abaixo, cada tela é analisada não pelo seu aspecto estético, mas pela sua eficiência de uso, prevenção de erros e capacidade de comunicar estados e feedbacks ao usuário. Detalhamos como signos estáticos e dinâmicos foram empregados para reduzir a carga cognitiva e como as diretrizes de acessibilidade foram integradas nativamente ao fluxo de tarefas dos formandos.

---

## 1. Fluxo de Acesso e Segurança

### Tela 01: Login (Acesso)
<img width="310" height="718" alt="image" src="https://github.com/user-attachments/assets/8835cb10-0b74-4a01-a3ee-f9de6d144ab3" />


É a tela de acesso inicial, solicitando o Código da Turma e o CPF. O design é direto, com ênfase no botão principal de ação. Este fluxo prioriza a eficiência para o aluno e a clareza na recuperação de erros.

**Heurísticas Atendidas:**
* **Eficiência de uso (H7):** Eliminamos a necessidade de senha. O uso do Código da Turma + CPF acelera o acesso para o usuário frequente.
* **Prevenção de Erros (H5):** O botão de ação "Confirmar Login" possui destaque visual (cor laranja), mas só é ativado após preenchimento, prevenindo cliques em branco.

**Comunicabilidade (Signos Metalinguísticos):**
* A mensagem "Sistema seguro • Dados protegidos" atua como um signo de confiança para tranquilizar o usuário sobre a segurança da aplicação.

**Acessibilidade:**
* Campos de texto com rótulos (*labels*) externos claros e alto contraste (texto branco sobre fundo escuro).

---

### Tela 02: Solicitação de Recuperação
<img width="344" height="745" alt="image" src="https://github.com/user-attachments/assets/98a75ec1-4926-469e-a50f-e5a269aa2b86" />


Inicia o processo de recuperação de acesso, solicitando o e-mail cadastrado e oferecendo a opção manual.

**Heurísticas Atendidas:**
* **Reconhecer, diagnosticar e se recuperar de erros (H9):** Oferece um caminho claro ("Solicitação manual") quando o usuário falha no login.

**Comunicabilidade (Signos):**
* O ícone de informação (i) é um signo que reforça a informação ou o estado de validação da tela.
* O botão "Enviar solicitação" é o signo de ação primário.
* O ícone de "Carta/Envelope" no topo funciona como signo estático reforçando que o processo envolve comunicação externa (e-mail).

**Acessibilidade:**
* O campo de texto para o e-mail é único e as instruções são separadas por parágrafos curtos, tornando a leitura mais fácil.

---

### Tela 03: Feedback de Recuperação
<img width="293" height="638" alt="image" src="https://github.com/user-attachments/assets/e5f5c323-294b-4d7b-b27e-e360c19fc575" />


É a tela de confirmação após o envio do pedido de recuperação de acesso.

**Heurísticas Atendidas:**
* **Visibilidade do Status do Sistema (H1):** O sistema fornece feedback imediato e explícito ("Solicitação Enviada") com um ícone de "Check" verde, tranquilizando o usuário.
* **Controle e liberdade do usuário (H3):** O botão "Voltar para o Login" oferece uma saída de emergência clara para reiniciar o fluxo.

**Comunicabilidade:**
* A mensagem é um signo de fecho de interação, estabelecendo a expectativa de tempo e confirmando o e-mail cadastrado.

---

## 2. Navegação e Personalização

Foco na orientação do usuário dentro do sistema.

### Tela 04: Dashboard (Home)
<img width="254" height="906" alt="image" src="https://github.com/user-attachments/assets/0a1475be-cdcf-4723-b142-b8d594f155a8" />


Esta é a tela inicial do aplicativo, que resume o status mais importante para o formando. O design é hierárquico, começando com uma saudação ("Olá, formando(a)!") e links rápidos (Documentos, Avisos), seguido pelos blocos de informação de "Próximos Eventos", "Pagamentos" e "Checklist".

**Heurísticas Atendidas:**
* **Visibilidade do estado do sistema (H1):** O usuário vê imediatamente que a contribuição está "Em dia" e em qual parcela se encontra ("7/12 parcelas"), além do progresso do Checklist ("2/3").
* **Reconhecimento em vez de lembrança:** O painel exibe o status atual de todas as áreas críticas (Próximo evento, Status financeiro, Checklist), para que o aluno não precise "lembrar" o que tem pendente.

**Comunicabilidade:**
* O texto "Em dia" com um marcador de bolha (sendo da cor verde, que comunica sucesso) é um signo de estado instantâneo.
* O ícone de seta (>) ao lado de "Pagamentos" atua como um signo de navegação, indicando que a seção é clicável.

**Acessibilidade:**
* O agrupamento de informações em blocos distintos facilita a leitura e o foco, minimizando a sobrecarga cognitiva.
* **UX Writing:** O uso do nome do usuário ("Olá, formando!") cria proximidade e personalização.

---

### Tela 05: Menu Lateral (Sidebar)
<img width="261" height="691" alt="image" src="https://github.com/user-attachments/assets/59d53f4a-aefb-4cf4-9706-1bec240de565" />


O menu de navegação completo (Menu Hambúrguer) lista todas as seções do aplicativo. O design é limpo, com cada item (Ex: Pagamentos, Documentos, Mídias) acompanhado de um ícone e espaçamento.

**Heurísticas Atendidas:**
* **Consistência e Padrões (H4):** Segue o padrão mental de menus móveis (lista vertical com ícones à esquerda).
* **Reconhecimento em vez de lembrança:** A lista permite reconhecimento das funcionalidades através dos nomes e ícones.

**Comunicabilidade:**
* Os ícones são signos icônicos que reforçam a semântica do texto (Ex: o ícone do Checklist ou da Loja GRAL).
* O botão de fechar (X) e o botão "Ver Perfil >" são signos de controle e navegação.

**Acessibilidade:**
* Ícones acompanham o texto, auxiliando usuários com dificuldades de leitura ou dislexia a identificarem a função pela forma visual.
* O tamanho da área de toque de cada item da lista (botões) é grande, facilitando a seleção precisa.

---

### Tela 06: Modal de Acessibilidade
<img width="378" height="770" alt="image" src="https://github.com/user-attachments/assets/00d2493a-b1bd-48d2-806e-0177cf131a58" />


Esta tela é dedicada exclusivamente a configurações de interface para adaptação do usuário. O design apresenta opções de ativação/desativação claras para alto contraste e tamanho do texto.

**Heurísticas Atendidas:**
* **Flexibilidade e Eficiência de Uso (H7):** Atendida ao permitir que o usuário personalize a interface de acordo com suas necessidades. O uso de *toggles* ou botões de alternância comunica o estado atual da funcionalidade (Ex: "Desativado").
* **Controle e liberdade do Usuário (H3):** O botão "X" e a área de fundo escurecida permitem fechar o modal facilmente (saída de emergência).

**Comunicabilidade:**
* O termo "Desativado" ao lado das funções de contraste e acessibilidade de mídia é um signo de feedback textual imediato sobre o estado da configuração.

**Inclusão (Persona Beatriz):**
* Esta tela é o coração da acessibilidade do app. Permite ao usuário ativar "Alto Contraste" e "Aumentar Texto" sem depender das configurações nativas do celular.

---

## 3. Fluxo Financeiro

Foco na transparência e redução da ansiedade financeira.

### Tela 07: Visão Geral Financeira
<img width="286" height="576" alt="image" src="https://github.com/user-attachments/assets/63ad1a67-6d6f-4764-b4cc-08bc6b452989" />


Exibe o panorama financeiro, detalhando o status da contribuição, valores pagos/pendentes e o histórico das parcelas pagas.

**Heurísticas Atendidas:**
* **Visibilidade do Status do Sistema (H1):** O uso de uma barra de progresso visual ("Contribuição 7/12") e a etiqueta "Em dia" (verde) comunicam a saúde financeira do aluno em segundos.
* **Reconhecimento em vez de lembrança (H6):** Facilitado pelo botão "Baixar comprovante" visível em cada parcela.

**Comunicabilidade:**
* Cores semânticas (Verde = Pago/OK, Laranja = Ação necessária) são signos dinâmicos essenciais.

**Acessibilidade:**
* A repetição do padrão de informação por parcela (Número, Data, Valor, Status) garante que a lista seja altamente previsível e legível.

---

### Tela 08: Lista de Parcelas (Scroll)
<img width="319" height="619" alt="image" src="https://github.com/user-attachments/assets/d2f5d30f-3a74-41da-a726-0f4eebfd3f4d" />


Exibe o panorama financeiro, detalhando o status da contribuição, valores pagos/pendentes e o histórico das parcelas futuras (Pendentes).

**Heurísticas Atendidas:**
* **Visibilidade do estado do sistema (H1):** Reforçada com a exibição do "Total pago" e o "Pendente" em valores absolutos.
* **Consistência e Padrões (H4):** Mantida na formatação das informações de cada parcela (Vencimento, Valor, Status).
* **Design Minimalista (H8):** A lista apresenta apenas as informações essenciais (Mês, Valor, Vencimento e Status), evitando poluição visual.
* **Consistência:** O botão "Pagar agora" repete o padrão visual de ação principal, reduzindo a curva de aprendizado.

**Acessibilidade:**
* A clareza das etiquetas ("Parcela 8/12", "Vencimento: 05/08/2024") garante que a informação complexa seja acessível e de fácil compreensão.

---

### Tela 09: Modal de Pagamento
<img width="356" height="829" alt="image" src="https://github.com/user-attachments/assets/18ef3493-1af6-4d9b-b98f-eaa6747e25d3" />


Permite ao usuário escolher entre PIX ou Cartão para quitar uma parcela pendente.

**Heurísticas Atendidas:**
* **Ajuda e Documentação (H10):** Dada pelas dicas abaixo das opções (Ex: "Confirmação em minutos" para PIX e "Crédito ou débito" para Cartão), que ajudam na tomada de decisão.
* **Prevenção de Erros (H5):** O sistema força uma escolha explícita do método (Pix ou Cartão) antes de processar, evitando cobranças indesejadas.

**Comunicabilidade:**
* As opções de pagamento são signos de ação futuros (clicar em um leva ao fluxo de pagamento).
* O ícone de seta (>) no final de cada opção comunica que ao tocar haverá uma transição de tela.

**Acessibilidade:**
* Cada opção de pagamento é um grande bloco de toque, o que é crucial para garantir que a transação seja iniciada corretamente.

**UX:**
* O modal sobreposto (em vez de nova tela) mantém o contexto do usuário, que ainda consegue ver qual parcela está pagando.

---

## 4. Tarefas e Mídias

Foco na execução de tarefas complexas de forma simples.

### Tela 10: Envio de Documentos
<img width="258" height="649" alt="image" src="https://github.com/user-attachments/assets/b0f87dc2-98ad-4453-9220-a4d93a1603a6" />


Tela de formulário para envio de documentos obrigatórios e informações personalizadas (Nome para o canudo).

**Heurísticas Atendidas:**
* **Prevenção de Erros (H5):** Manifestada ao listar os formatos aceitos: "Formatos aceitos: JPG, PNG".
* **Prevenção de Erros (H5):** O botão final não é "Enviar", mas sim "REVISAR DADOS". Isso força uma etapa cognitiva de conferência, crucial para evitar erros em dados de diploma.

**Comunicabilidade:**
* O ícone de câmera centralizado com a chamada "Toque para selecionar" é um signo icônico que guia o usuário na ação de upload e os *placeholders* ("Ex: Lucas") instruem o usuário sobre o formato esperado dos dados.

**Acessibilidade:**
* As instruções são numeradas e separadas por títulos, melhorando a clareza e o foco.
* O uso de dicas de campo (Ex: "Digite seu primeiro nome") auxilia o usuário.

---

### Tela 11: Calendário de Eventos
<img width="289" height="570" alt="image" src="https://github.com/user-attachments/assets/a293364f-bee4-43d7-ae22-60f90ea393c7" />


Lista de eventos da formatura com detalhes e status de presença.

**Heurísticas Atendidas:**
* **Visibilidade do estado do sistema (H1):** Atendida ao mostrar o status da presença (Ex: "Presença confirmada" ou o botão "Confirmar presença" necessário) para cada evento.
* **Compatibilidade entre o sistema e o mundo real (H2):** Ordenação cronológica lógica (do evento mais próximo para o mais distante).

**Comunicabilidade:**
* Ícones de relógio (horário) e o pin de mapa (local) são signos icônicos que representam de forma universal as informações de tempo e espaço.
* O botão "Confirmar presença" é um signo de ação claro.

**Acessibilidade:**
* Optamos por uma Lista Vertical (Timeline) em vez de uma grade de calendário. Isso facilita a navegação sequencial por leitores de tela (*TalkBack*), beneficiando a persona Beatriz.

---

### Tela 12: Galeria de Mídias
<img width="292" height="640" alt="image" src="https://github.com/user-attachments/assets/b48374c1-9d2c-4bc9-9855-7992123673ca" />


Área para visualização e download de fotos e vídeos da formatura, com opções de filtragem e download em lote.

**Heurísticas Atendidas:**
* **Flexibilidade e Eficiência de Uso (H7):** Inclusão de botões "Aceleradores": "Baixar tudo (ZIP)". Isso permite que usuários experientes (Lucas) realizem uma tarefa complexa (salvar centenas de fotos) com um único clique e permitindo ao usuário escolher como e o que baixar.

**Comunicabilidade:**
* O ícone de download (seta para baixo) no botão laranja é um signo icônico que reforça a função do botão de forma universal. Os filtros "Todas", "Studio Day" atuam como signos de organização.

**Organização:**
* Uso de pílulas de filtro (*Tags*) para segmentar o conteúdo por evento.

---

### Conclusão

O design do aplicativo **GRAL** se destaca pela sua usabilidade, graças à visibilidade do estado do sistema (progresso de pagamentos e checklist) e à consistência na interface. A Comunicabilidade é forte, utilizando cores como signos de estado (verde para sucesso) e ícones claros para reforçar ações.

O aplicativo demonstra um foco robusto em Acessibilidade com seu Menu de Acessibilidade dedicado, que permite a personalização do contraste e do tamanho do texto, garantindo uma experiência de usuário inclusiva e eficiente.
