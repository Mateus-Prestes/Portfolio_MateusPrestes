# Aprendizagem por Projetos Integrados 2021-1
<img src="https://user-images.githubusercontent.com/56441534/143027596-7630130d-e962-4fbf-9f9b-27f7d949a375.png" width="300"/>

No quinto semestre do Curso de Análise e Desenvolvimento de sistemas na FATEC - São José dos Campos, a empresa parceira identificou uma oportunidade de anunciar vendas de carros através de uma aplicação mobile, onde o próprio anunciante conseguisse acompanhar o andamento do seu anúncio (quantidade de visualizações/quantidade de interesses).
A ferramenta tem como objetivo ser composta pelas seguintes características:

- Comunicação entre comprador/vendedor realizada através do sistema;
- Segurança de todos os dados gravados;
- Solução que seja robusta; e
- Alto índice de disponibilidade/responsividade, pois, se necessário implementar pequenas melhorias/correções, o sistema deve ficar o menor tempo possível em atualização.

### Parceiro Acadêmico
GSW: Oferece soluções em Tecnologia da informação que promovem melhorias significativas no gerenciamento e controle dos processos e negócios.
Conheça mais em [gsw.com.br](http://www.gsw.com.br/index.php).

<img src="https://user-images.githubusercontent.com/56441534/143023020-6b1dc732-0d3b-4590-a1e2-f2a860081a67.png
" width="400"/>

***

### Visão do Projeto
O OnlyMotors é um sistema de venda de veículos online onde os anunciantes têm acesso a um painel de gerenciamento de anúncios podendo vizualizar ou fazer modificações nos seus anúncios. 

A ferramenta ainda traz a possibilidade do usuário gerar relatórios para ter mais informações sobre os veículos anúnciados. 

O usuário comprador tem acesso aos anúncios, onde pode utilizar filtros de pesquisa, e facilitar o encontro com o anúncio desejada. Podendo ainda entrar em contato com os vendedores através do chat em tempo real integrado a aplicação.

#### Lista de Requistos 

`Requisitos Funcionais` requeridos pelo cliente foram:
1. Importar arquivos estruturados (csv) com os dados do anúncio e com os dados de anunciantes/usuário; 
2. Importação de fotos do anúncio, podendo variar de acordo com a fonte do dado.
3. O sistema deve cadastrar automaticamente a senha para o primeiro acesso, obrigando a alteração no segundo acesso;
4. Comunicação entre comprador e vendedor através de um sistema em tempo real;
5. Painel administrativo do anúncio;
6. Informações sigilosas devem ser ocultadas conforme a LGPD;
7. Funcionalidades de pesquisa de anúncios; e
8. Gerar de relatórios.

`Requisitos não Funcionais`:
1. LGPD;
2. Alta disponibilidade (99%);
3. Segurança da informação (dados extremamente sigilosos);
4. A expectativa de anúncios ativos por mês é de 7 milhões;
5. O sistema intuitivo, pois, não contará com manual de utilização e deve ateder a todo tipo de público;
6. Desenho da Arquitetura aplicação;
7. Documento de implantação;
8. Documento de estratégia de branchs/ versionamento
9. Documentação das APIs (Implementar com uma ferramenta, ex.: Swagger);
10. Relatório com o histórico do build automatizado; e
11. A quantidade de visualizações do anúncio, é extremamente confidencial, os usuários não
podem visualizar dados de outros anúncios.
***

#### link do repositório no Github
[Repositório](https://github.com/onlymotors)


### Tecnologias adotadas na solução
Para obter o resultado esperado, a equipe utilizou as seguintes tecnologias:

![image](https://user-images.githubusercontent.com/56441534/143033089-a0cb7912-4e3c-4bba-8fe7-360ad8ae9db1.png)

<p float="left">
    <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white"/> 
    <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white"/>
    <img src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E"/>
    <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB"/>
    <img src="https://img.shields.io/badge/Expo%20Go-black?style=for-the-badge&logo=expo&logoColor=white"/>

</p>
<p float ="left">
    <img src ="https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white"/>
    <img src ="https://img.shields.io/badge/swagger-8bbf3d?style=for-the-badge&logo=swagger&logoColor=white"/>
    <img src ="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white"/>
    <img src ="https://img.shields.io/badge/firebase-yellow?style=for-the-badge&logo=firebase&logoColor=white"/>
</p>

- [HTML](https://devdocs.io/html/), [CSS](https://devdocs.io/css/) e [JavaScript](https://www.javascript.com/): Criação e desenvolvimento do design da Interface do usuário.
- [React Native](https://reactnative.dev/): Para a criação de aplicativos Nativos.
- [Expo Go](https://expo.dev/): Plataforma de código aberto para fazer aplicativos nativos universais para Android, iOS e web com JavaScript e React.
- [Node](https://nodejs.org/en/): Construção do serviço API's contendo as rotas e funcionalidades da aplicação.
- [Mongo](https://www.mongodb.com/): Banco de dados não relacional, baseado em documentos.
- [Firebase](https://firebase.google.com/): Utilizado para hospedagem de arquivos de imagem.
- [docker](https://www.docker.com/): Utilizado para facilitar a instalação do sistema entre os desenvolvedores

### Funcionamento

Abaixo alguns vídeos para demonstração da utilização da ferramenta OnlyMotors em seu resultado final.

## Chat e Pesquisa
1. Registro de Anúncios no sistema. (o sistema de cadastro de usuários segue o mesmo padrão).

<p align=center>
<img src ="https://user-images.githubusercontent.com/56441534/143032011-a2af8cd9-5c03-4217-913a-e6ce21e3f3a0.gif" width=250/>

2. Cadastro de usuário. Painel de controle onde podemos ver o usuário alterando dados pessoais e seus anúncios. 

https://user-images.githubusercontent.com/56441534/143039123-8b3985e6-1df7-43ca-a382-a9ff30762b41.mp4


4. Pesquisa de veículos anunciados, com filtros de:
    - Marca;
    - Modelo;
    - Ano; e
    - Valor.

5. Chat em tempo real, onde um usuário comum entra em contato com o anúnciante através de outro dispositivo.

![chat_e_pesquisa](https://i.imgur.com/rv5bvbF.gif)

6. Documentação Viva do serviço de API utilizando `Swagger`:
![image](https://user-images.githubusercontent.com/56441534/143042377-7157b75b-f995-4672-b79a-941b06ec4a3a.png)
![image](https://user-images.githubusercontent.com/56441534/143042434-76c84b6a-43f8-4dc5-b5d0-a2b699be4eb3.png)
![image](https://user-images.githubusercontent.com/56441534/143042124-20a38843-ee94-4358-b568-1b59f5304632.png)
![image](https://user-images.githubusercontent.com/56441534/143042156-9b34e409-3db1-4fac-8d6a-15debacd8df1.png)


### Contribuições Pessoais
Para desenvolver este projetos, utilizamos a stack MERN (React.js + Node.js + Express + MongoDB). Durante o desenvolvimento, atuei no BackEnd, subindo o servidor e criando as rotas. Também atuei criando a documentação viva do servidor de API, utilizando a ferramenta Swagger. 

Para a ultima entrega deste projeto, trabalhei na criação de um Dockerfile e um Docker-compose, onde o Docker-Compose contém dois serviços integrados aplicados ao API.

### Hard Skills
Dentre as habilidades técnicas, obtive o seguinte avanço:
- Criação de serviços de API utililizando `Node JS`:
    - Sei fazer com ajuda.
- Criação de UI (User Interface) utilizando `HTML`, `CSS`, `JavaScript` e `React JS`:
    - Sei Fazer com Ajuda.
- `Docker`:
    - Sei utilizar com ajuda.
- Criação de Documentação viva de APIs utilizando `Swagger`:
    - Sei fazer com autonomia.
- Utilização do banco de dados não relacional `Mongo DB`:
    - Sei fazer com autonomia.

### Soft Skills
Foi utilizado a metodologia SCRUM para o gerenciamento do tempo, cards e planejamentos.
Durante este projeto atuei como desenvolvedor backend em minha equipe, consegui participar ativamente das reuniões e entrega dos requisitos solicitados pelo cliente.
 
