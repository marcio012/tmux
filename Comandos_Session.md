# Estudo sobe a ferramenta TMUX - Interação com as Sessões.

No Tmux o conceito de sessão e muito parecido com o de uma workspace. A árvore hierarquica seria:

**Criar um sessão:**

```bash
$ tmux
```

**Criar uma sessão nomeada:**

```bash
$ tmux new-session -s 'nome-da-sessão'
```

Comando mais curto um short hand.

```bash
$ tmux new -s 'nome-da-sessão'
```

Criar um sessão e em background

```bash
$ tmux new -s "nome-da-sessão" -d
```

A flag *"-d"* passa para o tmux para criar a sessão desatachada do terminal, no caso em background.

**Fechar a sessão**

```bash
$ tmux kill-session -t basic
```

Ou se houver mais de uma sessão. Tem que ser removida digitando o nome da sessão.

```bash
$ tmux kill-session -t "nome_da_sessão"
```

**Listar a sessões ativas**

```bash
$ tmux list-sessions
```
 
**Comando mais curto um short hand**

```bash
$ tmux ls
```

**Anexar uma sessões**

Se tiver apenas uma sessão aberta 
```bash
$ tmux attach
```

Se houver mais de uma sessão aberta
```bash
$ tmux attach -t "nome-da-sessão"
```

**Desconectar um sessão**

```tmux
: <C-b>+d
```

**Navegando entre as sessões**

```tmux
: <C-b>+(
```

ou

```tmux
: <C-b>+)
```

**Fechar a janela da sessão**

```tmux
: <C-b>+x
```

```tmux
: exit
```

