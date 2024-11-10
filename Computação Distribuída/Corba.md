# Definição
CORBA (common object request broker architecture) é especificação padronizada de um OMA (object management architecture) com o objetivo de interoperabilidade entre diferentes sistemas computacionais e linguagens de programação através de um ORB definido, que são estruturas que permitem que os programadores façam chamadas de um computador a outro através de uma rede. Tal padrão é definido pela OMG. [¹]  [²]

A versão 1.1 do CORBA foi introduzida em 1991 pelo OMG e definia a Linguagem de Definição de Interface (_Interface Definition Language_ - IDL) e a Interface de Programação de Aplicação (_Application Program Interface_ - API) que permitiam a interação de objetos cliente/servidor com uma implementação específica de um Barramento para Pedidos de Objetos (_Object Request Broker_ - ORB). O CORBA 2.0, adotado em Dezembro de 1994, definia a verdadeira interoperabilidade especificando como ORBs de fabricantes diferentes podem interoperar.[³]
# Criadores
OMG significa Object Management Group, que é um consórcio com a intenção de definir padrões para sistemas distribuídos orientados a objetos. Participam as grandes: 
• Adobe Systems Inc. 
• AT&T 
• Boeing 
• Borland Software Corporation 
• Department of National Defence 
• Ericsson 
• Fujitsu 
• GNOME Foundation 
• Hewlett-Packard 
• Hitachi 
• Massachusetts Institute of Technology (MIT) 
• Motorola 
• NASA 
• Nokia 
• Oracle 
• Sun Microsystems 
• Alcatel-Lucent 
• Telefonica I+D 
• Toshiba 
• W3 Consortium 
• Walt Disney World Co. 
• Entre outros. [²]
# Funcionamento
O componente fundamental para o CORBA é o [ORB](#ORB) que tem a tarefa de facilitar a comunicação dos objetos. Provendo o [IOR](#OIR) (Interoperable Object Reference), o ORB consegue localizar os objetos destinos e transmitir informação para ou das invocações de métodos remotos. A interface para objetos CORBA é especificado pela CORBA Interface Definition Language ([IDL](#IDL)). Um compilador traduz a definição IDL em uma linguagem de programação (C++,Java) gerando IDL Stubs e skeletons que provêm respectivamente um framework para o lado cliente e um proxy para o lado servidor.

Requisições e respostas entre objetos são entregues através de um formato padrão definido pelo [IIOP](#IIOP)(Internet Inter-ORB Protocol). O Dynamic Invocation Interface ([DII](#DII)) e o Dynamic Skeleton Interface ([DSI](#DSI)) permitem que os objetos sejam criados sem um conhecimento prévio da interface IDL.

Requisições são empacotadas em um formato de plataforma independente, através do cliente stub(ou no DII) e desempacotadas no lado servidor em um formato especifico definido pelo IDL skeleton (ou no DSI) e pelo objeto adaptador, que serve como um mediador entre a implementação do objeto , o servidor, e o seu ORB, através disso desacoplando o código usuário do processo ORB.

O Portable Object Adapter ([POA](#POA)) prove objetos CORBA com um conjunto de métodos comuns para acessar funções [ORB](#ORB), abrangendo autenticação de usuário para ativação de objetos e persistência de objetos. Seu tarefa básica, entretanto, é criar referencia de objetos e despachar requisições ORB apontados para objetos destinos em seus respectivos servidores. Um servidor pode prover um numero qualquer de POAs, cada com seu próprio conjunto de seguranças. POA também prove um mecanismo para salvar e restaurar estados de objetos. Isto, junto com o uso do Implementation Repository (IMR), que cuida do start e o restart automático dos servidores, realizam a persistência dos objetos.
## OMA
OMA (object management architecture) é a estrutura que define a arquitetura sob a qual os objetos locais e remotos irão comunicar-se. [¹] A OMA define os serviços e as interfaces necessárias para gerenciar objetos distribuídos em um ambiente CORBA. Ela estabelece padrões para aspectos como segurança, transações, persistência e gerenciamento de eventos em sistemas distribuídos baseados em CORBA. De forma mais visual, a estrutura básica de um OMA é similar à seguinte figura:
![[Pasted image 20231119123010.png |500]]
## ORB
Em computação distribuída, um ORB (object request broker) é uma peça de [middleware]([[Middleware]]) que permite que os programadores façam chamadas de um computador a outro via uma rede. ORB é o componente-chave da OMA (object management architecture), sendo muitas vezes chamado de barramento de objetos pela sua funcionalidade de trafegar os dados dos objetos do ambiente local para o remoto e vice versa. A principal função de um ORB é a transformação das estruturas de dados envolvidas nas chamadas aos objetos remotos no stream de bytes que será trafegado pela rede, utilizando o protocolo GIOP.[¹]
## GIOP
GIOP (general interORB protocol) é um protocolo abstrato de comunicação utilizado entre os ORB’s. Os padrões associados a este protocolo são mantidos pela OMG. O GIOP disponibiliza alguns protocolos concretos: 
• IIOP (Internet interORB protocol): é o protocolo de comunicação entre ORB’s CORBA publicado pela OMG, sendo uma implementação do GIOP para ser utilizado na Internet (sobre TCP/IP). 
• SSLIOP (SSL interORB protocol): é uma implementação do IIOP sobre SSL, permitindo criptografia dos dados e autenticação. 
• HTIOP (HyperText interORB protocol): é uma implementação do IIOP sobre HTTP, permitindo transparência sob o ponto de vista de firewalls. [¹]
## IDL
## DII
## DSI


[¹]: https://www.inf.ufrgs.br/~johann/sisop2/gvgoCORBA20062.pdf
[²]: https://www.inf.ufrgs.br/~johann/sisop2/GVGOgrupo2.htm
[³]: https://www.gta.ufrj.br/~renata/corba/corba.htm
[⁴]: https://www.omg.org/spec/CORBA/2.0/PDF
[⁵]: https://www.omg.org/spec/CORBA/3.4/Interoperability/PDF


