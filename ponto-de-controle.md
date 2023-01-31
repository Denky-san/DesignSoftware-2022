## Visão

Fornecer aos usuários uma forma de receber alertas de vagas de emprego personalizadas.

## Limite

- Deve-se usar a página do Twitter (@Technovagas1) para o registro de vagas na base de dados

- Deve-se usar Python para a construção do Backend

- Deve-se usar ReactJS no frontend web

- Deve-se usar o framework React Native para a contrução do app 

- Postgresql será utilizado como SGBD

- Deve-se usar AWS como serviço de computação em nuvem


## Contratos (Pontes de comunicação)

1. O usuário irá interagir com a aplicação de 3 formas diferentes:
 1.1 Por meio de um Aplicativo Mobile
 1.2 Por meio de uma página web
 1.3 Por meio de emails recebidos

2. O app irá interagir com o backend da aplicação por meio de uma API Rest

3. O backend se comunicará com a página de vagas do Twitter por meio da API do Twitter

4. O modelo de dados segue a estrutura relacional descrita no MER

5. Para acessar a API e sua documentação, o desenvolvedor utilizará a documentação gerada automaticamente pelo Swagger

6. Os commits no repositório deve serguir a atrutura GitFlow

7. Toda solicitação de PullRequest deve ser feita via GitHub após o código passar por revisão

8. O projeto deve ter 3 branches principais (prod, dev, hml)
  8.1 Branch de produção (prod): é a branch que contém o código da versão de produção
  8.2 Branch de Homologaçnao (hml): é a branch que contém um código espelho da branch de produção
  8.3 Branch de desenvolvimento (dev): é a branch usada para adicionar novas versões de código solicitadas com PullRequest

9. Deve-se realizar testes de unidade para as funções criadas no backend, frontend web e app
  9.1 No backend será usada a biblioteca unittest (Python)
  9.1 No app serão usadas as bibliotecas reac-native-test-library e jest
  9.2 No frontend web serão usadas as bibliotecas reac-native-test-library e jest

10. Os testes de integração serão realizados por meio de scripts para testes da API usando Postman

11. Testes de integração do app e frontend web devem ser realizados utilizando o FireEvent da biblioteca reac-native-test-library

## Design da solução

[Diagrama de Contexto](https://user-images.githubusercontent.com/29666978/202816195-2650b8c7-588e-4b17-9621-7adad2ef12a7.jpg)

[Diagrama de Container (Arquitetura)](https://raw.githubusercontent.com/Denky-san/DesignSoftware-2022/master/Diagramas/Diagrama%20de%20Container.jpg)

[Modelo de Dados (MER)](https://raw.githubusercontent.com/Denky-san/DesignSoftware-2022/master/Diagramas/DER.png)

[Diagrama de componentes WEB](https://raw.githubusercontent.com/Denky-san/DesignSoftware-2022/master/Diagramas/Diagrama%20de%20Componentes_Web.jpeg)

[Diagrama de componentes Mobile](https://raw.githubusercontent.com/Denky-san/DesignSoftware-2022/master/Diagramas/Web-server-basico.jpg)
