# Aprendizagem por Projetos Integrados 2021-1
<img src="https://user-images.githubusercontent.com/56441534/142959484-12836894-06f3-4346-91ce-1fb6891da026.png" width="300"/>

A necessidade de uma ferramenta capaz de gerar Atas de Reunião dinâmicas e funcionais levou a empresa parceira a ter a iniciativa de apresentar o tema aos alunos do quarto Semestre de Análise e Desenvolvimento de Sistemas da FATEC São José dos Campos.
As principais funcionalidades da ferramenta deveriam ser:

- Funcionalidades de cadastro;
- Controle de acesso;
- Logs de execução; 
- Geração e monitoramento de ata de reunião; e 
- Assinatura digital.

### Parceiro Acadêmico
IACIT: Empresa brasileira, fundada em 1986 e com capacitação tecnológica para o desenvolvimento de produtos e sistemas aplicados ao Auxílio  e ao Controle do Tráfego Aéreo e Marítimo (CNS/ATM); Meteorologia Radar; Telemetria; Redes Integradas; Comunicação; Defesa e Segurança Pública.
Conheça mais em [iacit.com.br](https://www.iacit.com.br/).

<img src="https://user-images.githubusercontent.com/56441534/142960594-c77702b5-7bda-492d-97f7-fbbb2475e6b2.png" width="400"/>

***

### Visão do Projeto
O EasyAta é uma aplicação web que tem como objetivo gerir Atas de Reunião,
conta com funcionalidades de cadastro, controle de acesso, geração e monitoramento das Atas de Reunião e assinatura digital. 
A aplicação facilita o processo de criação e registro de Atas de reunião, e ao mesmo tempo permite que todas as informações relevantes da reunião sejam armazenadas de maneira limpa e organizada. 

Conta também com um sistema de controle de acesso, com restrições e privilégios que convém aos tipos de usuários do sistema. 

Com todo esse pacote o EasyATA oferece uma gestão segura dos dados e informações abordadas em uma reunião. 

#### Lista de Requistos 

`Requisitos Funcionais` requeridos pelo cliente foram:
1. Cadastro de Usuários, Cadastro de Perfil de Acesso, Cadastro de modelo de ata de Reunião.
    - O cadastro de usuário deve conter os seguintes campos: Nome, Título/Cargo,Área/Empresa, E-mail e Telefone;
    - Todo usuário deve ter pelo menos um perfil de acesso;
    - O perfil de acesso define quais funcionalidades o usuário pode acessar, sendo: 
        - Administrador: Acesso total ao sistema;
        - Usuário: Acesso ao cadastro do modelo de ata de reunião, a geração de ata de reunião, ao monitoramento de ata de reunião e à imprimir ata de reunião em PDF e Excel;
        - Gerência: Acesso aos relatórios do sistema, à aprovação do modelo de ata de reunião e a imprimir ata de reunião em PDF e Excel;
        - A aplicação deve ter pelo menos um usuário administrador o qual não pode ser excluído;

2. Login; Logout;
3. Gerar Ata de Reunião;
4. Monitorar Ata de Reunião;
    - Deve ser exibida uma listagem com a situação es todas as atas de reunião. Esta listagem deve possuir filtros: Por Estado, Por Data de Criação da Ata e Por Pauta;
    - A listagem pode ser ordenada de forma crescente e decrescente;
    - Uma Ata de Reunião pode ter os seguintes estados: Nova, Revisada, Assinada e Enviada.

`Requisitos não Funcionais`:
1. Backend: Linguagem Java (sugestão); 
2. Frontend: HTMLS, CSS 3,15, Angular ou React;
3. Ser usual com dispositivos móveis;
4. Estar disponível no idioma Português do Brasil;
5. Manual de usuário com prints de telas e explicação das funcionalidades;
6. Registros de testes de todas as funcionalidades; e
7. Código fonte do sistema documentado.

***

#### link do repositório no Github
[Repositório](https://github.com/DaviNeves0/EasyATA)


### Tecnologias adotadas na solução
Para obter o resultado esperado, a equipe utilizou as seguintes tecnologias:

![](https://i.ibb.co/9bMTdSP/API4-GITHUB.png)</br>
</br>

<p float="left">
    <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white"/> 
    <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white"/>
    <img src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E"/>
    <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB"/>
    <img src="https://img.shields.io/badge/Sass-CC6699?style=for-the-badge&logo=sass&logoColor=white"/>

</p>
<p float ="left">
    <img src ="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white"/>
    <img src ="https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=whitee"/>
    <img src ="https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white"/>
</p>

- [Java](https://www.oracle.com/br/java/): Em conjunto do framework `Spring` para criação do sistema web;
- [Spring](https://spring.io/): Framework java para criação de aplicações web.
- [MySQL](https://www.mysql.com/): Sistema gerenciador de Banco de Dados Relacional. Utilizado para salvar os cadastros de usuários, seus níveis de acesso e o registro de novas Atas de Reunião, registrando todo o ciclo de vida de uma Ata de Reunião.
- [HTML](https://devdocs.io/html/), [CSS](https://devdocs.io/css/) e [JavaScript](https://www.javascript.com/): Criação e desenvolvimento do design da Interface do usuário.
- [React](https://pt-br.reactjs.org/): Uma biblioteca JavaScript para criar interfaces de usuário


### Funcionamento

Abaixo alguns vídeos para demonstração da utilização da ferramenta EasyATA em seu resultado final.

## Cadastro e Login

A ferramenta dispõe uma tela de login que solicita a senha do usuário cadastrado no banco. Portanto, para que o usuário tenha acesso a aplicação é necessário que o seu cadastro seja finalizado, dessa forma o acesso a ferramenta é disponibilizado.

Vale lembrar que todo usuário cadastrado, inicialmente é um usuário de nível comum e seu nível de acesso só pode ser concedido por um usuário de nível Administrador.

#### **Cadastrando um usuário e aceesando o sistema**:
https://user-images.githubusercontent.com/56441534/142968754-aace60ea-403a-4637-9806-555e4afb405d.mp4


## Geração de Atas de Reunião
O Usuário preenche os dados e ao enviar o formulário, a Ata de Reunião é salva no banco de dados com o status de Nova. Neste momento também é possível realizar download do documento nos formatos `pdf` e `csv`.

#### **Criando uma Ata de Reunião**
https://user-images.githubusercontent.com/56441534/142968947-ab95af53-ed92-441d-bb0b-74b4b5b01170.mp4

## Revisando de Atas

Após a criação de uma Ata de Reunião, é possível solicitar uma revisão para a mesma. 

Para solicitar uma revisão deve-se informar o assunto, Responsável e o Prazo da Revisão podendo antes de solicita-la, editar os dados contidos na Ata.

Neste momento, é possível fazer o download da Ata para os formatos `pdf` e `csv`.

#### **Revisão de Ata de Reunião**
https://user-images.githubusercontent.com/56441534/142969763-3d25e989-4538-4a9e-868b-3a77d9f2d528.mp4

## Análise de Ata Pendente

Após ser solicitada a revisão, as atas passam de novas para pendentes e são exibidas para o Gerente ou Administrador avalia-las. 

Atas aprovadas passam para a fase de assinaturas. Atas reprovadas voltam para o estado de uma nova ata, podendo assim ser solicitada para uma nova revisão.

#### **Aprovando Ata de Reunião**
https://user-images.githubusercontent.com/56441534/142970433-3e152976-9afd-4eaa-9349-0655034d62d0.mp4

#### **Assinando Ata de Reunião**
https://user-images.githubusercontent.com/56441534/142972156-9f00effa-1649-4449-8660-95b010ba702e.mp4


Todas as telas de listagem de atas contam com filtros e sistemas de pesquisa para facilitar a busca do documento desejado.

Basicamente esse é processo do clico de vida de uma Ata de reunião criada pelo EasyATA.

![diagrama (2)](https://user-images.githubusercontent.com/56441534/120910907-1ca69400-c659-11eb-92b6-22799b94d875.png)

## Controle de acesso

Todo usuário cadastrado, por padrão é um usuário comum e seu nível de acesso pode ser alterado somente por um usuário de nível Administrador. um usuário Administrado também é capaz de excluir usuários do banco de dados.

**Níveis de acesso:**
1. Usuário Comum:
    - Criação e envio de atas de Reunião ao banco de dados;
    - Download da atade reunião nos formatos `pdf` e `csv`;
    - Solicita Revisão para atas novas e atas ja reprovadas.

2. Gerente:
    - Todas as funcionalidades do Usuário Comum; e
    - Aprova ou Reprova as Atas que forem solicitadas para uma revisão.

3. Administrador:
    - Acesso total as funcionalidades da aplicação;
    - Sistema de controle de cadastro de usuários, podendo mudar o nível de qualquer Usuário para Administrador, Gerente ou Usuário Comum; e
    - Exclusão de registros de usuários no banco de dados da aplicação.

#### **Alterando nível de acesso**
https://user-images.githubusercontent.com/56441534/142972085-5ef452ec-b11c-4aca-a91f-e677c2d65948.mp4

#### **Deletando Usuário**
https://user-images.githubusercontent.com/56441534/142972447-fc3885ba-cf3f-4663-8d7b-0fad9ef35f4c.mp4

### Contribuições Pessoais
Durante o desenvolvimento do projeto atuei fortemente na ferramenta ETL, trabalhando as seguintes funcionalidades:
- Extração e transformação dos dados de arquivos `shapefile`;
- Configuração do ambiente e integração com banco de dados;
- Ingestão e extração dos dados geoespaciais contidos no banco de dados da aplicação;
- Geração de arquivos `shapefile` a partir da extração dos dados geoespaciais contidos no banco;
- Plotagem das formas geométricas (ponto, linha e polígono) dos dados geoespaciais; e
- Desenvolvimento do servidor web utilizando o microframework `flask`.

### Hard Skills
Dentre as habilidades técnicas, obtive o seguinte avanço:
- Criação de sistema web utilizando linguagem de programação `Java` e conjunto do Framework `Spring`:
    - Sei fazer com ajuda.
- Criação de UI (User Interface) utilizando `HTML`, `CSS`, `JavaScript` e `React JS`:
    - Sei Fazer com Ajuda.
- Integração com banco de dados relacional utilizando ORM com `java` e `Hibernate`:
    - Sei fazer com autonomia.

### Soft Skills
Durante este projeto tive a oportunidade de ser o Scrum Master da minha equipe pela segunda vez, onde consegui aprimorar minhas habilidades interpessoais:
- companheirismo;
- Solução de problemas complexos;
- Organização;
- Empatia;
- Comunicação e escuta ativa;
- liderança;
- Flexibilidade e adaptabilidade.

 
