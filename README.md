# labdio-4
Lab dio 4

A criação de bots e assistentes virtuais na Azure, é bastante intuitiva, e permite ser analisado todos os contextos envolvidos com a concepção e fala.

O processo :

Gerenciando recursos
Quando você cria um recurso de bot, o Azure cria recursos associados. Alguns dos recursos criados dependem de como você decide gerenciar a identidade do seu bot.

Sua identidade de bot pode ser gerenciada no Azure de diversas maneiras.

Como uma identidade gerenciada atribuída pelo usuário, você não precisa gerenciar as credenciais do bot por conta própria.
Como um aplicativo de locatário único.
Como um aplicativo multilocatário.
O suporte para a identidade gerenciada atribuída pelo usuário e os tipos de aplicativo de locatário único foi adicionado ao SDK do Bot Framework para C#, JavaScript e Python. Esses tipos de aplicativo não têm suporte em outras linguagens ou no Bot Framework Composer, no Bot Framework Emulator ou nos Dev Tunnels.

Criar o recurso
Crie o recurso Bot do Azure, que permitirá a você efetuar o registro do seu bot no Serviço de Bot de IA do Azure.

 Dica

Não é possível criar novos recursos do Bot de aplicativo web e do Registro de Canais de Bot, no entanto, qualquer recurso existente que esteja configurado e implantado continuará a funcionar. Os bots criados usando um modelo VSIX ou Yeoman do SDK versão 4.14.1.2, ou versões posteriores, contêm modelos do ARM que gerarão um recurso de Bot do Azure.

Acesse o portal do Azure.

No painel à direita, selecione Criar um recurso.

Na caixa de pesquisa, insira bot e pressione Enter.

Selecione o cartão do Bot do Azure.

Selecione o recurso de bot do Azure

Selecione Criar.

Insira valores nos campos obrigatórios e revise e atualize as configurações.

Forneça informações em Detalhes do projeto. Selecione se o bot terá residência de dados global ou local. Atualmente, o recurso de residência de dados local está disponível para recursos na região "europa ocidental" e "centralíndia". Para obter mais informações, confira como Regionalização no Serviço de Bot de IA do Azure.

O projeto detalha as configurações de um recurso de Bot do Azure

Forneça informações no ID do Aplicativo da Microsoft. Selecione como a identidade do bot será gerenciada no Azure e se deseja criar uma nova identidade ou usar uma existente.

As configurações de ID do aplicativo da Microsoft para um recurso de Bot do Azure

Selecione Examinar + criar.

Se os testes de validação forem aprovados, selecione Criar.

Assim que a implantação for concluída, selecione Ir para o recurso. Você deve ver o bot e os recursos relacionados listados no grupo de recursos selecionado.

Se você ainda não tem o SDK do Bot Framework, selecione Fazer download usando o GitHub para saber como consumir os pacotes de seu idioma preferido.

Criar bot no SDK

Agora, você está com tudo pronto para desenvolver o bot com o SDK do Bot Framework.

-----

Como obter a ID do aplicativo ou do locatário
Para obter a ID do aplicativo ou do locatário do bot:

Acesse a folha de recursos do Bot do Azure para seu bot.
Acesse a folha Configuração do bot. Nessa folha, é possível copiar a ID do Aplicativo da Microsoft ou a ID do aplicativo do Locatário do bot.
Para gerar uma nova senha
Os bots de locatário único e de multilocatário têm um segredo ou uma senha para o aplicativo que você precisa para efetuar algumas operações. O Serviço de Bot de IA do Azure oculta o segredo do bot. No entanto, o proprietário do recurso de Serviço de Aplicativo do bot pode gerar uma nova senha:

Acesse a folha de recursos do Bot do Azure para seu bot.
Acesse a folha Configuração do bot.
Selecione Gerenciar, ao lado da ID do Aplicativo da Microsoft, para acessar a folha Certificados + segredos do serviço de aplicativo.
Siga as instruções na folha para criar um novo segredo do cliente e registrar o valor em um local seguro.


Informações de identidade do bot
Siga estas etapas para adicionar informações de identidade ao arquivo de configuração do bot. O arquivo difere dependendo da linguagem de programação usada para criar o bot.

----

Para atualizar seu serviço de aplicativo
Se você tiver um recurso de serviço de aplicativo existente (aplicativo Web) para o bot e o bot for um aplicativo de identidade gerenciada atribuída pelo usuário, poderá ser necessário atualizar o serviço de aplicativo do bot:

Acesse a folha Serviço de Aplicativo do aplicativo Web do bot.
Em Configurações, selecione Identidade.
Na folha Identidade, selecione a guia Atribuído pelo usuário e Adicionar (+).
Na folha Adicionar a identidade gerenciada atribuída pelo usuário:
Selecione sua assinatura.

Para Identidades gerenciadas atribuídas pelo usuário, selecione a identidade gerenciada para seu bot. Se a identidade gerenciada foi gerada automaticamente para você, ela terá o mesmo nome do seu bot.

Selecione Adicionar para usar essa identidade para o bot.

A folha Identidade do Serviço de Aplicativo com a identidade gerenciada do bot selecionada.

Como obter a ID do aplicativo ou do locatário
Para obter a ID do aplicativo ou do locatário do bot:

Acesse a folha de recursos do Bot do Azure para seu bot.
Acesse a folha Configuração do bot. Nessa folha, é possível copiar a ID do Aplicativo da Microsoft ou a ID do aplicativo do Locatário do bot.
Para gerar uma nova senha
Os bots de locatário único e de multilocatário têm um segredo ou uma senha para o aplicativo que você precisa para efetuar algumas operações. O Serviço de Bot de IA do Azure oculta o segredo do bot. No entanto, o proprietário do recurso de Serviço de Aplicativo do bot pode gerar uma nova senha:

Acesse a folha de recursos do Bot do Azure para seu bot.
Acesse a folha Configuração do bot.
Selecione Gerenciar, ao lado da ID do Aplicativo da Microsoft, para acessar a folha Certificados + segredos do serviço de aplicativo.
Siga as instruções na folha para criar um novo segredo do cliente e registrar o valor em um local seguro.

Deste modo podemos realizar tarefas mais rapidas e fácil com maior acertividade 
