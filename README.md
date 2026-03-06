Título: Sistema aceita a criação de conta sem o preenchimento dos campos.

Descrição: Na tela de criação de conta, caso não sejam preenchidos os campos, quando clicado o botão de criar conta, o sistema aceita a criação de conta como se os campos
tivessem sido preenchidos. 

Reproduzindo o erro: Na tela inicial, deixar todos os campo em branco e clicar em criar conta, será exibida a mensagem "Conta criada com sucesso".(ver vídeo)

Resultado Atual: Sistema permite a criação de conta sem a entrada de dados.

Resultado Esperado: No processo de criação de conta, o sistema deve requisitar o preenchimento obrigatório para então aí sim, criar uma conta ou verificar se já é uma existente.

Severidade: Alta, pois compromete a integridade e a qualidade dos dados do sistema, causando diversos impactos técnicos tais como: falta de informações essenciais, inconsistência de dados, falhas em funcionalidades que dependem destas informações, etc.

Prioridade: Alta, pois ocorre em fluxo essência do sistema(neste caso, a criação de conta), compromete a confiabilidade da base de usuários, numerosos cadastros inválidos, etc.

--------------------------------------------------------------------------------------------------------------------------

Título: Exibição de informações sensíveis no console do DevTools.

Descrição: Uma vez realizado o login, ao se utilizar a ferramenta do DevTools é possível visualizar as credenciais utilizadas.

Reproduzindo o erro: Logar no sistema, abrir a ferramenta DevTools(F12), clicar em Console e observar a exibição das credenciais nas linhas abaixo. (ver vídeo)

Resultado Atual: No uso do console é exibida as credenciais utilizadas pelo usuário.

Resultado Esperado: Que não sejam exibidas as credenciais do usuário no Console.

Severidade: Crítica. Pois mesmo usando https, expõe as credenciais utilizadas a qualquer pessoa que tenha acesso ao computador. É uma situação que viola princípios básicos de segurança da informação.

Prioridade: Alta. Pois afeta diretamente dados sensíveis do usuário, podendo acarretar em outros problemas, tais como vazamento de credenciais e a reputação do sistemas e/ou da empresa.

---------------------------------------------------------------------------------------------------------------------------
