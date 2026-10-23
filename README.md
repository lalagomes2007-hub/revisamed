# RevisaMed — protótipo gratuito

## O que esta versão faz
- Cria, edita, pesquisa e exclui flashcards.
- Programa revisão espaçada com intervalos de 1, 3, 7, 14 e no máximo 21 dias.
- Mostra quantos cartões estão vencidos e quantos foram revisados hoje.
- Guarda os dados no armazenamento local do navegador.
- Permite exportar/importar backup em JSON.
- Pode ser adicionada à tela inicial como web app quando publicada por HTTPS.

## Limitações importantes
Esta é a primeira versão individual. Não tem login, convite privado, sincronização entre aparelhos/pessoas nem notificações push programadas. Os dados ficam no navegador/aparelho em que os cartões foram criados. Use Exportar backup para não perder dados.

Para permitir contas privadas e sincronização, será preciso integrar autenticação e banco de dados. Para notificações push no iPhone/iPad, o site precisa estar instalado na tela inicial, o usuário deve autorizar notificações e o app precisa de um serviço de envio no servidor. Não prometa avisos pontuais sem testar essa parte.

## Publicar gratuitamente usando GitHub Pages
1. Crie/entre numa conta em https://github.com/
2. Clique em `+` > `New repository`.
3. Dê o nome `revisamed`, selecione `Public` e crie o repositório.
4. Dentro do repositório, use `Add file` > `Upload files`.
5. Extraia este ZIP no computador e envie `index.html`, `manifest.webmanifest` e `sw.js` (os arquivos, não a pasta externa).
6. Clique em `Commit changes`.
7. Abra `Settings` > `Pages`.
8. Em `Build and deployment`, selecione `Deploy from a branch`; escolha `main` e `/ (root)`; salve.
9. Aguarde a publicação. O endereço ficará no formato `https://SEU-USUARIO.github.io/revisamed/`.

**Privacidade:** um repositório público deixa o código visível. Não coloque senhas, dados pessoais ou cartões particulares no código. Os cartões deste protótipo ficam no aparelho, não no GitHub.

## Adicionar à tela inicial no iPhone/iPad
1. Abra o endereço publicado no Safari.
2. Toque em Compartilhar.
3. Escolha `Adicionar à Tela de Início`.
4. Se aparecer a opção para abrir como app web, ative-a.
5. Toque em `Adicionar`.

## Como usar
1. Entre em `Criar cartão`.
2. Informe matéria, pergunta e resposta.
3. Em `Revisar`, tente responder antes de revelar.
4. Escolha Difícil, Moderado ou Fácil.
5. Confira `Meus cartões` e exporte backups regularmente.

## Regras atuais
- Difícil: 1 dia
- Moderado: 3 dias
- Fácil: começa em 7 dias; se continuar acertando, dobra o intervalo, limitado a 21 dias.
