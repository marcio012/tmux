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
: <Prefix>+,
```

**Movendo entre as janelas:**

Para próxima janela: 
```tmux
: <Prefix>+n
```

Para janela anterior: 
```tmux
: <Prefix>+p
```
Por padrão cada janela tem um index gerado pelo tmux, isso permite navegar por esse index.
```tmux
: <Prefix>+0
```
Se houver mais de nove janelas pode se fazer uso do ```<Prefix>+w```.

Para buscar um janela pode se fazer uso do ```<Prefix>+f```, ele aceita uma string como parametro. 

Para fechar uma janela pode usar o comando.

```tmux
: <Prefix>+&
```
Esse comando exibirar uma mensagem que espera uma confirmação para fechar a tela. 

> Maximizando um janela, dando um zoom na tela, transformando de visão multipla para visão única.

```tmux
: <Prefix>+z
```

> Adicionar um nova janela

```tmux
: <Prefix>+c
```

> Navegar entre as janelas

```tmux
: <Prefix>+<numero_da_janela>
```

