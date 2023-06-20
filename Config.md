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
pyenv install 3.10.7
```

```console
pyenv global 3.10.7
```

Fedora

```
sudo dnf groupinstall "Development Tools" -y
sudo dnf install zlib-devel bzip2 bzip2-devel readline-devel sqlite sqlite-devel openssl-devel xz xz-devel libffi-devel findutils tk-devel -y
```

## 3) zsh

```console
sudo dnf install zsh
```

```console
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

starship

```console
curl -sS https://starship.rs/install.sh | sh
```

configs

```console
plugins=(
 zsh-autosuggestions
 zsh-syntax-highlighting
)

eval "$(starship init zsh)"
```

```console
chsh -s $(which zsh)
```

## 3) poetry

```console
curl -sSL https://install.python-poetry.org | python3 -
```

```console
export PATH=$PATH:$HOME/.local/bin
```

## 4) pipenv

## 5) alias

## 6 Git

```console
git config --global core.excludesfile ~/.gitignore
git config --global core.pager "cat"
git config --global init.defaultBranch main
```
