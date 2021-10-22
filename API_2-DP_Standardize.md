# Aprendizagem por Projetos Integrados 2020-1
![logo_figma](https://user-images.githubusercontent.com/56441534/138282337-943cad4b-ddad-43b0-a959-aa154fa47837.png)

O desenvolvimento do projeto foi em torno da necessidade da empresa parceira, de realizar uma gestão de informação mais eficaz para garantir a qualidade, o uso adequado desta informação e gerar valor através dos dados.
Tendo em vista a mudança do modelo de operação do Cadastro Positivo.

### Parceiro Acadêmico
SPC - Brasil: Uma empresa de tecnologia vinculada à CNDL para processar e armazenar todas as operações de crédito realizadas pelas empresas associadas.

Conheça mais em [spcbrasil.org.br](https://www.spcbrasil.org.br/).

<img src="https://user-images.githubusercontent.com/56441534/138450126-38d20c22-1d13-463b-b7af-3174a93ea759.png" width="300"/>

***

### Visão do Projeto
DP Standardize se trata de uma ferramenta no formato Aplicativo Desktop que visa padronizar dados recebidos em remessas. O objetivo da ferramenta é ser utilizada como um Data Preparation, auxiliando no tratamento e padronização de uma remessa de dados, poupando um tempo valioso de trabalho antes de se agregar um valor maior a estes dados em futuros projetos.

![marketing_PI_11111](https://user-images.githubusercontent.com/57918707/87260544-dbc5ef80-c488-11ea-8987-faec80939a8b.png)

DP Standardize trabalha principalmente na padronização dos dados, sendo capaz de analisar qualquer tabela `xlsx` e `csv`. Permite a personalização dos campos e possibilita um apontamento de quais tipos de dados não podem conter em cada coluna.

A ferramenta permite também a geração de novos arquivos `xlsx` e `csv` oriundos dos arquivos originais. Depois de trabalhar na remessa de dados, as novas tabelas podem ser geradas, agora com os dados padronizados.

#### Lista de Requistos 
Os `Requisitos Funcionais` foram aplicados tendo em vista as seguintes Métricas de Qualidade disponibilizadas pela empresa parceira:

1. COMPLETUDE:
    - O campo de cadastro do estado referente a um endereço pode estar preenchido ou não, mesmo sendo obrigatório.

2. CONFORMIDADE:
    - Uma vez preenchido, tal preenchimento pode ser feito seguindo ou não as regras de negócio (formato, tamanho, etc).

3. CONSISTÊNCIA:
    - “Estado” é um dado presente em diversas bases, para um mesmo endereço é importante que todas as bases tenham o mesmo estado cadastrado.

4. UNICIDADE:
    - Em cada base que tenha dados geoespaciais é importante que o mesmo endereço, no mesmo estado, não tenha múltiplos registros.

5. ACURÁCIA:
    - Mesmo preenchido (completude) e no formato adequado (validade), o valor pode não se referir a nenhum estado existente na federação 
(ex: “RG” é uma sigla no formato adequado, porém não simboliza um estado).


Requisitos não Funcionais:
1. Aplicação Desktop.
2. Análise e tratamento de arquivos no formato `xlsx` e `csv`.

***

#### link do repositório no Github
[Repositório](https://github.com/Mateus-Prestes/Tratamento-de-dados-SPC/tree/master)


### Tecnologias adotadas na solução
Para obter o resultado esperado, a equipe utilizou as seguintes tecnologias:

![tecnologias_PI](https://user-images.githubusercontent.com/56441214/87261156-8c34f300-c48b-11ea-89cf-a96eef22661c.png)

- [Python](https://www.python.org/): Análise dos dados e alcance dos indicadores propostos.
- [Electron](https://www.electronjs.org/): Desenvolvimento da aplicação desktop GUI (Graphical User Interface).
- [HTML](https://devdocs.io/html/), [CSS](https://devdocs.io/css/) e [JavaScript](https://www.javascript.com/): Criação e desenvolvimento do design da Interface do usuário.
- [NodeJS](https://nodejs.org/en/) Por conta da utilização do Framework Electron, foi necessário migrar de python para NodeJS. 

### Funcionamento

Abaixo alguns gifs de demonstração da utilização da ferramenta DP Standardize em seu resultado final.

A aplicação contém um sistema de login e senha, onde cada Analista pode possuir seu cadastro.

A padronização das tabelas é feita de forma rápida, devendo somente arrastar ou clicar para adicionar a tabela ao local indicado.

A página seguinte já contará com seus metadados, que ao serem clicados, abrirão uma nova janela para inserção da personalização já citada no tópico acima.

Após a escolha das opções, clique em **Baixar Tabela**, assim seus dados padronizados serão gerados e salvos. 

![ezgif com-video-to-gif (4)](https://user-images.githubusercontent.com/57918707/87265117-47fc1f80-c498-11ea-8787-60aab6d6b2e4.gif)

Ao final, sua nova tabela será gerada e salva automaticamente na pasta **GenerateTable** para tomar o destino conveniente.

![ezgif com-video-to-gif (5)](https://user-images.githubusercontent.com/57918707/87265314-dc668200-c498-11ea-9721-fe048f989bf3.gif)

Para padronizar mais campos, volte ao DP Standardize, clique em **Limpar**, adicione as novas personalizações e clique em **Baixar Tabela** novamente.

![ezgif com-video-to-gif (6)](https://user-images.githubusercontent.com/57918707/87265504-5dbe1480-c499-11ea-9b1e-51bab99032d0.gif)

Assim será gerada uma nova tabela com as novas padronizações.

![ezgif com-video-to-gif (7)](https://user-images.githubusercontent.com/57918707/87265568-7c241000-c499-11ea-90f2-1b7276aeaa5b.gif)


### Contribuições Pessoais
Durante o desenvolvimento do projeto atuei em conjunto com os demais membros no tratamento dos dados em arquivos no formato `xlsx` e `csv` utilizando a linguagem de programação `python` em conjunto de algumas bibliotecas como `xlrd` e `matplotlib`.
Foram diversos tratamentos realizados nos dados, dentre eles:
- Verificação de valores nulos e repetidos.
- Geração de gráficos das métricas obtidas com os tratamentos.
![gráficos](https://user-images.githubusercontent.com/57918707/87258902-93ed9b00-c47d-11ea-8016-06595b8f563e.jpeg)

- Inserção, exclusão e listagem de dados confidenciais contidos nas remessas de dados. Com um Algoritmo capaz de ler as extensões `xlsx` e `csv` da base de dados enviadas pela empresa parceira e fazer a verificação em todas as tabelas.

- Também atuei fortemente no estudo e entendimento para com a equipe das regras de negócio e métricas solicitadas pelo cliente a serem atendidas.

### Hard Skills
Dentre as habilidades técnicas, obtive o seguinte avanço:
- Análise de dados com python3 de arquivos `xlsx` e `csv`:
    - Sei fazer com autonomia;
- Geração de gráficos com python3 e a biblioteca matplotlib:
    - Sei fazer com autonomia.
- Desenvolvimento dentro dos padrões da LGPD:
    - Aprendi a utilizar LGPD com acompanhamento de profissionais mais experientes.

### Soft Skills

Dentre as habilidades interpessoais performei minhas habilidades em Regras de Negócio e Relacionamento com Cliente. Quanto as habilidades na metodologia ágil, também foram bem trabalhadas através do SCRUM, onde tive pela primeira que vez que utilizar minhas habilidades e as ferramentas SCRUM com um cliente real. Todo esse desenvolvimento junto ao cliente foi acompanhado pelo corpo docente da FATEC São José dos Campos - Prof. Jessen Vidal.
