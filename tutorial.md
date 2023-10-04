O Git Flow é um modelo de fluxo de trabalho para o Git que define uma estrutura para o gerenciamento de branches em um repositório Git. Ele define algumas branches padrão e fornece um conjunto de convenções para criar, mesclar e nomear branches. Aqui estão os principais comandos do Git Flow:

<!-- trabalhando em um projeto existente -->
1. **Clonando repositório existente**: abra a pasta que recebera seu repositório clonado. E no terminal digite:

   ```shell
   git clone <nome-do-repositorio>
   ```

   Isso irá clonar o repositório emitente. Abra o projeto no vs code.

2. **Iniciando repositório local**: no terminal do vs code, inicie o git flow.

   ```shell
   git flow init
   ```

   Isso irá guiá-lo por algumas configurações iniciais, como as branches padrão (e.g., `master`, `develop`) e as convenções de nomenclatura.

   Desta forma voce também ja iniciara na branch developer.

3. **Criando atualizações para o projeto**: Crie uma nova feacture para criar atualizaçoes:

   ```shell
   git flow feature start <nomeDaAtualizaçao>
   ```

   Isso irá guiá-lo por algumas configurações iniciais, como as branches padrão (e.g., `master`, `develop`) e as convenções de nomenclatura.

   Desta forma voce também ja iniciara na branch developer.




<!-- Comandos principais -->
<!-- Comandos principais -->
<!-- Comandos principais -->
1. **Inicializar o Git Flow**: Para começar a usar o Git Flow em um repositório, você precisa inicializá-lo primeiro.

   ```shell
   git flow init
   ```

   Isso irá guiá-lo por algumas configurações iniciais, como as branches padrão (e.g., `master`, `develop`) e as convenções de nomenclatura.

2. **Iniciar uma nova funcionalidade**:

   ```shell
   git flow feature start <nome-da-funcionalidade>
   ```

3. **Finalizar uma funcionalidade**:

   ```shell
   git flow feature finish <nome-da-funcionalidade>
   ```

   Isso irá mesclar a funcionalidade de volta para a branch `develop` e excluí-la.

4. **Iniciar um hotfix (correção de bug)**:

   ```shell
   git flow hotfix start <nome-do-hotfix>
   ```

5. **Finalizar um hotfix**:

   ```shell
   git flow hotfix finish <nome-do-hotfix>
   ```

   Isso irá mesclar o hotfix para a branch `master` e `develop`, e também etiquetar a versão de lançamento.

6. **Iniciar um lançamento**:

   ```shell
   git flow release start <nome-do-lancamento>
   ```

7. **Finalizar um lançamento**:

   ```shell
   git flow release finish <nome-do-lancamento>
   ```

   Isso irá mesclar o lançamento para a branch `master`, criar uma etiqueta de versão e mesclar as alterações de volta para a `develop`.

8. **Verificar o status do Git Flow**:

   ```shell
   git flow status
   ```

   Esse comando mostrará o status atual do Git Flow, incluindo as branches em andamento.

9. **Publicar uma funcionalidade, hotfix ou lançamento**:

   ```shell
   git flow feature/hotfix/release publish <nome-da-branch>
   ```

10. **Puxar atualizações das branches remotas**:

   ```shell
   git flow feature/hotfix/release pull <nome-da-branch>
   ```

Esses são os principais comandos do Git Flow. Lembre-se de que é importante configurar e inicializar o Git Flow em seu repositório antes de começar a usá-lo. O Git Flow pode ser uma ferramenta útil para fluxos de trabalho mais complexos, como desenvolvimento de software em equipe, onde é necessário gerenciar recursos, correções de bugs e lançamentos de forma estruturada.