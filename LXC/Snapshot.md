## Estrutura do LXC
O LXC é composto por um conjunto de ferramentas e bibliotecas que facilitam a criação e a gestão de contêineres no Linux. Ele utiliza recursos do kernel do Linux, como CGroups e Namespaces, para isolar processos e sistemas de arquivos entre diferentes contêineres.[¹]

### Namespaces e CGroups
O uso de namespaces no kernel do Linux permite a criação de ambientes isolados, como namespaces de PID, rede, usuário, entre outros. Os CGroups (Control Groups) são usados para controlar e limitar os recursos, como CPU, memória e rede.[²]

## Ferramentas de Snapshots no LXC

1. **lxc-snapshot**
   - O `lxc-snapshot` é uma ferramenta integrada ao LXC que permite criar e gerenciar snapshots de contêineres. Ela captura o estado atual do sistema de arquivos e dos processos do contêiner.[³]

3. **Criação de Snapshots**
   - Para criar um snapshot com o `lxc-snapshot`, você pode usar o comando `lxc-snapshot -n nome-do-container nome-do-snapshot`. Isso captura o estado atual do contêiner para um snapshot específico.

4. **Restauração de Snapshots:**
   - Para restaurar um contêiner para um snapshot anterior, você pode usar o comando `lxc-snapshot -n nome-do-container restore nome-do-snapshot`.

5. **Listagem de Snapshots:**
   - O comando `lxc-snapshot -n nome-do-container list` permite listar todos os snapshots disponíveis para um contêiner.
---
# Links Úteis
- https://discuss.linuxcontainers.org/t/managing-lxd-container-snapshots/1951/3
- https://www.cyberciti.biz/faq/create-snapshots-with-lxc-command-lxd/

[¹]: https://linuxcontainers.org/lxc/introduction/
[²]: https://lwn.net/Articles/531114/
[³]: https://linuxcontainers.org/lxc/manpages/man1/lxc-snapshot.1.html