# br.svelte.dev

Repositório de tradução do site `svelte.dev` para o português brasileiro. Ele é totalmente baseado no [template de tradução](https://github.com/sveltejs-translations/template-svelte.dev) feito pelo pessoal da [Rússia](https://ru.svelte.dev).


## O que deve ser traduzido
* [Tutorial](https://svelte.dev/tutorial) no Svelte V3 ([GitHub](https://github.com/sveltejs/svelte/tree/master/site/content/tutorial))
* [Documentação](https://svelte.dev/docs) no Svelte V3 ([GitHub](https://github.com/sveltejs/svelte/tree/api-reference/site/content/docs))
* [Documentação](https://sapper.svelte.technology/guide) por Sapper ([GitHub](https://github.com/sveltejs/sapper.svelte.technology/tree/master/content/guide))
* [Exemplos](https://svelte.dev/repl) ([GitHub](https://github.com/sveltejs/svelte/tree/master/site/content/examples))
* [Blog](https://svelte.dev/blog) ([GitHub](https://github.com/sveltejs/svelte/tree/master/site/content/blog))
* Conteúdo do site [svelte.technology](https://svelte.dev) ([GitHub](https://github.com/sveltejs/svelte/tree/master/site/src))
* Conteúdo do site [sapper.svelte.technology](https://sapper.svelte.technology) ([GitHub](https://github.com/sveltejs/sapper.svelte.technology/tree/master/src))
* Conteúdo do site [svelte-native.technology](https://svelte-native.technology) ([GitHub](https://github.com/halfnelson/svelte-native/tree/master/docs_src/content))


## Como funcionam as traduções?

O processo de tradução utiliza o [translation-patcher](https://www.npmjs.com/package/trpatcher). Para executar, basta digitar isso no terminal:

```shell
$ npm run dsa
```

Este comando irá fazer o download, instalar as dependencias e sobrescrever os arquivos pelos que estiverem traduzidos no diretório `patch`.

Então você poderá rodar o site no modo de desenvolvimento:

```shell
$ npm run dev
```

No seu navegador, acesse o endereço http://localhost:3000 para ver o site traduzido rodando.

O conteúdo traduzido encontra-se na pasta `patch`. Procure mantê-los atualizados e adicione nela os novos conteúdos traduzidos.

*Dica*: Você pode copiar os arquivos da pasta gerada automaticamente `__BUILD`. Nela encontram-se os arquivos atualizados no momento em que você executou os comandos `npm run dsa` ou `npm run download`.

Há também o arquivo `strings.json` na pasta `patch`. Neste arquivo, você pode escrever as traduções baseando-se nas _strings_ de cada página. O `trpatcher` irá substituir as strings pelo texto traduzido nestes arquivos, é muito útil quando a lógica de componentes do site muda com o tempo mas o texto continua lá.

Quando o site estiver rodando no modo `dev`, toda vez que modificar um arquivo no diretório `patch` eles serão mesclados com os arquivos originais. Então você conseguirá ver as alterações no navegador (as vezes será necessário dar um reload na página).


## Build

Se quiser rodar o site em modo de produção. Basta rodar estes comandos:

```shell
$ npm run build
$ npm run start
```

O site traduzido estará montado e rodando em http://localhost:3000 no mode de produção.


## Como posso contribuir na tradução

> Toda ajuda é sempre bem-vinda. Para isso, você deverá clonar este repositório na sua máquina e fazer as alterações em uma `branch` localmente. Quando estiver satisfeito com as traduções feitas, você irá solicitar um [`pull request`](https://github.com/svelte-brasil/br.svelte.dev/pulls) para que o seu texto entre na fila de revisão e, quando aprovado, será integrado no `MASTER`.

* [Acompanhe o andamento](https://github.com/svelte-brasil/br.svelte.dev/projects/1) das traduções feitas até agora.
* [Melhore uma tradução](https://github.com/svelte-brasil/br.svelte.dev/projects/1#column-10572747) já realizada.

## Dúvidas?

Caso tenha alguma dúvida, pode nos procurar em qualquer um dos nossos canais:

* [Telegram](https://t.me/sveltebrasil)
* [Facebook](https://www.facebook.com/groups/sveltebrasil/)
* [Twitter](https://twitter.com/sveltebrasil)
* [Github](https://github.com/svelte-brasil)
* [Youtube](https://www.youtube.com/channel/UCp8jamqJRGg86eMnewxjWng)