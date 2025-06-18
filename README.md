# Passo a passo para construir sua-page.github.io

Primeiro você deve criar um repositório para seu nome de usuário no github.

Exemplo:

Meu nome de usuário no github é andersonbraz.

então criei um repositório com o nome:

andersonbraz.github.io

que virou posteriormente a página:

https://andersonbraz.github.io

## Clonar o repositório para seu computador

```shell
git clone https://nomeusuario.github.io
```

## Acessar o diretório do seu repositório

```shell
cd nomeusuario.github.io
```

## Criar o ambiente de Python do seu projeto

```shell
python -m venv .venv
```

## Ativar o ambiente de Python do seu projeto

```shell
. .venv/bin/activate
```

## Atualizar o ambinete de Python do seu projeto

```shell
python -m pip install --upgrade pip
```

## Instalar a biblioteca mkdocs-material no seu projeto

```shell
pip install mkdocs-material
```

## iniciar um novo projeto mkdocs no seu repositório

```shell
mkdocs new .
```

## Ativar um servidor http para visualizar o seu projeto 

```shell
mkdocs serve
```

## IMPORTANTE: Configurar url do seu site para deploy

```shell
site_name: Nome do seu site
site_url: https://nomeusuario.github.io.com
```

## Submeter branch principal para o github

```shell
git checkout -b main
git add .
git commit -m "Up File(s) project."
git push
```

## Realizar deploy para o github

```shell
mkdocs gh-deploy --force
```