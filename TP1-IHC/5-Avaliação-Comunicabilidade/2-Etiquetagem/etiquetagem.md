# 📝 Etiquetagem das Rupturas de Comunicação (MAC)

## Participante U1

| Tarefa | Timestamp | Etiqueta       | Trecho observado / Contexto               | Interpretação |
|--------|-----------|----------------|-------------------------------------------|---------------|
|       | 00:16     | Cadê?          | Usuário procurando onde digitar dados     | Falta de visibilidade do campo de entrada |
|     | 00:45     | E agora?       | Qual documento escolher                   | Dúvida sobre qual opção correta seguir |
|       | 02:31     | Epa!           | Site deslogou                             | Perda inesperada de sessão (logout automático) |
|       | 02:48     | Cadê?          | Procurando próxima tarefa                 | Usuário não encontra próximo passo |
|       | 03:00     | Cadê?          | Procurando serviços                       | Dificuldade em localizar opções de serviço |
|       | 03:48     | Assim não dá   | Demora no carregamento                    | Frustração com lentidão do sistema |
|        | 05:09     | O que é isto?  | Confusão sobre opção correta              | Incerteza quanto ao significado de uma opção |
|       | 05:15     | Pra mim está bom! | Achou as informações suficientes        | Usuário satisfeito parcialmente com resultado |
|        | 05:43     | E agora?       | Dúvida de navegação                       | Falta de orientação sobre próximos passos |
|        | 06:28     | E agora?       | Dúvida das opções                         | Opções pouco claras gerando incerteza |
|        | 08:09     | Onde estou?    | Incerteza se está na tela certa           | Falta de clareza na navegação |
|        | 08:43     | E agora?       | Informação pouco clara                    | Sistema não fornece feedback adequado |
|        | 09:00     | O que é isto?  | Confusão sobre opção correta              | Falta de consistência ou explicação das opções |
|        | 09:19     | Pra mim está bom! | Satisfação parcial                      | Usuário considera aceitável a informação apresentada |

---

# Etiquetagem – Participante 02

| Part. | Tarefa | Timestamp | Trecho observado                                                                 | Etiqueta MAC | Interpretação                                                                                     |
|-------|--------|-----------|----------------------------------------------------------------------------------|--------------|--------------------------------------------------------------------------------------------------|
| U1    | T1 - Login                  | 00:36 | Usuário afirma que não pode fazer a segunda parte da tarefa (recuperar senha) pois já estava logado automaticamente. | Assim não dá  | A configuração do teste (login salvo) impediu a realização de uma parte da tarefa.               |
| U1    | T3 - Assinar documento      | 00:48 | Usuário rola a página inicial para cima e para baixo, procurando visivelmente pelo serviço de assinatura. | Cadê? | O atalho para o serviço não estava em um local esperado pelo usuário.                           |
| U1    | T3 - Assinar documento      | 02:27 | Sistema exige um código enviado para outro aplicativo, forçando o usuário a sair do navegador para buscar a informação. | E agora? | O fluxo exigiu uma ação externa (verificar outro app), quebrando o processo e introduzindo uma etapa inesperada. |
| U1    | T4 - Emitir comprovante CPF | 03:30 | Usuário tenta sair da tela do assinador para iniciar uma nova tarefa e verbaliza: "Não tô conseguindo acessar a página inicial". | Onde estou? | A navegação entre os microsserviços do gov.br é confusa e não há um caminho de volta claro para a página principal. |
| U1    | T4 - Emitir comprovante CPF | 04:38 | Após várias tentativas frustradas de encontrar o serviço, o usuário desiste e afirma: "Essa tarefa número 4 não consegui fazer". | Desisto | O usuário abandonou a tarefa por completo, indicando uma falha grave na comunicação da interface. |
| U1    | T5 - Atualizar dados        | 04:51 | Usuário procura na tela inicial onde clicar para acessar seus dados pessoais, hesitando antes de encontrar o menu no topo. | Cadê? | A entrada para a área de perfil do usuário não é imediatamente óbvia na interface principal.     |
| U1    | T6 - Ver serviços acessados | 06:35 | Usuário encontra a seção "Consultar serviços solicitados", vê que está vazia e conclui que ali é o histórico. | O que é isto? | Um estado vazio na interface levou o usuário a uma interpretação possivelmente incorreta da funcionalidade. |
| U1    | T7 - Certificado de Vacinação | 09:35 | Usuário passa mais de dois minutos navegando por vários menus e fala: "Não tô achando o certificado, não". | Cadê? | A localização de um serviço muito popular não foi intuitiva, gerando uma busca longa e frustrante. |
| U1    | T8 - Informações Bolsa Família | 09:57 | Usuário inicia a busca pela informação, mas o vídeo termina antes que ele encontre ou desista. | (Inconclusivo) | A gravação foi interrompida antes da conclusão ou abandono da tarefa.                            |

--

# Consolidação Geral das Etiquetas

| Etiqueta MAC   | Part. | Tarefa(s) | Interpretação consolidada |
|----------------|-------|-----------|---------------------------|
| Assim não dá   | U1    | T1        | O login automático impediu a realização completa da tarefa de recuperação de senha. |
| Cadê?          | U1    | T3, T5, T7 | O usuário não encontrou facilmente atalhos e serviços importantes, gerando frustração. |
| E agora?       | U1    | T3        | O fluxo exigiu ações externas inesperadas, quebrando a continuidade do processo. |
| Onde estou?    | U1    | T4        | A navegação entre microsserviços foi confusa, sem clareza para retornar à página principal. |
| Desisto        | U1    | T4        | O usuário abandonou a tarefa, evidenciando falha grave na usabilidade. |
| O que é isto?  | U1    | T6        | Estados vazios e falta de clareza levaram a interpretações erradas. |
| (Inconclusivo) | U1    | T8        | A gravação foi interrompida antes da conclusão da tarefa. |



