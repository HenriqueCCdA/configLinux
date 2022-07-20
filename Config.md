# Config Linux

Setup incial da maquina linux que eu uso para desenvolvimento

## 1) nvm

O nvm server para gerenciar a versão do **node** instalada.

[nvm - projeto do github](https://github.com/nvm-sh/nvm)

Exemplo de Instalação

```console
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

### Instalando o node 16:

```console
nvm install 16
```

### Para usar o node 16

```console
node use 16
```

## 2) pyenv

Clonando o Repositorio

```
git clone https://github.com/pyenv/pyenv.git ~/.pyenv
```

Configura da bash

```console
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bashrc
echo 'command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(pyenv init -)"' >> ~/.bashrc
```

Lista os interpretadores disponiveis

```console
pyenv install --list
```

```console
pyenv install 3.10.5
```

```console
pyenv global 3.10.5
```

## 3) zsh

## 3) peotry

## 4) pipenv

## 5) alias
