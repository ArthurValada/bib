SSL, ou Secure Sockets Layer, é um protocolo de segurança projetado para garantir a privacidade e a integridade dos dados transmitidos pela Internet. Originalmente desenvolvido pela Netscape, o SSL foi substituído pelo TLS (Transport Layer Security), mas muitas vezes o termo "SSL" ainda é usado de maneira geral para se referir aos protocolos de segurança da camada de transporte.

Ele utiliza criptografia para proteger os dados contra interceptação por terceiros mal-intencionados. Aqui estão alguns dos principais objetivos do SSL/TLS:

1. **Confidencialidade:** Os dados transmitidos entre o cliente e o servidor são criptografados, tornando difícil para qualquer pessoa não autorizada entender ou utilizar as informações transmitidas.
2. **Integridade dos Dados:** O SSL/TLS inclui mecanismos que garantem que os dados não foram alterados durante a transmissão.
3. **Autenticação:** O protocolo permite a autenticação do servidor para garantir que o cliente esteja se conectando ao servidor desejado. Além disso, a autenticação mútua pode ser configurada para autenticar também o cliente perante o servidor.
4. **Compatibilidade:** SSL/TLS é amplamente suportado pelos navegadores e aplicativos, tornando-o uma escolha comum para proteger a comunicação na web.

Para usar SSL/TLS, um site geralmente precisa obter um certificado SSL de uma Autoridade Certificadora (CA). Esse certificado é uma espécie de "selo de aprovação" digital que ajuda a verificar a identidade do proprietário do site.

É importante notar que, com o tempo, o uso do termo "SSL" tem se expandido para incluir tanto o SSL quanto suas versões mais recentes, como TLS 1.0, TLS 1.1, TLS 1.2, e assim por diante. No entanto, é altamente recomendável usar versões mais recentes, pois versões mais antigas podem ter vulnerabilidades conhecidas.

## Funcionamento
Três chaves são usadas para configurar a conexão SSL: as chaves pública, privada e de sessão. Qualquer conteúdo criptografado com a chave pública só pode ser descriptografado com a chave privada e vice-versa. Como a criptografia e a descriptografia com chaves privada e pública consomem muita capacidade de processamento, elas só são usadas durante o ==handshake SSL== para criar uma chave de sessão simétrica. Depois que a conexão segura é feita, a chave de sessão é usada para criptografar todos os dados transmitidos. [¹]

### Detalhamento[¹]

1. Um host se conecta a um servido protegido por SSL. É solicitada a identificação do servidor;
2. O **servidor** envia uma cópia de seu certificado SSL, inclusive sua chave pública;
3. O host verifica a raiz do certificado em uma lista de CAs confiáveis ​​e se o certificado não expirou, não foi revogado e se o nome comum é válido para o site ao qual ele está se conectando. Quando o host confia no certificado, ele cria, criptografa e retorna uma chave de sessão simétrica usando a chave pública do servidor.
4. O **servidor** descriptografa a chave de sessão simétrica usando a chave privada e retorna uma confirmação criptografada com a chave de sessão para iniciar a sessão criptografada.
5. O **servidor** e o host agora criptografam todos os dados transmitidos com a chave de sessão.
## Quais são os tipos de certificados SSL?

Um certificado pode ser aplicado a um único site ou a diversos sites, dependendo do tipo:[²]

- **Domínio único:** um certificado SSL de domínio único aplica-se apenas a um domínio;[²]
- **Curinga:** como um certificado de domínio único, um certificado SSL curinga aplica-se apenas a um domínio. No entanto, também inclui os subdomínios desse domínio;[²]
- **Multidomínio:** como o próprio nome indica, os certificados SSL multidomínio podem ser aplicados a vários domínios não associados;[²]

Os certificados SSL também vêm com diferentes níveis de validação. Um nível de validação é como uma verificação de antecedentes, e o nível muda dependendo do rigor da verificação.[²]
### Tipos de validação
- **Validação do domínio:** esse é o nível de validação menos rigoroso e mais barato. Tudo o que um empresa precisa fazer é provar que controla o domínio.
- **Validação da organização:** esse é um processo mais manual — a autoridade de certificação entra em contato diretamente com a pessoa ou empresa e solicita o certificado. Esses certificados são mais confiáveis para os usuários.
- **Validação estendida:** requer uma verificação completa dos antecedentes de uma organização antes que o certificado SSL possa ser emitido.
## Links Úteis
- [Evolução do SSL - Inglês](https://www.digicert.com/blog/evolution-of-ssl) 
- [O que é a criptografia SSL?](https://www.digicert.com/faq/cryptography/what-is-ssl-cryptography)


---
[¹]: https://www.digicert.com/pt/what-is-an-ssl-certificate#:~:text=inserir%20informa%C3%A7%C3%B5es%20confidenciais.-,O%20que%20%C3%A9%20SSL%20(Secure%20Sockets%20Layer)%3F,por%20exemplo%2C%20o%20Outlook).
[²]