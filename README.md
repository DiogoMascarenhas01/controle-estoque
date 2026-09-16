# Controle de Estoque

Aplicação desktop em Python/Tkinter para controle de produtos, movimentações, usuários, inventários e relatórios.

## Requisitos

- Windows 10 ou 11
- Python 3.14
- MongoDB local disponível em `mongodb://localhost:27017/`

## Instalação

```bash
py -3.14 -m pip install -r requirements.txt
```

Inicie o serviço do MongoDB e execute:

```bash
py -3.14 gerenciamento_estoque.py
```

O banco utilizado pela aplicação é `ControleDeEstoque`.

## Recursos visuais

Mantenha estes arquivos junto ao código principal:

- `background.png`
- `logo.png`
- `icon.png`

## Segurança

Esta versão foi desenvolvida para uso local. Antes de disponibilizá-la em rede ou para vários usuários, revise o gerenciamento de contas: o código atual mantém um campo de senha em texto simples no MongoDB para exibição administrativa, além do hash usado na autenticação. Não use credenciais reais ou reutilizadas enquanto esse comportamento não for removido.

## Arquivos não versionados

Artefatos do PyInstaller, executáveis, relatórios, inventários, caches, ambientes virtuais e dados locais são excluídos pelo `.gitignore`.
