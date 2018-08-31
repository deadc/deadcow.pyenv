Pyenv
=========

[![Travis-CI](https://travis-ci.org/deadc/deadcow.pyenv.svg?branch=master)](https://travis-ci.org/deadc/deadcow.pyenv)

O pyenv permite alternar facilmente entre várias versões do Python. É simples, discreto e segue a tradição UNIX de ferramentas de propósito único que fazem uma coisa bem.

Requirementos
------------

Nenhum

Variaveis
--------------

Abaixo as variaveis da role e seus respectivos valores padrão.

    pyenv_python_version: 2.7.9

Define a versão do python desejada, lembrando que apenas a partir da versão 2.7.9 o binário pip vem por padrao com o pacote python.

    pyenv_repository: https://github.com/pyenv/pyenv.git

Endereço do repositorio que o pyenv utiliza, este endereço deverá ser git://

    pyenv_path: /data/shared

Caminho onde o pyenv será instalado, neste caminho também estará o arquivo de de variaveis de ambiente `pyver` a ser carregado na sessão onde o python será chamado.


Dependencias
------------

Nenhum

Playbook Exemplo
----------------

    - hosts: all
      vars:
        pyenv_python_version: 3.6.4

      roles:
         - pyenv

License
-------

BSD

Informaçoes sobre o autor
------------------

Esta role foi desenvolvida por Thiago Freitas (deadcow@archlinux.com.br) em 03/2018.
