# Funcionalidades

## Usuários com as permissões

- Gerenciar Marcações
- Gerenciar Agendamento
- Gerenciar Agendas Profissionais
- Gerenciar Atendimentos Encaminhados
- Gerenciar Atendimentos

### As funcionalidades são:

#### Criar Novo Atendimento

**Quando clico em: Botão "Novo Atendimento"**

O que acontece:

- Abre um modal para cadastro de novo atendimento

Permite informar:

- Dados do paciente
- Tipo de prioridade (Normal ou Preferencial)
- Selecionar profissional

Ao salvar:

- O atendimento é criado com status "Criado"
- Gera número da senha automaticamente
- Exibe modal com a senha para impressão
- Atualiza a lista de atendimentos
- Chamar Paciente no Painel

**Quando clico em: Botão "Chamar no painel" (ícone de alto-falante)**

O que acontece:

- Envia comando para exibir o chamado no painel de TV/monitor
- Exibe nome do paciente e número da senha no painel
- Insere outros dados do paciente
- Exibe histórico de marcações do paciente
- Inicia timer de 12 segundos antes de permitir novo chamado
- Exibe barra de progresso visual no botão durante o timer
- Se o usuário tentar chamar antes do tempo, exibe mensagem:
"Aguarde X segundos para chamar novamente"
- Abre modal de atendimento automaticamente
- Opção de reencaminhar atendimento (aparece modal para selecionar profissional)

#### Atualizar

Quando outro usuário realiza uma ação:

- A lista é atualizada automaticamente sem precisar recarregar a aba

#### Atender em Outro Local

**Quando clico em: Toggle "Atender em outro local"**

O que acontece:

- Ativa modo de seleção de múltiplos profissionais
- Permite visualizar atendimentos de outros profissionais
- A lista é filtrada pelos profissionais selecionados
- Locais disponíveis dependem das permissões do usuário

#### Impressão de Senha

Quando um atendimento é criado:

Modal automático com dados da senha

Exibe:

- Número da senha
- Nome do paciente
- Unidade de atendimento
- Data e hora
- Após 500ms, inicia impressão automaticamente
- Formato otimizado para impressora térmica (80mm)

#### Atendimentos em andamento

Aba no topo da tela que mostra ou oculta todos os atendimentos em andamento e a quantidade de finalizados.

## Usuário com permissão

- Somente Marcação por UBS

### As funcionalidades são:

- Não consegue ver Atendimento Central de Marcação
- Só tem acesso à Central de Marcação
- Tem acesso à lista de pacientes
- Acesso a atendimentos CM
- Acesso à tela de procedimentos

#### Quando clico em: Fila de marcação

O que acontece:

- Aparece a fila das marcações com:
- Nome do paciente
- Data de registro
- Profissional solicitante
- Procedimento
- Ações

- Nas ações, existem os botões:
- Ver detalhes
- Comprovante
- Excluir

- É possível buscar paciente pelo:
- Nome
- CPF
- CNS

#### Opção avançada de filtros:

- Data inicial da marcação
- Data final da marcação
- É retorno?
- Classificação
- Unidade
- Categoria
- Procedimento
- Profissional solicitado

#### Botão que exibe relatórios:

Opções:

- Exportar fila em PDF
- Relatório por especialidade
- Relatório de produção por profissional

#### Em agendamentos confirmados

- Aparecem quase as mesmas opções da fila de marcação
- Adiciona, em filtros avançados, a opção Profissional executado
- Nas ações existem os botões:
- Ver detalhes
- Comprovante

#### Agendamentos finalizados

- Aparecem quase as mesmas opções da fila de marcação
- Adiciona, em filtros avançados, a opção Profissional executado
- Nas ações existem os botões:
- Ver detalhes
- Comprovante
- Comprovante de inscrição

## Usuário com permissão

- Setor Transporte

### As funcionalidades são:

- Tem acesso a atendimentos
- Tem acesso à agenda do setor de transporte
- Não aparecem todas as opções de atendimentos da Central de Marcação (não é possível criar um novo atendimento)

#### Ao apertar em: Exportar agenda

**O que acontece:**

- Cria um PDF com tudo que está marcado na agenda de transporte

#### Quando clico em: Nova agenda

**O que acontece:**

- Aparece um quadro para o usuário escrever:
- A descrição
- A data da nova agenda
- Quando a agenda é criada, aparece mensagem dizendo que a agenda de transporte foi criada com sucesso
- Opção de filtro por nome da agenda

#### Outras opções na interface

- Opção de ver agendas ativas
- Opção de mudar o dia do mês
- Opção de filtrar por nome da agenda
- Na lista de atendimentos aparecem todas as informações e o horário do paciente

#### Ao clicar em alguma agenda

**O que acontece:**

Abre um modal com as opções:
- Adicionar agendamento
- Nessa opção é possível agendar pelo:
- Nome do paciente
- CPF
- CNS
- Escolher o horário

Editar
- Edita a agenda já criada
- É possível mudar:
- Descrição
- Data

Gerar relatório
- Gera PDF com todos os pacientes contendo:
- Telefone
- Idade
- Assinatura