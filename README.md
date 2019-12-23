# Estudo sobe a ferramenta TMUX - Terminal Multiplex.

## Tmux 
[github](https://github.com/tmux)

---

> Acesso a documentação

```bash
$ man tmux
```

O termux usa um prefixo para eviar o choque de teclas e atalhos com outras ferramentas do gênero. 
O prefixo padrão ou default do tmux é o <C-b> 'ctrl + b'.

### Modificando o prefixo padrão. 

```
$ <C-b> : 'novo comando'
```

### Lista de comandos do tmux:
 
```
$ <C-b> !
```

### Commandos Sessões

> Criar um sessão:

```bash
$ tmux
```

> Criar uma sessão com nomeada: 

```bash
$ tmux new-session -s 'nome-da-sessão'
```

Comando mais curto um short hand.

```bash
$ tmux new -s 'nome-da-sessão'
```

> Fechar a janela da sessão

```tmux
: <C-b>+x
```

```tmux
: exit
```

> Fechar a sessão

```bash
$ tmux kill-session -t basic
```

Ou se houver mais de uma sessão.

```bash
$ tmux kill-session -t second_session
```

> Desconectar um sessão

```tmux
: <C-b>+d
```

> Listar a sessões ativas

```bash
$ tmux list-sessions
```
 
Comando mais curto um short hand

```bash
$ tmux ls
```

> Anexar uma sessões

Se tiver apenas uma sessão aberta 
```bash
$ tmux attach
```

Se houver mais de uma sessão aberta
```bash
$ tmux attach -t "nome-da-sessão"
```

> Navegando entre as sessões

```tmux
: <C-b>+(
```

ou

```tmux
: <C-b>+)
```

### Comandos de Tela ou Window

> Criando um sessão nomeada:

```tmux
$ Tmux new -s 'sessão' -n 'nome_da_janela'
```

> Dividir a tela na vertical:

```tmux
: <C-b>+shift+% 
```

> Dividir a tela na horizontal

```tmux
: <C-b>+"
```

> Navegação entre telas || windows || janelas.

```tmux
: <C-b>+'seta_a_esquerda'
: <C-b>+'seta_a_direita'
: <C-b>+'seta_cima'
: <C-b>+'seta_baixo'
```

> Rotacionar as telas

```tmux
: <C-b><C-o>
```


> Listar as janelas abertas

```tmux
: <C-b>+s
```

> Navegando entre as janelas

```tmux
: <C-b>+(
```

ou

```tmux
: <C-b>+)
```

> Maximizando um janela

```tmux
: <C-b>+z
```
> Adicionar um nova janela

```tmux
: <C-b>+c
```

> Navegar entre as janelas

```tmux
: <C-b> <numero_da_janela>
```

