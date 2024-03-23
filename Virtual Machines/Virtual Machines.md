Uma máquina virtual é uma representação virtual ou emulação de um computador físico. Eles são frequentemente referidos como convidados, enquanto a máquina física em que eles rodam é chamada de host.[¹]

A virtualização torna possível criar várias máquinas virtuais, cada uma com seu próprio sistema operacional (SO) e aplicativos, em uma única máquina física. Uma VM não pode interagir diretamente com um computador físico. Em vez disso, ele precisa de uma camada leve de software chamada hipervisor para coordenar entre ele e o hardware físico subjacente. O hipervisor aloca recursos de computação física - como processadores, memória e armazenamento - para cada VM. Ele mantém cada VM separado dos outros para que eles não interfiram um no outro.[¹]

## Como a virtualização funciona
Quando um hipervisor é usado em um computador ou servidor físico - também conhecido como bare metal server -, ele permite que o computador físico separe seu sistema operacional e aplicativos de seu hardware. Então, ele pode se dividir em várias “máquinas virtuais independentes." [¹]
  
Cada uma dessas novas máquinas virtuais pode executar seus próprios sistemas operacionais e aplicativos de forma independente, enquanto ainda compartilha os recursos originais do servidor, gerenciado pelo hipervisor. Esses recursos incluem memória, RAM, armazenamento, etc.

## Tipos de Hipervisores
1. **Hipervisores do tipo 1:** são executados diretamente no hardware físico (geralmente um servidor), substituindo o sistema operacional. Normalmente, você usa um produto de software separado para criar e manipular VMs no hipervisor.
	Você pode usar uma VM como modelo para outras pessoas, duplicando-a para criar novas. Dependendo das suas necessidades, você pode criar vários modelos de VM para diferentes propósitos, como testes de software, bancos de dados de produção e ambientes de desenvolvimento.[¹]
2. **Hipervisores do tipo 2:** são executados como um aplicativo em um sistema operacional host e geralmente têm como alvo plataformas de desktop ou notebook de usuário único. Com um hipervisor Tipo 2, você cria manualmente uma VM e instala um SO convidado. Você pode usar o hipervisor para alocar recursos físicos à sua VM, definindo manualmente a quantidade de núcleos do processador e a memória que ele pode usar.[¹]
### Vantagens
- Flexibilidade;
- Portabilidade;
- Segurança;
#### Segurança
As VMs melhoram a segurança de várias maneiras quando comparadas aos sistemas operacionais executados diretamente no hardware. Uma VM é um arquivo que pode ser verificado quanto a software malicioso por um programa externo. Você pode criar um instantâneo inteiro da VM a qualquer momento e restaurá-lo para esse estado se estiver infectado por malware, efetivamente levando a VM de volta no tempo. A criação rápida e fácil de VMs também permite excluir completamente uma VM comprometida e recriá-la rapidamente, acelerando a recuperação de infecções por malware.

## Escolhendo um provedor de máquina virtual

Selecionar uma máquina virtual não precisa ser desafiador, desde que você saiba o que procurar. A máquina virtual precisa atender às suas necessidades de carga de trabalho e orçamento de negócios, é claro, mas outros fatores desempenham papéis importantes entre você e seu ambiente de virtualização. Abaixo estão dez coisas a considerar ao selecionar um provedor de serviços de máquina virtual.[¹]

- **Opções gerenciadas.** O provedor de nuvem oferece soluções não gerenciadas e gerenciadas? Se você não conhece a tecnologia de virtualização por dentro e por fora, considere um provedor responsável pela configuração, manutenção e monitoramento contínuo do desempenho.[¹]
- **Integração de Software.** O ambiente da sua máquina virtual funcionará bem com os outros? Sistemas operacionais, software de terceiros, tecnologia de código aberto e aplicativos ajudam a fornecer mais soluções em todos os seus negócios. Você desejará um fornecedor de máquinas virtuais com suporte e fortes parcerias com os fornecedores de software mais usados do setor.

## Segurança

A virtualização oferece alguns benefícios de segurança. Por exemplo, VMs infectadas com malware podem ser revertidas para um momento no tempo (chamado de instantâneo) quando a VM não foi infectada e estável; eles também podem ser excluídos e recriados com mais facilidade. Você nem sempre pode desinfetar um sistema operacional não virtualizado, porque o malware geralmente é profundamente integrado aos componentes principais do sistema operacional, persistindo além das reversões do sistema.[²]

%%
Cada VM inclui um arquivo de configuração que armazena as configurações da VM, um arquivo de disco virtual que é uma versão de software de um disco rígido, e um arquivo de log que acompanha as atividades da VM, incluindo falhas no sistema, alterações de hardware, migrações de máquinas virtuais de um host para outro, e o status da VM. 
%%

---
[¹]: https://www.ibm.com/topics/virtual-machines
[²]: https://www.ibm.com/topics/virtualization