# Estudo sobe a ferramenta TMUX - Interação com os panels

As Sessões são compostas por *"n"* Janelas, e as janelas são compostas e *"n"* paineis, sendo o terceiro nível. 

### Comandos de Tela ou Window
**Dividir a tela na vertical:**

```tmux
: <C-b>shift% 
```

> Dividir a tela na horizontal

```tmux
: <C-b>"
```

> Navegação entre telas || windows || janelas.

```tmux
: <C-b>'seta_a_esquerda'
: <C-b>'seta_a_direita'
: <C-b>'seta_cima'
: <C-b>'seta_baixo'
```

> Rotacionar as telas

```tmux
: <C-b><C-o>
```


> Listar as janelas de uma sessão

```tmux
: <C-b>s
```

> Navegando entre as janelas de uma sessão


```tmux
: <C-b>( 

```

ou

```tmux

```

> Maximizando um janela, dando um zoom na tela, transformando de visão multipla para visão única.

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

