# Estudo sobe a ferramenta TMUX - Interação com as Janelas.

As Sessões são compostas por n Janelas, sendo o segundo nível. 

### Comandos de Tela ou Window

**Criando um sessão nomeada:**

```tmux
$ Tmux new -s 'sessão' -n 'nome_da_janela'
```

Passando a flag **"-n"** no comando identifica que está nomeando a sessão.
Dentro do tmux você pode definir um nome passando o comando.

```tmux
: <C-b>,
```

**Movendo entre as janelas:**

Para próxima janela: 
```tmux
: <C-b>n
```

Para janela anterior: 
```tmux
: <C-b>p
```
Por padrão cada janela tem um index gerado pelo tmux, isso permite navegar por esse index.
```tmux
: <C-b>0
```
Se houver mais de nove janealas pode se fazer uso do ```<C-b>w```.

Para buscar um janela pode se fazer uso do ```<C-b>f```, ele aceita uma string como parametro. 

Para fechar uma janela pode usar o comando.

```tmux
: <C-b>&
```
Esse comando exibirar uma mensagem que espera uma confirmação para fechar a tela. 

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

