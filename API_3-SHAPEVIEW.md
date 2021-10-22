# Aprendizagem por Projetos Integrados 2020-2
![Logo](https://user-images.githubusercontent.com/56441534/138449995-c249e266-cdb5-4cdb-a018-45b64c0ae2c3.png)

O desenvolvimento do projeto foi em torno da necessidade da empresa parceira em ter uma ferramenta web que funcionasse como um mini-ETL, tendo como principais operações:
- Extrair dados de um arquivo `shapefile` e envia-los ao banco de dados; e
- Realizar o processo inverso convertendo os dados ingeridos no banco de dados em um novo arquivo `shapefile`.

### Parceiro Acadêmico
Visiona Tecnologia Espacial: Uma empresa brasileira integradora de sistemas espaciais.
Conheça mais em [visionaespacial.com.br](https://www.visionaespacial.com.br/).

<img src="https://user-images.githubusercontent.com/56441534/138451551-477b7c4e-12fc-48ab-bf1b-e0e7b70e1da4.png" width="400"/>

***

### Visão do Projeto
Shapeview se trata de uma ferramenta web capaz de realizar a ingestão de dados Geoespaciais contidos em um arquivo shapefile em um banco de dados e realizar também o processo inverso, convertendo os dados extraídos do banco para um novo arquivo `shapefile`.

<img src="https://user-images.githubusercontent.com/58118956/100612612-05759b00-32f2-11eb-992a-c1380029209a.png" width="700"/>

O Shapeview tem como objetivo funcionar como um mini-ETL, visando suprir a necessidade do cliente o Shapeview realiza a ingestão dos dados contidos em arquivos `Shapefile` de forma personalizada, podendo retirar dados e metadados que não são necessários em seu contexto de negócio.
A ferramenta também permite realizar a extração de dados contidos no banco de dados para um novo arquivo `shapefile`.

#### Lista de Requistos 

`Requisitos Funcionais` requeridos pelo cliente foram:
1. Carga de dados geográficos (ponto, linha e polígono) e seus atributos alfanuméricos em tabelas existentes de banco de dados geográficos; e
2. Recuperação de dados geográficos (ponto, linha e polígono) e seus atributos alfanuméricos armazenados em banco de dados geográficos.

`Requisitos não Funcionais`:
1. Linguagem Java ou python; 
2. Banco de Dados Geográficos PostGIS; e
3. Documentações.

***

#### link do repositório no Github
[Repositório](https://github.com/Mateus-Prestes/ShapeView)


### Tecnologias adotadas na solução
Para obter o resultado esperado, a equipe utilizou as seguintes tecnologias:
<p float="left">
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width="50"/> 
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flask/flask-original.svg" width="50"/>
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" width="50"/>
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" width="50"/>
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" width="50"/>
</p>

- [Python](https://www.python.org/): Em conjunto da biblioteca [Geopandas](https://geopandas.org/) para a análise dos dados geoespaciais e alcance dos indicadores propostos.
- [Flask](https://flask.palletsprojects.com/en/2.0.x/): Micro framework python para criação de aplicações web.
- [HTML](https://devdocs.io/html/), [CSS](https://devdocs.io/css/) e [JavaScript](https://www.javascript.com/): Criação e desenvolvimento do design da Interface do usuário.

### Funcionamento

Abaixo alguns gifs de demonstração da utilização da ferramenta Shapeview em seu resultado final.

A ferramenta conta com uma tela de login e senha para que o usuário tenha acesso a aplicação. Sendo assim é necessário que o usuário realize um cadastro, para ter acesso a ferramenta.

## Cadastro e Login
![Login-1](https://user-images.githubusercontent.com/56441534/138462716-afa4f79b-5a7d-40b6-9982-7071159ef908.gif)

## Cadastro do banco de dados
Para utilizar a ferramenta é necessário informar as credencias de seu banco de dados antes, criando uma conexão com o mesmo. Vale lembrar que o banco deve suportar dados geoespaciais.
![Crendenciando-2](https://user-images.githubusercontent.com/56441534/138464110-b5f063ac-0572-4d44-9a76-8725ebdaf78f.gif)

## Ingestão
Ingestão no bancos de dados geográfico dos dados oriundos de arquivos `shapefile`.

Antes de finalizar a ingestão é possível verificar a forma geométrica do arquivo, e podendo também salvar o PNG da forma geométrica.

![upload-3](https://user-images.githubusercontent.com/56441534/138463610-ac397e3d-9855-4dea-ae2d-28239f940b7e.gif)

Realizada a ingestão o úsuario pode verificar se os dados foram inseridos no banco, neste exemplo usamos o PGADMIN(interface gráfica do postgreSQl) para a verificação.

![dados no banco-4](https://user-images.githubusercontent.com/56441534/138463858-700d641b-63a3-46bb-b19a-d07cf7b99a9c.gif)

## Extração
Extração do bancos de dados geográfico de dados oriundos de arquivos `shapefile`. A extração gera um novo arquivo `shapefile`.

Extraindo os dados do banco de dados para a criação de um novo arquivo `shapefile` (.shp, .shx, .dbf, .prj e .cpg), é necessário informar de qual tabela o ShapeView irá extrair os dados.

![Download-5](https://user-images.githubusercontent.com/56441534/138464037-0ba802fd-d0f0-4c42-9565-acfdd1bdf3be.gif)


### Contribuições Pessoais
Durante o desenvolvimento do projeto atuei fortemente na ferramenta ETL, trabalhando as seguintes funcionalidades:
- Extração e transformação dos dados de arquivos `shapefile`;
- Configuração do ambiente e integração banco de dados;
- Ingestão e extração dos dados geoespaciais contidos banco de dados da aplicação;
- Geração de arquivos `shapefile` a partir da extração dos dados geoespaciais contidos banco;
- Plotagem das formas geométricas (ponto, linha e polígono) dos dados geoespaciais; e
- Desenvolvimento do servidor web utilizando o microframework `flask`.

### Hard Skills
Dentre as habilidades técnicas, obtive o seguinte avanço:
- Análise de dados geoespaciais de arquivos `shapefile` utilizando python3 em conjunto biblioteca Geopandas:
    - Sei fazer com autonomia;
- Geração de formas geométricas(ponto, linha e polígono) utilizando python3 e a biblioteca matplotlib:
    - Sei fazer com autonomia.
- Desenvolvimento do seridor web com `flask`:
    - Sei fazer com autonomia.
- Ingestão e extração de dados de bancos de dados relacionais:
    - Sei fazer com autonomia.

### Soft Skills
Durante este projeto tive a oportunidade de ser o Scrum Master da minha equipe, podendo exercitar varias habilidades interpessoais, como:
- Solução de problemas complexos;
- Organização;
- Empatia;
- Comunicação e escuta ativa;
- liderança;
- Flexibilidade e adaptabilidade.

 
