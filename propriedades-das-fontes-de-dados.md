-  Qual o tipo do sistema de origem dos dados? É uma aplicação, um sistema de mensageria ou outro?

Há um sistema de origem dos dados, nomeadamente os tweets da timeline de um perfil do Twitter, identificado por @tecnovagas1.
Tais tweets podem ser acessados pela [API do Twitter](https://developer.twitter.com/en/docs/twitter-api).
Há n níveis de acesso distintos à API do Twitter.


- Como os dados são persistidos e recuperados? Eles são persistidos permanentemente ou temporariamente?

O gerenciamento do armazenamento dos tweets é gerenciado internamente pelo Twitter. Com relação a timeline de um usuário,
é possível recuperar os 3200 tweets, retweets, respostas e menções mais recentes. Os tweets são retornados em ordem cronológica
reversa, ou seja, começando a partir do mais recente. Por fim, os resultados são paginados em até 100 tweets por página. Também
é possível recuperar o tweet de um usuário de por stream (fluxo contínuo), isto é, logo após o tweet ser gerado, através da
funcionalidade denominada **Filtered stream**.

Informações sobre timeline: https://developer.twitter.com/en/docs/twitter-api/tweets/timelines/introduction
Informações sobre leiura de tweets em stream: https://developer.twitter.com/en/docs/twitter-api/tweets/filtered-stream/introduction



- Qual a frequência em que os dados são gerados? Quantos eventos de gerações ocorrem por intervalo de tempo e quantos bytes de dado?

TODO


- Qual o nível de consistência e confiabilidade esperado? Podem ocorrer valores nulos em campos obrigatórios?
Podem ocorrer duplicações? Podem ocorrer má formatações ou outro tipos de erros?

TODO


- Dados podem chegar fora de ordem ou com atraso?

TODO


- Será necessário cruzar conjuntos de dados, arquivos, tabelas ou documentos diferentes?

TODO


- O schema dos dados gerados é *schemaless* ou *fixed schema*?

TODO


- Como mudanças no schema dos dados são tratadas e comunicadas?

TODO


- Como ingerir (ler) dados do sistema de origem afeta seu desempenho?

TODO
