Em redes de computadores, um "proxy" refere-se a um servidor intermediário que atua como um intermediário entre os usuários e os servidores de destino. Ele recebe solicitações dos clientes e as encaminha para os servidores, mascarando assim a identidade real do cliente. Os proxies podem ser usados para controle de acesso, cache, filtragem de conteúdo, entre outras finalidades.

Proxy como servidores intermediários desempenham um papel crucial na comunicação de rede, atuando como intermediários entre clientes e servidores. Esses servidores intermediários têm várias finalidades, incluindo controle de acesso, aumento de desempenho, cache de conteúdo, filtragem de conteúdo e anonimização.

## Detalhamento

1. **Controle de Acesso:**
   - Proxies são frequentemente utilizados para implementar políticas de controle de acesso. Eles atuam como gatekeepers, permitindo ou negando o acesso a recursos da internet com base em políticas predefinidas. Isso pode incluir bloqueio de sites específicos, filtragem de conteúdo ou restrições de acesso baseadas em endereço IP.

2. **Cache de Conteúdo:**
   - Proxies podem armazenar em cache recursos frequentemente acessados, como páginas da web, imagens e arquivos, localmente. Quando um cliente solicita um recurso já presente no cache, o proxy pode fornecê-lo diretamente, reduzindo a carga nos servidores de origem e melhorando a velocidade de resposta.

3. **Aumento de Desempenho:**
   - Ao armazenar em cache recursos e otimizar a entrega de conteúdo, os proxies contribuem para o aumento geral do desempenho da rede. Eles podem reduzir a latência e o tempo de carregamento de páginas, especialmente para recursos estáticos, ao fornecer cópias locais dos dados.

4. **Filtragem de Conteúdo:**
   - Proxies são utilizados para aplicar políticas de filtragem de conteúdo, bloqueando ou permitindo o acesso a determinados tipos de dados. Isso pode ser útil em ambientes corporativos para garantir conformidade com políticas internas ou em instituições educacionais para filtrar conteúdo inadequado.

5. **Anonimização e Privacidade:**
   - Alguns proxies oferecem serviços de anonimização, ocultando o endereço IP do cliente dos servidores de destino. Isso pode ser usado para proteger a privacidade dos usuários, impedindo que os servidores de destino rastreiem diretamente a origem das solicitações.

6. **Segurança:**
   - Proxies podem ser usados como uma camada adicional de segurança, fornecendo um ponto de controle para monitorar e filtrar tráfego malicioso. Eles podem bloquear conteúdo suspeito, proteger contra ameaças conhecidas e fornecer uma barreira adicional contra ataques.

7. **Gateway para Redes Internas:**
   - Em ambientes corporativos, proxies muitas vezes atuam como gateways entre redes internas e a internet. Isso permite implementar políticas de segurança, controle de acesso e monitoramento do tráfego entre as redes.

8. **Proxy Reverso:**
   - Um proxy reverso é colocado entre os clientes externos e os servidores internos para gerenciar solicitações de clientes. Ele ajuda a melhorar o desempenho, escalabilidade e segurança dos servidores internos, atuando como um ponto de entrada controlado.

9. **Balanceamento de Carga:**
   - Em conjunto com funções de proxy reverso, os proxies também podem realizar balanceamento de carga, distribuindo solicitações entre vários servidores para otimizar a utilização dos recursos e melhorar a capacidade de resposta do sistema.

Os proxies como servidores intermediários são versáteis e podem ser configurados para atender a uma variedade de necessidades, dependendo dos requisitos específicos do ambiente de rede.
## Tipos de proxy
- **Proxy transparente:** com ele, o site que estiver acessando ainda vai saber quem é você. Ou seja, ele passa seu endereço IP para o servidor web, além de mostrar que está usando um proxy. Ele normalmente é usado por escolas e bibliotecas para filtragem de conteúdo;[¹]

- **Proxy anônimo:** nesse caso, ele se identifica como um proxy, mas fornece um IP falso para o site. Assim, você pode parecer estar em um local diferente do que está e conseguir acessar conteúdos que na sua região está bloqueado, por exemplo. Assim como no transparente, ele também mostra que o usuário está usando um proxy;[¹]

- **Proxy de alto anonimato:** esses proxies disfarçam seu uso, ou seja, não permitem que detectem que o usuário está usando um proxy. Além disso, alteram com frequência o endereço IP apresentado a um site dificultando o rastreamento de tráfego;[¹]

- **Proxy Reverso:** Como o nome indica, o que esse proxy faz é o caminho inverso do que faria um “forward proxy” — aqueles situados entre o computador do usuário e o servidor. Isto é, ele está no intermédio do servidor para com a internet.[²]

- **Proxy de Distorção:** Esse tipo de servidor proxy se apresenta ao servidor de destino com um IP falso ou incorreto. Assim, mesmo não ocultando do servidor que um proxy está sendo utilizado, ele protege e esconde sua própria identidade. É normalmente utilizado para acessar sites específicos que só estejam disponíveis em um território, pois assim é possível ocultar e manipular a localização do servidor de origem que está tentando o acesso.[²]

Então, um Proxy Reverso filtra informações geradas por visitantes, encaminhando solicitações filtradas para o servidor. Por este motivo, um proxy reverso é mais comumente utilizado para lidar com requisições de servidores de hospedagem de sites, ou por grandes sites que precisam controlar o consumo de banda larga.

Um Proxy é um ótimo local para configurar um firewall.

---
[¹]: https://tecnoblog.net/responde/o-que-e-proxy-e-qual-a-diferenca-para-a-vpn/
[²]: https://www.hostinger.com.br/tutoriais/servidor-proxy
