A fim de que cada container seja isolado dos demais apesar de funcionar na mesma máquina surgem os _namespaces_. São eles:
- PID: Responsável por prover o isolamento entre os processos que estão rodando dentro do container;
- NET: Encarregado do isolamento entre as interfaces de rede;
- IPC: Incumbido do isolamento da comunicação entre processos e a memória compartilhada;
- MNT: Provê o isolamento do sistema de arquivos, ponstos de montagem.
- UTS: Provê o isolamento do kernel. Age como se o container fosse outro host.