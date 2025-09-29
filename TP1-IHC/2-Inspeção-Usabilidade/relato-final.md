# Lista limpa (relato final)

A seguir está a lista limpa com soluções sugeridas e racional (por que corrigir a heurística e como impacta o usuário).

| ID | Localização | Problema (resumo) | Heurística | Recomendações de correção | Benefício esperado |
|----|-------------|-------------------|------------|----------------------------|--------------------|
| 01 | Tela de Login | Linguagem técnica e opções confusas no login (“Entrar com gov.br”, “Gerar código”). | 6, 10, 8, 2 | Usar termos simples (“Entrar com CPF e senha”), adicionar ícones e exemplos breves. | Facilita o login e reduz erros de usuários iniciantes. |
| 02 | Recuperação de Senha (fluxo direto) | Sistema envia usuário direto para recuperação sem permitir novas tentativas de senha. | 3, 5, 9, 2 | Permitir tentativas extras antes da recuperação; mostrar limite de tentativas. | Usuário mantém controle e evita frustração. |
| 03 | Cadastro de Nova Senha | Critérios de senha exibidos de forma intimidadora, sem exemplo prático. | 1, 5, 2, 8 | Mostrar exemplo válido e feedback visual positivo (verde) ao atender critérios. | Usuário cria senhas fortes com menos erros. |
| 04 | Identificação com CPF (erro de captcha) | Mensagens de erro técnicas como “ERL0000900” sem explicação. | 2, 9, 5, 1 | Exibir mensagens claras (“Erro no Captcha, tente novamente”). | Facilita diagnóstico e recuperação pelo usuário. |
| 05 | Assinatura Digital – Escolher Arquivo | Tela poluída, ícone de acessibilidade sobreposto ao texto, instruções pouco claras sobre formatos aceitos. | 8, 1, 2, 5 | Reorganizar layout, separar funções e destacar instruções. | Usuário entende rapidamente como assinar documentos. |
| 06 | Assinatura Digital – Inserção da Assinatura | Campo de inserção de assinatura não é claro. | 3, 6, 9, 8 | Destacar área de inserção com marcador visual. | Reduz erros e aumenta clareza da tarefa. |
| 07 | Caixa de Entrada de Mensagens | Usuário não consegue voltar após abrir mensagem; falta de navegação clara. | 3, 4, 1, 5 | Incluir botão “Voltar” ou breadcrumbs de navegação. | Usuário recupera o controle do fluxo facilmente. |
| 08 | Dados pessoais | Ícone “Home” leva para área diferente do esperado. | 4 | Padronizar destino do ícone conforme convenção de sistemas. | Evita confusão e retrabalho do usuário. |
| 09 | Assinar documentos digitalmente | Autenticação restrita apenas via app no login/assinatura. | 7, 3 | Oferecer alternativas (senha + token, SMS). | Garante inclusão e acesso de todos os perfis de usuários. |
| 10 | Comparação entre o Web e App | Diferenças de fluxo entre Web e App. | 4, 6, 7 | Unificar lógica e padronizar elementos visuais. | Usuário não precisa reaprender entre plataformas. |
| 11 | Tela Inicial | Tela inicial sobrecarregada de informações. | 8 | Reduzir elementos, priorizar principais serviços. | Melhor experiência inicial, navegação mais ágil. |
| 12 | Selecionar qualquer ação no site | Cada ação abre uma nova aba de navegação. Após realizar várias atividades, o usuário acaba com muitas abas abertas. | 7, 3 | Abrir ações na mesma aba, só usar nova aba quando necessário. | Reduz desorganização e perda de foco. |
| 13 | Tela de Recuperação de Conta | Ao tentar recuperar a conta pelo site, o usuário é redirecionado automaticamente para a loja de aplicativos para baixar o app Gov.br sem aviso prévio. | 3, 7 | Informar antes de redirecionar e oferecer opção. | Evita perda de contexto e melhora controle. |
| 14 | Login → Inserção de Senha | Mensagens de erro genéricas (“usuário/senha inválidos”). | 9 | Indicar causa provável (ex.: “Senha incorreta”). | Usuário corrige erro mais rapidamente. |
| 15 | Formulário de Serviço → Consultar Cadastro de Pessoa Física (CPF) na Receita Federal | Formulário aceita entradas inválidas (CPF com letras). | 5 | Validar campos em tempo real. | Previne erros antes de submissão. |
| 16 | Portal e-CAC (Receita Federal) | Interface do e-CAC inconsistente com gov.br. | 4 | Adotar padrão visual unificado. | Cria confiança e reduz reaprendizado. |
| 17 | Fluxo de inscrição para um serviço ou emissão de um documento. | Fluxos longos sem opção de cancelar/voltar. | 3 | Adicionar botões de “Cancelar” e “Voltar” em todas as etapas. | Dá autonomia e reduz frustração em erros. |
| 18 | Acesso a serviços federais específicos | Redirecionamentos para domínios externos sem aviso. | 4, 6 | Informar que usuário sairá do gov.br; manter padrão visual. | Aumenta confiança e consistência. |
| 19 | Fluxo de "Esqueci minha senha" | Recuperação de senha complexa (exige autenticação bancária etc.). | 3, 9 | Simplificar processo ou oferecer alternativas acessíveis. | Usuário recupera acesso sem barreiras excessivas. |
| 20 | Sistema SEI – navegação e localização de ações importantes | SEI com termos técnicos e navegação confusa. | 2, 6 | Usar linguagem simples e menus mais intuitivos. | Facilita uso por não especialistas. |
| 21 | Portal da Transparência / Portais governamentais – dificuldade de localização de informações | Informações do Portal da Transparência escondidas em menus profundos. | 6 | Reestruturar menus e destacar links principais. | Usuário encontra dados mais rapidamente. |
| 22 | Portal Brasileiro da Legislação – inconsistência visual e de estrutura | Inconsistência no Portal da Legislação. | 4 | Padronizar interface e navegação. | Reduz erros e melhora confiança. |
| 23 | Portal Brasil de Dados Abertos – personalização / customização limitada | O usuário não consegue adaptar ou personalizar a interface, configurar filtros ou atalhos etc. | 7 | Incluir opções de personalização da interface, filtros salvos, atalhos configuráveis e ajuste de visualização de dados. | Usuários frequentes realizam tarefas com mais rapidez e eficiência, reduzindo esforço e tempo de navegação. |
| 24 | Plataforma COTIC – feedback insuficiente | A plataforma não informa claramente ao usuário em que etapa ele está em certos fluxos ou se uma ação foi efetuada. | 1 | Exibir status claros de carregamento e conclusão. | Usuário sabe que ações foram registradas com sucesso. |
| 25 | Chatbot “Helô” do INSS – manutenção de contexto / compreensão de linguagem natural | Chatbot Helô perde contexto das conversas. | 5 | Melhorar lógica de fluxo e salvar histórico da interação. | Usuário recebe respostas mais consistentes e úteis. |

