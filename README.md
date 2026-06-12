# Bolsao da Fluencia - Copa da Contabilidade

Landing page publicada em:

- `https://bolsao.fluenciacontabil.com.br/`
- `https://bolsao.fluenciacontabil.com.br/obrigado.html`

O dominio e definido pelo arquivo `CNAME`:

```txt
bolsao.fluenciacontabil.com.br
```

## Publicacao

Este diretorio e um repositorio Git separado:

- Repositorio remoto: `https://github.com/gruponbeducacao/bolsao-lp.git`
- Branch publicada: `main`
- Publicacao: GitHub Pages via `CNAME`

Para publicar alteracoes:

```powershell
git status --short --branch
git add index.html obrigado.html
git commit -m "Descricao objetiva da alteracao"
git push origin main
```

## Google Tag Manager

O GTM instalado nesta LP e:

```txt
GTM-WF6P82HX
```

Arquivos com o GTM instalado:

- `index.html`
- `obrigado.html`

Em ambos os arquivos:

- O bloco `<script>` do Google Tag Manager fica no topo do `<head>`.
- O bloco `<noscript>` fica imediatamente apos a abertura do `<body>`.

O arquivo local `tag manager lp bolsao.txt` contem o snippet original fornecido pelo Google Tag Manager. Ele foi usado como fonte do codigo instalado e nao precisa ser publicado junto com a landing.

## Historico

Em 2026-06-12, o GTM `GTM-WF6P82HX` foi instalado e publicado no commit:

```txt
fbcbe63 Instala GTM na LP do bolsao
```

Apos o push, as duas URLs publicadas foram verificadas e retornaram o container `GTM-WF6P82HX` no bloco do `<head>` e no `noscript` do `<body>`.

## Validacao rapida

Para confirmar o GTM publicado:

```powershell
curl.exe -L https://bolsao.fluenciacontabil.com.br/ | Select-String "GTM-WF6P82HX"
curl.exe -L https://bolsao.fluenciacontabil.com.br/obrigado.html | Select-String "GTM-WF6P82HX"
```

Cada pagina deve retornar duas ocorrencias do container: uma no script principal e outra no `noscript`.
