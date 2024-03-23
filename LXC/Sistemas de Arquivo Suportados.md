O lxc suporta vários sistemas de arquivos Linux, os comandos para a seleção de cada um deles são:
- dir;
- lvm;
- loop;
- btrfs;
- zfs;
- rbd;
- best;
Segue as especificações de cada comando.

## Dir

O padrão é 'dir', o que significa que o sistema de arquivos raiz do contêiner será um diretório em /var/lib/lxc/container/rootfs.[¹]

# LVM

## BTRFS

Se 'btrfs' for especificado, o sistema de arquivos de destino deverá ser btrfs e os rootfs do contêiner serão criados como um novo subvolume. Isso permite a criação de clones instantâneos, mas também faz com que o rsync --one-filesystem o trate como um sistema de arquivos separado.[¹]

### Definição
Btrfs, ou B-tree file system, é um sistema de arquivos desenvolvido para Linux. Ele foi criado por Chris Mason para servidores e dispositivos de armazenamento em rede. 

O Btrfs é baseado no princípio copy-on-write (COW).  Por padrão, o Btrfs usa COW para todos os arquivos. As gravações não substituem os dados no local, mas sim gravam uma cópia modificada do bloco em um novo local. Os metadados são atualizados para apontar para o novo local. 

O Btrfs permite o agrupamento de discos ou volumes e oferece maior escalabilidade em relação aos sistemas de arquivos tradicionais como o ext4. 

O desenvolvimento do Btrfs começou em 2007 e, desde agosto de 2014, o formato em disco do sistema de arquivos foi marcado como estável.



[¹]: https://linuxcontainers.org/lxc/manpages//man1/lxc-create.1.html