# 🧩 Diagrama MoLIC — Partes Detalhadas

Este documento contém a explicação **parte a parte** do Diagrama MoLIC.  
Cada seção representa um recorte específico do diálogo entre:

- Formando (F)  
- Formando com Acessibilidade (FA)  
- Equipe Interna (EI)  

A divisão em partes facilita a compreensão do fluxo completo e permite analisar separadamente:

- Estados de conhecimento  
- Intenções do usuário  
- Respostas do sistema  
- Mediações  
- Interrupções  
- Alternativas de navegação

As partes abaixo seguem o mesmo recorte utilizado no arquivo visual enviado no GitHub.

---

# 🔷 Acesso ao Sistema


<img width="3555" height="3095" alt="Acessar o sistema drawio" src="https://github.com/user-attachments/assets/12ee838f-26a1-4785-92b3-3cce2b5c5fe0" />


---

### 📝 Descrição

Mostra o fluxo de entrada no app GRAL.
O usuário abre o app, informa dados de login (código da turma, CPF) e confirma.
O sistema valida as informações: se estiver certo libera o painel; se der erro, direciona para recuperar acesso.

---

# 🔷 Envio de documentos obrigatorios

<img width="2740" height="7405" alt="Enviar documentos obrigatorios (foto do quadro, nome do canudo) drawio" src="https://github.com/user-attachments/assets/e343f7f7-4aa3-451a-b307-761d488b0c15" />


---

### 📝 Descrição

Fluxo onde o usuário envia os documentos exigidos para a formatura.
Primeiro escolhe e envia a foto do quadro. Depois digita nome e sobrenome que irão no canudo.
Em seguida revisa tudo, pode editar foto ou nome caso esteja errado e confirma o envio.
O sistema salva os dados e finaliza.

---

# 🔷 Baixar fotos e videos

<img width="2305" height="7055" alt="Baixar fotos e vídeos drawio" src="https://github.com/user-attachments/assets/6805ea77-e83d-4919-b66d-a82396930645" />


---

### 📝 Descrição

Mostra como o usuário baixa mídias da plataforma.
Ele acessa a área de arquivos, escolhe a pasta (fotos ou vídeos) e o sistema prepara os arquivos.
Depois escolhe baixar por ZIP ou download direto, com acompanhamento de progresso.
Se houver falha ao carregar ou baixar, pode tentar de novo.

---

# 🔷 Acompanhar pagamentos, mensalidades e situação financeira

<img width="4795" height="6755" alt="Acompanhar pagamentos, mensalidades e situação financeira drawio" src="https://github.com/user-attachments/assets/e9d43439-bdc5-4e57-9c11-2a4c7b712461" />


### 📝 Descrição

Fluxo financeiro do aluno dentro do app.
O usuário abre a situação financeira, visualiza mensalidades pagas e pendentes.
Se tiver pendências, escolhe forma de pagamento (Pix ou cartão), o sistema valida saldo/crédito, processa e confirma o pagamento.
Ao final gera e disponibiliza comprovante.

---

# 🔷 Selecionar produtos para compra

<img width="1795" height="6755" alt="Selecionar produtos para compra drawio" src="https://github.com/user-attachments/assets/8dda1446-2583-4735-8a7c-55308858af7f" />


### 📝 Descrição

Representa o processo de compra na loja do sistema.
O usuário abre a lista de produtos, navega/filtra, seleciona um item e acessa informações.
Depois configura variação e quantidade e adiciona ao carrinho.
Se configuração estiver inválida, corrige antes de concluir.

---

# 🔷 Criar e atualizar eventos do calendário

<img width="4190" height="7355" alt="Criar e atualizar eventos do calendário drawio" src="https://github.com/user-attachments/assets/a9469712-a072-456f-97fc-e1b76c8ca1f0" />


---

### 📝 Descrição


Fluxo de gerenciamento de calendário.
O usuário abre o calendário e pode escolher criar um evento novo ou editar um existente.
No caso de criar: informa título, data/horário e descrição opcional, depois salva.
No caso de atualizar: seleciona evento, edita dados e salva alterações.
Inclui validação de erro (campos inválidos ou conflito de horário).

---

# 🔷 Visualizar pendências financeiras da turma

<img width="3155" height="5455" alt="Visualizar pendências financeiras da turma drawio" src="https://github.com/user-attachments/assets/992b3752-55f3-4551-8b34-cd0a13baf226" />


---

### 📝 Descrição

Fluxo do responsável/ADM para consultar finanças por turma.
Ele acessa o módulo, visualiza lista de turmas e o status geral (pendente/ok/parcial).
Depois seleciona uma turma específica e abre pendências e pagamentos daquela turma.
Os dois caminhos convergem na finalização com resumo e saída.

---

# 🔷 Cadastrar novos produtos na loja

<img width="2625" height="5505" alt="Cadastrar novos produtos na loja  drawio" src="https://github.com/user-attachments/assets/e8894aea-6bb5-4642-be2d-3a123bcc114e" />

Fluxo do administrador cadastrando produtos.
O ADM acessa o módulo, preenche nome, descrição, imagens, preço e estoque.
O sistema valida os dados; se algo estiver errado, volta para corrigir.
Depois revisa, confirma e o produto é registrado no catálogo com sucesso.
---

### 📝 Descrição



---

# 📌 Observações Finais

- Todas as partes do MoLIC estão diretamente ligadas aos **HTAs**  
- Toda interação modelada considera a **metamensagem**  
- Os fluxos completos permitirão gerar telas coerentes na etapa de **sketches**  

---

