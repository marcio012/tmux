# Estudo sobe a ferramenta TMUX - Interação com as Sessões.

*Criar um sessão:*

```bash
$ tmux
```

*Criar uma sessão com nomeada:* 

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
