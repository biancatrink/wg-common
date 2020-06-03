# Como Contribuir?

## O que é este documento?

Este documento descreve um processo genérico de contribuição e aplica-se a todos os repositórios CHAOSS. Cada repositório pode ter diretrizes exclusivas específicas para o projeto.

* Definição de métricas.Para cada métrica, temos um documento descrevendo-o, todos eles no [diretório de métricas] (métricas). Você pode contribuir ajudando a refinar essas definições de métricas.

## Onde posso contribuir?

Qualquer pessoa pode contribuir com o CHAOSS em qualquer de nossos canais de comunicação. Veja em <https://chaoss.community/participate/>.

* Se você acha que algo deve ser feito (incluindo uma contribuição sua), abra uma issue neste repositório. Isso permitirá que outras pessoas leiam que você acha que algum trabalho deve ser feito e possam comentar sobre isso. Se você pretende fazer o trabalho sozinho, por favor diga isso.

* Todos que possuem uma opinião sobre o assunto devem comentar a issue, explicar como eles apóiam a idéia, propor alguma mudança ou opinar que não vale a pena ou que não é o momento para fazê-lo.

* Se os comentários forem positivos e um certo consenso for alcançado, proponha um Pull Request com as alterações no repositório (novo documento, alterações nos documentos existentes).

* Todos os que têm uma opinião sobre o Pull Request devem comentá-lo e revisões detalhadas devem ser feitas, talvez solicitando novas versões do Pull Request. Quando os comentários e as críticas forem positivos, a alteração será mesclada no repositório.

* Se o consenso não for alcançado em nenhum desses pontos ou se o processo parar, ele poderá ser levantado durante uma das reuniões do Grupo de Trabalho Comum ou na lista de discussão para tentar retomá-lo.

## Qual canal devo usar?
1. Lista de discussão
2. Submissão de Issue
3. Pull requests

### Conversas e contribuições de alto nível (email, call, f2f)

Instruções estratégicas, esclarecimentos de escopo e idéias em um estágio inicial são melhor discutidos na lista de discussão e nas reuniões. Veja <https://chaoss.community/participate/>.

### Contribuições de erros e novas funcionalidades (issue)

Erros e novas funcionalidades específicas são melhor discutidas atrav;es de um issue no repositório que elas pertencerem.

### Contribuições de alteração de código ou de documentação (pull request)

As alterações nos arquivos de código-fonte ou de documentação são melhor contribuídas e discutidas em Pull Request. Por favor, consulte os arquivos CONTRIBUTING.md para obter detalhes específicos do repositório.

Nesse processo, verifique se a sua [conta do GitHub][ssh] está configurada com um [fork][fork] e então localmente faça um [clone][clone] do repositório:

    git clone git@github.com:<your-username>/<repository>.git

Crie uma [feature branch][fb] no seu repositório local:

    git checkout -b <branch>

Faça a sua mudança e um commit da alteração:

    git add <changed file>
    git commit -m "<description of change>"

Faça um Push do seu fork no GitHub:

    git push origin <branch>

Então, [submeta um pull request][pr] nn GitHub para o repositório do CHAOSS.

[ssh]: https://help.github.com/articles/connecting-to-github-with-ssh/
[fork]: https://help.github.com/articles/fork-a-repo/
[fb]: https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow
[pr]: https://github.com/thoughtbot/factory_girl_rails/compare/
[clone]: https://help.github.com/articles/cloning-a-repository/

Neste ponto, você está aguardando os mantenedores do repositório CHAOSS. Eles comentarão seu Pull Request dentro de três dias úteis (e, normalmente, um dia útil).

Os mantenedores do repositório CHAOSS reportarão sobre Issues em aberto e Pull Requests nas [reuniões e listas de e-mails] [participate] para obter feedback da comunidade.

[participate]: https://chaoss.community/participate/

## Committing de volta ao repositório
## DCO e Sign-Off para contribuições

O [CHAOSS Charter](https://github.com/chaoss/governance/blob/master/project-charter.md) requer que as contribuições sejam feitas com um [Developer Certificate of Origin](http://developercertificate.org) sign-off.
Para garantir isso, um bot verifica todas as confirmações recebidas.

Para usuários que trabalham com linha de comando, o sign-off é realizado com um `-s` no comando commit:

```
git commit -s -m 'This is a commit message'
```

Para usuários da interface do GitHub (usando o botão "editar" em qualquer arquivo e produzindo uma confirmação a partir dele), o sign-off é feito por escrito:

```
Signed-off-by: Your Name <YourName@example.org>
```

em uma mesma linha, no campo de comentário do commit. Isso pode ser automatizado através de um plugin no navegador como 
[DCO GitHub UI](https://github.com/scottrigby/dco-gh-ui).

#### Procedimento para usar o plugin DCO no navegador
O [DCO browser plugin](https://github.com/scottrigby/dco-gh-ui) é uma ferramenta útil para automatizamente assinar commits usando o GitHub. 
Para habilitar este plugin: 

- Entre na página do plugin em [chrome web store](https://chrome.google.com/webstore/detail/dco-github-ui/onhgmjhnaeipfgacbglaphlmllkpoijo).
- Alternativamente, entre na [página de addon do Firefox](https://addons.mozilla.org/en-US/firefox/addon/scott-rigby/) para adicionar a extensão ao seu navegador.
- Depois de adicionar a extensão, clique com o botão direito do mouse na extensão na barra de ferramentas do seu navegador e selecione `Opções`. 
- Uma caixa de diálogo será aberta como mostrado abaixo. Preencha seu nome no GitHub (não o identificador) e o email.

 ![Tela das configurações do DCO GitHub UI](https://user-images.githubusercontent.com/31214064/55411911-194c8500-5584-11e9-8b56-c8f94b6fa213.png)

- Então, sempre  que você fizer um commit no GitHub, a linha `Signed-off-by: Seu Nome <Seuemail>` automaticamente aparecerá na descrição do commit ao fazer alterações em um arquivo como exemplificado abaixo. Uma mensagem de commit pode ser adicionada às linhas abaixo do sign-off que foi automaticamente gerado. 

![Tela do GitHub UI com sign-off automaticamente gerado na mensagem de commit](https://user-images.githubusercontent.com/31214064/55423206-127d3c80-559b-11e9-9a5e-6300105b8858.png)

- Depois de executar o commit e enviar o Pull Request, o commit será verificado e aprovado pelo bot do DCO.

 ![Tela de verificação com sucesso do DCO](https://user-images.githubusercontent.com/31214064/55415829-5f591700-558b-11e9-93ae-07b0ed432a53.png)


## Quem é o mantenedor do repositório do CHAOSS?

O README.md do repositório contém uma lista dos mantenedores. Cada repositório CHAOSS reúne pessoas diferentes e documenta no CONTRIBUTING.md específico do repositório como alguém se torna um mantenedor em seu repositório.

## E sobre releases?

Os mantenedores dos repositórios do CHAOSS marcam os commits no master branch como [releases][rl] (snapshots). Cada repositório CHAOSS possui sua própria cadência de releases. Entre as releases, o master branch está em desenvolvimento.

[rl]: https://help.github.com/articles/about-releases/
