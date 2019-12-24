# Estudo sobe a ferramenta TMUX - Interação com os panels

As Sessões são compostas por *"n"* Janelas, e as janelas são compostas e *"n"* paineis, sendo o terceiro nível. 

### Comandos de Tela ou Window
**Dividir a tela na vertical:**

```tmux
: <Prefix>+shift+% 
```

**Dividir a tela na horizontal**

```tmux
: <Prefix>+"
```

**Navegação entre telas || windows || janelas.**

```tmux
: <Prefix>+'seta_a_esquerda'
: <Prefix>+'seta_a_direita'
: <Prefix>+'seta_cima'
: <Prefix>+'seta_baixo'
```

**Rotacionar as telas**

```tmux
: <Prefix>+<C-o>
```

**Maximizando um painel, transformando de visão multipla para visão única.**

```tmux
: <Prefix>+z
```

**Layouts dos Paineis**
 
Pode se configurar os paineis para quando o tmux iniciar, ele carregar um configuração padrão personalizada do gosto do usuário. 

* *even-horizontal*, empilha todos os paineis horizontalmente, da esquerda para a direita. 
* *even-vertial*, empilha todos os paineis verticalmente, de cima para baixo.
* *main-horizontal*, cria um painel superior maior, e dois paineis inferiores menores.
* *main-vertical*, cria um painel grande do lado esquerdo da tela e emplilha os restantes dos paineis verticalmente a direita.

Pode percorre esse paineis usando o comando ```<Prefix>+barra-de-espaço```

Pode se encerra todo processo no painel como também no tmux digitando ```<Prefix>+x```

**Dimencionando o tamanhos das janelas**

Ao *precionar* o comando ```<Prefix>+shift+:``` com esse combo, inicia o prompt do tmux no canto inferior da janela, ele aceita comandos que interagiram com a ferramenta. 

**Comandos de redirecionamento das telas**

```tmux:
:resize-pane -D (Dimenciona o painel atual para baixo)
:resize-pane -U (Dimenciona o painel atual para cima)
:resize-pane -L (Dimenciona o painel atual para esquerda)
:resize-pane -R (Dimenciona o painel atual para direita)
:resize-pane -D 10 (Dimenciona o painel atual para baixo em 10 celulas)
:resize-pane -U 10 (Dimenciona o painel atual para cima em 10 celulas)
:resize-pane -L 10 (Dimenciona o painel atual para esquerda em 10 celulas)
:resize-pane -R 10 (Dimenciona o painel atual para direita em 10 celulas)

```
Podendo redimencionar ao toke do usuário.

