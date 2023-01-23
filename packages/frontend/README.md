# eslint-config-trybe-frontend

Configurações utilizadas pela Trybe em projetos Front-End!

## Instalação

basta instalar através do npm (ou gerenciador favorito):

```shell
npm i eslint-config-trybe-frontend
```

## Uso

Basta adicionar no seu `.eslintrc.json`:

```javascript
{
  // ...
  "extends": "trybe-frontend"
  // ...
}
```

## Possíveis problemas

Eventualmente pode ser necessário que você instale manualmente as `peerDependencies`.
Se esse for o caso, basta rodar o comando:

```shell
npx install-peerdeps --dev eslint-config-trybe-frontend
```

Isso deverá resolver o problema. Qualquer coisa, abra uma issue que ficaremos felizes em resolver :)
