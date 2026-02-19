
=======
# AS_teste
Usado para realizar teste de automação para QA

Live Code — QA Pleno com Cypress

Bem-vindo ao desafio de automação! Este repositório já possui o projeto Cypress configurado. Sua missão é implementar os cenários de teste descritos abaixo.

Pré-requisitos
Certifique-se de ter instalado:

Node.js v22
npm
Git
"Iniciar o cypress com o comando que está no package.json

Todos deverá ser executado no ambiente de (https://stg-amei.amorsaude.tech/auth/login)

Cada spec deverá ter uma describe com nome apropriado e com 2 cenários descritos abaixo

Spec 1 — Login
Arquivo: cypress/e2e/login/login.cy.js

Cenário 1 — Login com credenciais válidas
Informar usuário e senha corretos e verificar o redirecionamento para a página inicial da aplicação.
Objetivo - Ser redirecionado para a URL > https://stg-amei.amorsaude.tech/ com confirmação

Cenário 2 — Login com senha inválida
Informar um email correto com senha incorreta e verificar a exibição de mensagem de erro. O usuário deve permanecer na tela de login.
Objetivo - Deverá receber via front a mensagem > Senha incorreta, por favor revise seus dados.

----------------------------------------------------------------------------------------------------------------

Spec 2 — Agendamento (Moderado)
Arquivo: cypress/e2e/agendamento/agendamento.cy.js

Cenário 1 — Criar agendamento com dados válidos
Preencher todos os campos obrigatórios e confirmar o agendamento. A confirmação deve ser exibida ao final.
Objetivo - Receber via Front a mensagem na tela > Agendamento criado com sucesso

Cenário 2 — Tentar criar agendamento sem paciente estar cadastrado informando um CPF novo
Submeter o formulário sem preencher os campos obrigatórios e verificar as mensagens de validação.
Objetivo - Receber via front 2 mensagens > Paciente não encontrado > Deseja cadastrar um novo paciente?

----------------------------------------------------------------------------------------------------------------

Spec 3 — Proposta (Díficil)
Arquivo: cypress/e2e/proposta/proposta.cy.js

Cenário 1 — Criar proposta com dados válidos
Preencher os campos da proposta corretamente e submeter. A proposta deve ser salva com sucesso.
Objetivo - Deverá receber via front a mensagem > Proposta salva com sucesso

Cenário 2 — Tentar criar proposta com dados inválidos
Preencher os campos com dados inválidos e verificar que os erros de validação são exibidos e a proposta não é criada.
Objetivo - Clicar na proposta sem declarar todos os campos obrigátorio e receber mensagem via front 2 mensagens > Erro ao salvar proposta > Selecione um parceiro.

----------------------------------------------------------------------------------------------------------------

Flash

Faça o básico para atingir o resultado esperado

----------------------------------------------------------------------------------------------------------------
Opcional

Descreva o seguinte cenário para teste Manual 

Usar o gherkin para descrever o cenario de senha incorreta usando...

Given
When
And (caso necessite)
Then
