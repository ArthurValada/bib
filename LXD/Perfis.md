Os perfis armazenam um conjunto de opções de configuração. Podem conter opções de instância, dispositivos e opções de dispositivos. Uma ou mais conjuntos de configurações, perfis, podem ser aplicadas a uma mesma instância, entretanto, a última tem prioridade e, acima desta, está as configurações individuais da instância, que está acima de todos os perfis aplicados a uma instância.

> Perfis podem conter dados, opções, que dizem respeito a um container, uma máquina virtual ou ambos.

### Aplicando perfis inválidos a uma instância

Ao aplicar-se perfis inválidos a uma dada instância essa configuração é ignorada e não resulta em um erro.

## Perfil padrão

Ao criar-se uma instância sem perfil especificado, o perfil default é utilizado, este não pode ser renomeado ou excluído. Tal perfil define um disco raíz e uma interface de rede.

## Operações com perfis
### Listagem

Para listar o conjunto de perfis armazenados no seu LXC, use o seguinte comando:

```bash
lxc profile list
```

### Exibição

Para exibir o conteúdo de um dado perfil, use o seguinte comando:

```bash
lxc profile show <profile_name>
```

Onde `<profile_name>` é o nome do perfil listado usando o comando de listagem, contido em [Listagem](#Listagem).

### Criando um perfil vazio

Use o seguinte comando para criar um perfil vazio:

```bash
lxc profile create <profile_name>
```

Onde `<profile_name>` é o nome do perfil a ser criado.

