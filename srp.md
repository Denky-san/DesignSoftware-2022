# ANÁLISE DE APLICAÇÃO DO PRINCÍPIO DA RESPONSABILIDADE ÚNICA


  Concebido à luz das boas práticas de programação (SOLID), o projeto “Robô Buscador de Tweets” possui maior clareza e organização, pois os componentes do software foram separados com responsabilidades únicas. Além disso, o projeto foi pensado para ter menos acoplamento, ou seja, cada componente tem uma responsabilidade única, há menos dependência entre eles, o que torna o software mais fácil de mudar e testar. 
Como o SRP (single-responsibility principle) foi seguido durante o design, é mais provável que componentes possam ser reutilizados em outros projetos. Isso evita retrabalho, pois melhora a reutilização de código, e fica mais fácil expandir ou modificar o sistema sem afetar outras partes.
Os seguintes artefatos de design do projeto foram analisados a fim de se determinar se o SRP foi seguido ou não :

#### Pipelines

#### Diagrama de container

#### Diagrama de componentes (WEB e Mobile)

#### Diagrama entidade relacionamento

## Abaixo estão os resultados das análises.

#### Pipelines
  As responsabilidades de cada pipeline foram separadas, um para compreender a fonte de dados, e outro para de fato coletar os dados.
#### Diagrama de Container
  O usuário (stakeholder) pode interagir tanto com a Aplicação WEB, quanto com a Aplicação Mobile. Estas estão isoladas, e seus funcionamentos estão acondicionados dentro de si, de modo que apenas interagem com a API para comunicar a requisição de dados com a API do Twitter, e com o serviço de notificações. Este último, por ser externo às duas aplicações, foi pensado de modo a seguir o SRP. Por fim, a API interage com o Banco de Dados, que novamente segue o SRP.
#### Diagrama de Componentes

O diagrama de componentes possui cinco componentes: View, Action Creator, Dispatcher, Store e Web API. Esta separação de funcionalidades, junto com a aplicação do padrão Observer segue o princípio da responsabilidade única em amplo espectro.
#### Diagrama entidade relacionamento

No diagrama entidade relacionamento há cinco entidades: Usuario, Especializacao, Localizacao, Vaga, Fonte de Vaga, e Empresa, e uma entidade fraca; Pilha de alerta de vagas. Analisemos cada um deles:

      Usuario: possui seis atributos, todos condizentes com seu propósito e escopo. Relaciona-se com Pilha de alerta de vagas, e Especializacao. 

      Especializacao: possui um atributo, e relaciona-se com Usuario e Vaga. Poderia ser um atributo de Vaga? Consideramos que não.

      Localizacao: possui dois atributos e relaciona-se com Vaga. Poderia ser um atributo de Vaga, mas optamos por separá-la pois tem atributos próprios, e no código envolve métodos próprios para preenchê-los, o que foge ao propósito de Vaga.

      Vaga: possui três atributos, e relaciona-se com todas as entidades, exceto Usuario. Vaga - se não fosse utilizado o SRP - seria muito grande.

      Fonte de Vaga: possui dois atributos, e relaciona-se com Vaga. Poderia ser um atributo de Vaga, mas optamos por torná-la em entidade, que relaciona-se com Vaga.

     Empresa: Possui dois atributos, e relaciona-se com Vaga. Condizente com seu próprio escopo.

     Pilha de alerta de vagas: não possui atributos, e relaciona-se com Usuario e Vaga.

Dessa forma, fica claro o emprego do padrão SRP para guiar a criação do diagrama entidade relacionamento.
