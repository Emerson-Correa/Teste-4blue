##Bugs Encontrados

###Bug 1

**Título:** Sistema aceita a criação de conta sem o preenchimento dos campos.

**Descrição:** Na tela de criação de conta, caso não sejam preenchidos os campos, quando clicado o botão de criar conta, o sistema aceita a criação de conta como se os campos tivessem sido preenchidos. 

**Reproduzindo o erro:** Na tela inicial, deixar todos os campo em branco e clicar em criar conta, será exibida a mensagem "Conta criada com sucesso".(ver o vídeo: 4blue -Sistema aceita a criação de conta sem o preenchimento dos campos.mp4)

**Resultado Atual:** Sistema permite a criação de conta sem a entrada de dados.

**Resultado Esperado:** No processo de criação de conta, o sistema deve requisitar o preenchimento obrigatório para então aí sim, criar uma conta ou verificar se já é uma existente.

**Severidade:** Alta, pois compromete a integridade e a qualidade dos dados do sistema, causando diversos impactos técnicos tais como: falta de informações essenciais, inconsistência de dados, falhas em funcionalidades que dependem destas informações, etc.

**Prioridade:** Alta, pois ocorre em fluxo essência do sistema(neste caso, a criação de conta), compromete a confiabilidade da base de usuários, numerosos cadastros inválidos, etc.

--------------------------------------------------------------------------------------------------------------------------
###Bug 2

**Título:** Exibição de informações sensíveis no console do DevTools.

**Descrição:** Uma vez realizado o login, ao se utilizar a ferramenta do DevTools é possível visualizar as credenciais utilizadas.

**Reproduzindo o erro:** Logar no sistema, abrir a ferramenta DevTools(F12), clicar em Console e observar a exibição das credenciais nas linhas abaixo. (ver o vídeo: 4blue- Exibição de informações sensíveis no console do DevTools.mp4)

**Resultado Atual:** No uso do console é exibida as credenciais utilizadas pelo usuário.

**Resultado Esperado:** Que não sejam exibidas as credenciais do usuário no Console.

**Severidade:** Crítica. Pois mesmo usando https, expõe as credenciais utilizadas a qualquer pessoa que tenha acesso ao computador. É uma situação que viola princípios básicos de segurança da informação.

**Prioridade:** Alta. Pois afeta diretamente dados sensíveis do usuário, podendo acarretar em outros problemas, tais como vazamento de credenciais e a reputação do sistemas e/ou da empresa.

---------------------------------------------------------------------------------------------------------------------------
###Bug 3

**Título:** Erro de Login

**Descrição:** Após a criação de uma conta, ao se efetuar o login no sistema é exibida a mensagem "erro inesperado".
Fica evidenciado visualmente que entramos de fato no sistema, pela mensagem de "**Login realizado com sucesso**" e "**Você foi autenticado e já pode utilizar o sistema**". Uma vez logado, não é visível para o usuário as funcionalidades do sistema, restando somente como interação botão "**Sair da Conta**" e nada mais.

**Reproduzindo o erro:** Criar uma conta obedecendo os critérios para senha. Efetuar o login utilizando e-mail e senha previamente criados e observar o erro. (ver o vídeo: Erro de Login.mp4)

**Resultado Atual:** Efetuado o login, é exibida a mensagem de "erro inesperado" e não existe mais nenhuma funcionalidade disponível, a não ser a de sair da conta.

**Resultado Esperado:** É esperado que, ao se entrar no sistema o usuário consiga utilizar todas funcionalidades disponíveis para aquele perfil e que não ocorra mensagem de erro.

**Severidade:** Alta, pois mesmo o usuário entrando no sistema, ele não consegue utilizar nenhuma funcionalidade, exceto o botão de Sair da Conta.

**Prioridade:** Alta, pois este erro impede o uso da aplicação e precisa ser corrigido imediatamente.

------------------------------------------------------------------------------------------------------------------------------
###Bug 4

**Título:** Vazamento visual no layout

**Descrição:** Vazamento no layout(layout quebrado) na tela de criação de conta. Campos de preenchimento utrapassam o limite do formulário, porém o usuário consegue preencher normalmentee enviar os dados.   

**Reproduzindo o erro:** Na Tela inicial, clicar em criar conta e observar.(ver o vídeo: Vazamento apenas visual no layout.mp4)

**Resultado Atual:** Campos de preenchimento da tela de criação de conta com vazamento no layout.

**Resultado Esperado:** É esperado que a interface esteja com o seu layout visualmente harmônico, sem comprometer a tarefa a ser realizada pelo usuário.

**Severidade:** Baixa, uma vez que não impede a funcionalidade do sistema. 

**Prioridade:** Baixa, não sendo um tipo de vazamento que expõe dados sensíveis, não oferecendo impacto de segurança e privacidade.

----------------------------------------------------------------------------------------------------------------------------

##Bugs que devem ter prioridade de correção:

**Considerações:** 
Eu corrigiria primeiramente aquele que apresenta Severidade Crítica, pois este expõe os dados sensíveis do usuário.
Num segundo momento, eu faria correção no bug que aceita a criação de conta sem o preenchimento do formulário, pois interfere diretamente nos dados e nas funcionalidades que dependem deste dados, perdendo a confiabilidade do sistema e prejudicando a empresa e o seus clientes.

Sugestões de Melhoria: na tela de criação de conta, tornar visível a obrigatoriedade de preencher os campos, bem como a validação caso os dados inseridos já possuam cadastro, sinalizar a quem estiver preenchendo caso este evento ocorra.

