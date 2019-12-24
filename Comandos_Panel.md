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

